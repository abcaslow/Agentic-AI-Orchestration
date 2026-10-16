# Agentic AI Orchestration with the Sim Mothership Platform

## Part 03 — Hands-On Student Labs

**Course:** Agentic AI Orchestration with the Sim Mothership Platform
**Audience:** Broad — no coding required for Track A; some scripting comfort helps for Track B.
**Format:** Every lab has **two tracks**. Do the one that matches your comfort level (or do both).

- **Track A — No-Code:** build with the visual workflow builder and the chat/agent UI.
- **Track B — Code Sandbox:** build with the code sandbox, custom tools, and custom model configs.

---

> ## ⚠️ SAFETY &amp; COST REMINDER — READ BEFORE EVERY LAB
>
> - **Every lab has a hard credit cap.** Do not exceed it. If you hit the cap before finishing, stop and ask the instructor.
> - **Use cheap models for everything** except Lab 5. Default to a **Haiku / Flash / mini tier** model (e.g. `claude-haiku-4-5`, `gemini-3.5-flash`, `gpt-5-nano`). These cost a fraction of premium models.
> - **Never connect your real personal inbox, bank, or private accounts.** Labs use safe/test actions and instructor-provided sandbox data only.
> - **Never paste real passwords, API keys, or secrets into a prompt.** Use the workspace environment-variable store, referenced by name (e.g. `{{MY_KEY}}`).
> - **Turn off / pause anything scheduled** at the end of a lab so it does not keep running (and keep costing credits) overnight.
> - Full budget rules, per-student caps, and the model price tiers are in **`04-cost-control-plan.md`**. Read it once at the start of the course.

---

### How to use this document

Each lab is self-contained and copy-pasteable. Work top to bottom. A lab is finished when you pass the **"You're done when…"** checkpoint. Submit the deliverable named in the rubric. Stretch goals are optional and count as bonus.

| Lab | Module | Focus                          | Est. time | Credit cap |
| --- | ------ | ------------------------------ | --------- | ---------- |
| 1   | M1     | Explore &amp; map the platform | 30 min    | \~$0       |
| 2   | M2     | Build your first agent         | 45 min    | $0.15      |
| 3   | M3     | Give the agent a tool          | 60 min    | $0.25      |
| 4   | M4     | Scheduled durable workflow     | 60 min    | $0.30      |
| 5   | M5     | Multi-model comparison         | 60 min    | $1.00      |
| 6   | M6     | Knowledge base + RAG           | 60 min    | $0.30      |
| 7   | M7     | Deploy &amp; schedule          | 60 min    | $0.30      |
| 8   | M8     | Capstone                       | 3–5 hrs   | $3.00      |

---

## LAB 1 — Explore the Workspace &amp; Map the Platform

**Module:** M1 — What is agentic orchestration?
**Estimated time:** 30 min · **Credit cap:** \~$0 (observation only — no model runs)
**Prerequisites:** A Sim account and access to the class workspace.

**Goal:** Learn to *see* the architecture — orchestrator, subagents, tools, integrations, workflows, tables, knowledge bases, and scheduled jobs — before you build anything.

### Track A — No-Code

1. Log in and open the workspace. Find the left-hand navigation: **Workflows**, **Knowledge Bases**, **Tables**, **Files**, and **Jobs/Scheduled tasks**.
2. Open any deployed workflow (e.g. a "tracker" workflow). Note its **blocks** and the **arrows** (connections) between them — this is orchestration made visual.
3. Open a **scheduled job** and read its configuration panel: prompt, cron schedule, run count, last run. Notice the panel is a *live view*, not a file you edited.
4. Open the **Files** area and find one real saved document. Contrast it with the job config view you just saw.
5. On paper or in a doc, draw 7 boxes and label them: Orchestrator, VFS, Subagents, Tools, Integration Gateway, Scheduled Jobs, Persistence/Credentials. Draw an arrow from Orchestrator to each.

### Track B — Code Sandbox

1. Do steps 1–4 above.
2. Open the **code sandbox**. Run a one-line script that prints "hello" to confirm the sandbox works.
3. List the workspace tables and note their IDs and schemas (fields). Identify which workflow writes to each table.
4. Identify one workflow that uses a **custom tool** or **code block**. Read its code and describe in one sentence what it does.
5. Produce the same 7-box map as Track A, but annotate each box with a **real example from this workspace** (a specific workflow, table, or job).

**✅ You're done when…** you can point to a concrete example in the workspace for all 7 architecture components and explain, in plain language, how the orchestrator delegates work.

**Stretch goal:** Find a workflow that both reads AND writes a table, and explain the data loop.

**Grading rubric (10 pts):** Map complete with all 7 components (4) · each mapped to a real workspace example (3) · correct explanation of orchestrator→subagent delegation (3).

---

## LAB 2 — Build Your First Single Agent

**Module:** M2 — Build your first agent
**Estimated time:** 45 min · **Credit cap:** $0.15 · **Model:** cheap tier only (`claude-haiku-4-5`, `gemini-3.5-flash`, or `gpt-5-nano`)
**Prerequisites:** Lab 1.

**Goal:** Create a working single-agent that takes an input and returns a useful, structured response.

### Track A — No-Code

1. Create a new workflow. Add a **Start** block and an **Agent** block; connect Start → Agent.
2. In the Agent block, set **Model** to a cheap-tier model. Leave temperature at its default (\~0.3).
3. Write a **system prompt**: e.g. *"You are a concise study assistant. Summarize the user's text into exactly 3 bullet points."*
4. Run the workflow with a short sample paragraph as input. Confirm you get 3 bullets.
5. Add a **Response Format** (JSON schema) requiring a field `bullets` (array of strings). Re-run and confirm structured output.

### Track B — Code Sandbox

1. Create a new workflow with Start → Agent as above, cheap-tier model.
2. Instead of the visual response format, define the JSON schema yourself in the Response Format field: an object with `summary` (string) and `bullets` (array).
3. Add a downstream **code/function block** that reads `<agent.bullets>` and returns their count.
4. Run and verify the count matches the number of bullets.
5. Change the model to a *second* cheap-tier provider and re-run the same input. Note any difference in output style.

**✅ You're done when…** the agent returns valid structured output (parseable JSON with the required fields) on a sample input, under the $0.15 cap.

**Stretch goal:** Add a second input field (e.g. "tone") and make the agent adapt its summary tone accordingly.

**Grading rubric (10 pts):** Agent runs successfully (3) · uses a cheap-tier model as required (2) · returns valid structured output (3) · stayed under credit cap (2).

---

## LAB 3 — Give Your Agent a Tool (Make It *Do* Something)

**Module:** M3 — Tools &amp; integrations
**Estimated time:** 60 min · **Credit cap:** $0.25 · **Model:** cheap tier only
**Prerequisites:** Lab 2.

**Goal:** Move from an agent that *talks* to an agent that *acts* — by adding a tool. We use a **safe/test action only**: web search, a scratch table, or a class-provided sandbox integration. **Do NOT connect your real inbox or any private account.**

### Track A — No-Code

1. Open your Lab 2 workflow (or clone it). Keep the cheap-tier model.
2. In the Agent block, open the **Tools** section and add a safe tool — e.g. **web search** (read-only) or a **Table write** to a scratch table the instructor created.
3. Update the system prompt so the agent knows when to use the tool: *"When asked a factual question, use web search, then answer with a one-line citation."*
4. Run with a question like *"What is the capital of Australia?"* and confirm the tool was called (check the tool-call trace in the run view).
5. If using a scratch table, verify a new row appeared with the agent's output.

### Track B — Code Sandbox

1. Clone your Lab 2 workflow.
2. Write a **custom tool** (a small function block) that performs a safe local computation — e.g. takes a list of numbers and returns min/max/mean — and register it as a tool the agent can call.
3. Instruct the agent to use your custom tool for any math request instead of doing arithmetic itself.
4. Run with *"Give me the stats for 4, 8, 15, 16, 23, 42"* and confirm the agent invoked your tool (inspect the `toolCalls` output).
5. Add basic error handling: what does the tool return on empty input? Test it.

**✅ You're done when…** the run trace shows the agent actually invoked the tool and used its result in the final answer — not just answering from memory.

**Stretch goal:** Add a *second* tool and write a prompt that makes the agent choose correctly between them based on the request.

**Grading rubric (10 pts):** Tool registered correctly (3) · agent invokes it appropriately (3) · result used in final answer (2) · safe/test action only, no private accounts (2).

---

## LAB 4 — Turn an Agent into a Scheduled Durable Workflow

**Module:** M4 — Workflows vs. agents (durable automation)
**Estimated time:** 60 min · **Credit cap:** $0.30 · **Model:** cheap tier only
**Prerequisites:** Lab 3.

**Goal:** Build a **scheduled summarizer** — a simpler cousin of the instructor's "6am Gmail-check" job — that runs on a schedule, produces output, and appends it to a log file. Understand the difference between a one-off agent chat and a *durable, self-running* workflow.

> **Model reference:** The class "check my gmail account every morning at 6am" job runs on a cron schedule, checks a source, and appends a dated entry to a log file every run. You will build the same *shape* with a safe source (an RSS feed, a scratch table, or a fixed text input) — **not** a real inbox.

### Track A — No-Code

1. Create a new workflow. Add a **Schedule** trigger. Set it to run **every 10 minutes** for testing (you will change it later).
2. Add an Agent block (cheap model) that summarizes a safe input (e.g. a public RSS feed via web-fetch, or a fixed paragraph) into 2–3 bullets.
3. Add a **File append** (or Table write) step that writes a **dated entry** to a log file, e.g. `files/lab4-<yourname>-log.md`.
4. Save and let it run **twice**. Confirm two dated entries appear (appended, not overwritten).
5. **Change the schedule to daily**, then **pause the job** so it does not keep running. (This is the cost-safety habit.)

### Track B — Code Sandbox

1. Build the same Schedule → Agent → append pipeline, but write the append step as a **code block** that formats a Markdown heading with an ISO timestamp.
2. Make the summary **structured** (JSON) and have the code block render it into a clean Markdown table row.
3. Add a guard: if the source returns nothing new, write "No new items" instead of an empty entry.
4. Run twice; confirm idempotent, non-overwriting appends with correct timestamps.
5. Change to daily and **pause** the job.

**✅ You're done when…** your log file has at least two correctly-dated, appended entries AND you have paused the schedule so it stops consuming credits.

**Stretch goal:** Add a conditional that only appends when the summary differs from the previous run (dedupe).

**Grading rubric (10 pts):** Schedule trigger works (2) · agent produces a useful summary (2) · appends dated entries without overwriting (3) · job paused at end (2) · under cap (1).