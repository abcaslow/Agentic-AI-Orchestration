# Jev (TypeSafe AI) and Sim — session notes

*Compiled 9 October 2026 from a Claude Code session on itpietraining.com. Covers what Jev is, how to run it, whether it belongs in Sim workflows, and how Sim already supports it.*

---

## 1. What Jev is

- **Jev** is TypeSafe AI's first "System One" model: a **decision model, not a chat model**. TypeSafe AI was founded by former OpenAI researcher Diogo Almeida; Jev was released in early October 2026.
- You send it a **state** (text, a JSON object, or an array) and a set of **typed questions**. The answers you allow are declared in advance, and Jev returns one of them with a **probability**. It generates no text, so there is nothing to parse and no free-form hallucination.
- Three question types:
  - **Choice** — pick one option, with a probability for every option.
  - **Score** — place the input on a scale.
  - **Noul** — the probability that a yes/no statement is true.
- **Vendor claims** (not independently verified): 40–200× faster than frontier LLMs on comparable tasks; $0.042 per million input tokens, output free.
- Good fits per TypeSafe: **routing, classification, triage, agent control.**

## 2. The best "harness" for Jev

Because Jev does not chat, there is no chat or coding-agent harness to run it in. TypeSafe's own docs say there is **no `model: "jev-latest"` setting for coding agents**. The right harness is **ordinary code that stays in control and asks Jev narrow decisions**.

**Calling it — TypeSafe SDK**
- Python: `pip install typesafe-sdk` (or `uv add typesafe-sdk`); a JavaScript SDK also exists.
- API key in `TYPESAFE_API_KEY` (create keys at https://console.typesafe.ai/keys).
- Endpoint: `https://api.typesafe.ai/v1/systemone`.

```python
from typesafe_sdk import Choice, TypeSafeClient
client = TypeSafeClient()
r = client.system_one(
    state="Customer says the invoice was charged twice",
    questions={"department": Choice(
        instructions="Which team should handle this",
        criteria={"billing": "Payment issues",
                  "technical": "Bugs or integration problems"})})
print(r.answers["department"].choice)
```

**Writing the integration — coding agent + TypeSafe skill**
- Claude Code:
  ```bash
  claude plugin marketplace add typesafe-ai/skills
  claude plugin install typesafe@typesafe-ai
  ```
- Other agents: `npx skills add typesafe-ai/skills --skill typesafe-ai`
- The skill gives the agent full context on the Jev API so it writes correct integrations.

**In a larger AI system — TypeSafe's documented patterns**
- Intent routing (which handler, LLM or human gets a request)
- Confidence-gated routing (escalate to a big model only when Jev is unsure)
- Guardrails on LLM input and output
- RAG passage classification and citation checking

## 3. Does Jev make sense in a Sim workflow?

**Yes — for narrow decision steps, not as a replacement for the Claude agents.**

Good fits in our existing workflows:
- **`kb2itpieapi` endpoint choice.** Picking 1 of its 12 ITPIE endpoints is a Jev **Choice**. Its probability enables a confidence gate: if Jev is very sure, skip the Claude planner for that step; otherwise fall back to it.
- **Scope checks.** "Can ITPIE / the knowledge base answer this?" in `kb2itpieapi` and in netprog-qa (whose log table already has `in_scope` and `branch` columns) is a **Noul**.
- **Guardrails and RAG passage filtering** before Claude answers.

Poor fits:
- Anything that needs text. Jev cannot write the answer, and cannot pull a free-text search term (like `csr1`) out of a question — `kb2itpieapi` still needs Claude for that.
- "Find a restaurant" — it is all generation and knowledge.

Practical points:
- **Cost** is negligible; our workflows are dominated by Claude's time, so speed only matters if Jev lets us skip a Claude call.
- **Risk:** brand-new vendor and model; accuracy and speed figures are TypeSafe's own; one more API key and outside service.

**Recommended pilot:** in `kb2itpieapi`, run Jev beside the Claude planner without affecting output, log both endpoint picks to a Sim table, and compare after a few dozen real questions. If Jev agrees with Claude when confident, switch to confidence-gated routing.

## 4. Sim's agent block runs Jev natively

*Correction to an earlier answer in the session, which said Jev would need an API block.*

Verified in the Sim code running at localhost:3000 (the 2026-09-29 release). sim.ai cloud runs the current release, so it should be there too.

- Sim registers **TypeSafe** as a model provider ("Jev evaluation models for classification, scoring, and agent decisions") with models **`jev-latest`** (default), **`jev-1.13.0`** and **`jev-preview`**: 64k context, $0.042 per million input tokens, output free.
- In an **agent block**, pick a Jev model and the Messages box is replaced by two fields:
  - **State** — the text (or JSON object or array) to evaluate; a reference such as `<normalizeinput.result.question>` works.
  - **Questions** — a JSON map of question IDs to Jev Choice, Score or Noul questions.
- **Output:** `answers`, typed per question (e.g. `<blockname.answers.department.choice>`). Sim checks each answer matches the questions asked, including that a Choice answer is one of the declared options. `content` holds the same answers as a JSON string.
- In Jev mode the block **rejects** a system prompt, chat messages, tools, a response format, or memory, and returns no text. It is a decision step; a condition block or a Claude agent block acts on its answer.
- The block calls `https://api.typesafe.ai/v1/systemone` with the API key set on the block, like any other provider.

## 5. Next step

Get a TypeSafe API key from https://console.typesafe.ai/keys. With it, build the `kb2itpieapi` side-by-side comparison on the local Sim copy first: one agent block with `jev-latest` and a single Choice question listing the 12 endpoints.

## Sources

- TypeSafe docs — Introduction: https://docs.typesafe.ai/introduction
- TypeSafe docs — Quick start: https://docs.typesafe.ai/introduction/quickstart.md
- TypeSafe docs — Jev with coding agents: https://docs.typesafe.ai/introduction/coding-agents.md
- TypeSafe docs — Agent skill: https://docs.typesafe.ai/agent-skill.md
- TypeSafe docs index: https://docs.typesafe.ai/llms.txt
- InfoQ — TypeSafe AI Releases Jev: https://www.infoq.com/news/2026/10/typesafe-ai-jev-released/
- Tom's Hardware — TypeSafe AI's Jev: https://www.tomshardware.com/tech-industry/artificial-intelligence/typesafe-ais-jev-offers-an-alternative-to-llms-that-claims-to-be-193x-faster-and-445x-cheaper-system-one-type-model-is-bespoke-for-probabilistic-decision-making
- DataCamp — Jev explained: https://www.datacamp.com/blog/system-one-models-jev
- Sim agent-block Jev support: read directly from the Sim application code (provider `typesafe`), 6 October 2026.