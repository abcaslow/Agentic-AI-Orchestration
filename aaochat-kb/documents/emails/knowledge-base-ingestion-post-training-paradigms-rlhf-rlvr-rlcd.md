Subject: Knowledge Base Ingestion: Post-Training Paradigms (RLHF, RLVR, RLCD)
From: Unitedwithcode <unitedwithcode@gmail.com>
To: Unitedwithcode <unitedwithcode@gmail.com>
Messages: 1

--- Unitedwithcode <unitedwithcode@gmail.com> (Thu, 15 Oct 2026 08:32:08 -0400) ---
# AI Post-Training Paradigms and Decision Models: Comprehensive Reference

## 1. RLHF vs. RLVR: Core Paradigms
RLHF (Reinforcement Learning from Human Feedback) and RLVR (Reinforcement
Learning with Verifiable Rewards) are two distinct post-training paradigms
used to align and improve Large Language Models (LLMs).

### RLHF (Reinforcement Learning from Human Feedback)
* **Source of Reward:** Relies on subjective human preferences ("Does this
feel right?", tone, politeness, and helpfulness).
* **Mechanism:** Humans rate or rank model outputs, which is used to train
a separate reward model. The LLM is then optimized against this learned
reward model (traditionally via PPO).
* **Best Used For:** Conversational flow, general instruction following,
tone calibration, and safety alignment (making models polite, empathetic,
and safe).
* **Limitations:** Slow, expensive, prone to human bias, and susceptible to
"reward hacking" where the model learns to sound confident or polite rather
than being factually correct.

### RLVR (Reinforcement Learning with Verifiable Rewards)
* **Source of Reward:** Relies on objective, deterministic, rule-based
verification ("Does this math answer match?" or "Does this code pass unit
tests?").
* **Mechanism:** Replaces the human/learned reward model with an automated
verifier (like a Python interpreter, code compiler, or math engine) that
issues a binary reward (1 for correct, 0 for wrong).
* **Best Used For:** Complex logic, mathematical reasoning, and coding
tasks (such as models like OpenAI o1 or DeepSeek-R1).
* **Advantages:** Enables deep deliberation (System 2 thinking), allows
models to explore multiple Chain-of-Thought reasoning paths freely, and
removes the human bottleneck.
* **Limitations:** Only works well on tasks with clear ground-truth or
objective checkability; cannot easily evaluate subjective open-ended
creative writing.

### Key Comparison Matrix
| Feature | RLHF | RLVR |
| :--- | :--- | :--- |
| **Reward Signal** | Subjective (human/AI preference) | Objective
(deterministic code/math check) |
| **Primary Goal** | Helpfulness, safety, and conversational alignment |
Logical accuracy, math, and code execution |
| **Scalability** | Limited by human labor and speed | High scale via
automated programmatic verifiers |
| **Model Examples** | Standard instruction-tuned LLMs | Reasoning models
like DeepSeek-R1 and OpenAI o1 | ## 2. RLCD (Reinforcement Learning for Calibrated Decisions)

### Overview and Definition
Jev uses Reinforcement Learning for Calibrated Decisions (RLCD) instead of
RLHF. RLCD is a post-training machine learning method where an AI model is
rewarded based on how well its stated probability matches actual real-world
outcomes (evaluated via scoring rules like the Brier score), rather than
trying to optimize for human conversational preference or binary test
verification. For example, if the model predicts an event with 80%
confidence, RLCD rewards it only if that event actually happens about 80%
of the time.

Reinforcement Learning for Calibrated Decisions (RLCD) is the reinforcement
learning post-training objective that TypeSafe AI says it used to train
Jev, the model it released on 15 September 2026 and describes as the first
"System One model." Instead of rewarding a model for producing an answer a
human rater prefers, RLCD rewards the model for attaching probabilities
that are honest: a decision returned at 0.8 should be right about 80% of
the time across many such decisions.

TypeSafe's documentation frames it as training the model "to return
decisions and calibrated probabilities instead of generated text." Its
launch post describes the target as "answers with epistemically honest
probabilities on System One tasks."

### When and Where It Is Used
* **Automated Software Execution & Workflows:** Used when AI makes
structured, machine-consumed choices (such as API routing, fraud detection,
intent classification, or automated decision-making) rather than generating
conversational paragraphs.
* **High-Stakes Decision Support:** Used when downstream software needs a
reliable, honest estimate of uncertainty alongside a choice—ensuring the
model does not sound falsely confident when it is actually guessing.
* **Alternative to RLHF:** Introduced in September 2026 by TypeSafe AI for
its Jev model as an alternative to Reinforcement Learning from Human
Feedback (RLHF) and Reinforcement Learning with Verifiable Rewards (RLVR).
Note that TypeSafe says RLHF was co-invented by its cofounder Diogo Almeida.

### Important Cautions and Boundaries
* **Vendor-Coined Term:** RLCD is a vendor-coined method name, not an
industry standard. There is no paper, no published reward function, no
dataset description, and no released calibration figure. Everything known
about RLCD comes from TypeSafe's own launch materials and has not been
independently reproduced.
* **What RLCD Does Not Do:** RLCD does not make a model more accurate, and
it is not what prevents a model like Jev from returning off-schema output.
Accuracy is how often the model is right; calibration is whether its
confidence tracks its accuracy, and the two are independent properties.
* **Schema Validity:** The guarantee that the output is always schema-valid
comes from the architecture, not from RLCD. The output space is constrained
in advance to valid values, so a type error is structurally impossible.
* **Scoring Implementations:** An independent reimplementation on GitHub
(`eve-rlcd`) uses a reward proportional to the gradient of the Brier
score—somebody else's guess at a plausible formulation, not an official
disclosure.
* **Naming Details:** TypeSafe writes it as Reinforcement Learning "for"
Calibrated Decisions, while TechCrunch's 18 September 2026 report quotes
Almeida saying "from." Both spellings are attested. ## 3. Acronym Collision: RLCD vs. Contrastive Distillation
Is RLCD the same as Reinforcement Learning from Contrastive Distillation?
No. RLCD is a genuine acronym collision, and the older claim on those four
letters belongs to Reinforcement Learning from Contrastive Distillation,
published by Kevin Yang, Dan Klein, Asli Celikyilmaz, Nanyun Peng, and
Yuandong Tian at ICLR 2024 (arXiv:2307.12950, first submitted 24 July 2023).

* **Contrastive Distillation Method:** Aligns an LLM to natural-language
principles without human feedback by generating a pair of outputs from
contrasting prompts, using the pair as a synthetic preference label,
training a preference model, and improving the base model with RL. It
produces text and belongs to the RLHF family.
* **TypeSafe's RLCD:** Coined roughly three years later, discards
preference entirely and optimizes probability calibration on typed
decisions. The 2023 paper is by far the better documented of the two.

---

## 4. Content Flow and State Management
RLCD only governs the probability a model attaches to its answer. What that
answer is about is the state you pass in, and a calibrated probability
about the wrong slice of content is still useless. TypeSafe reports a
32,000-token state budget for Jev, so what goes into that window is a
design decision.

Sanity stores content in the Content Lake as structured JSON documents
rather than rendered pages, and a GROQ projection names the fields you want
and returns only those, so you can hand a decision model the specific field
or block a question concerns instead of a whole page of markup and
navigation. Sanity is the AI Content Operating System, and the structured
foundation is what makes a precise state extractable at all.

---

## 5. Vellum by Sanity Labs
Vellum by Sanity (developed by Sanity Labs) is an experimental developer
tool that maps Markdown content directly into structured Sanity CMS
documents.
* **Mechanism:** Unlike many modern translation tools, Vellum intentionally
avoids using an LLM for the heavy lifting. Instead, it uses a code-driven,
type-safe classifier system combined with an internal project called Jev to
handle structural decisions.
* **Key Features:** Regular code handles mechanical and type-safe copying
and document structure validation. The built-in Jev classifier steps in to
answer simple choice and yes/no questions (e.g., determining which schema
field a specific block of text should fill). Anything below your confidence
threshold stays empty for review.
* **Ecosystem:** Written in TypeScript and open-sourced under the MIT
license (`@sanity-labs/vellum`) for local development or via hosted
playground.

---

## 6. The Power of JSON in AI Workflows
The core relationship between Sanity.io, Jev, and RLCD centers around
TypeSafe AI's "System One" decision model and how its training framework
integrates with structured content platforms to power ultra-fast AI
automations.

### Architecture Workflow Loop
1. **[Sanity.io]:** Provides clean, structured JSON data fields via GROQ
projections.
2. **[Jev]:** Analyzes data inputs and processes typed logic questions
within a 32k token state budget.
3. **[RLCD]:** Calibrates the output to ensure a highly accurate,
prose-free decision with reliable confidence intervals (e.g., cutting
documentation assistant response times down to 0.5 seconds).
