# Agentic AI Orchestration with the Sim Mothership Platform

**Instructor:** Unitedwithcode (UnitedwithCode / SmartNewDeal) · DS4HS &amp; ITPIE hands-on training background
**Format:** 8 weeks · one module per week · \~2.5 hours per session (lecture + live demo + lab)
**Delivery:** Cloud-based — students work entirely in the browser on the Sim platform; no local installs required
**Companion materials (same folder):** `02-slide-deck` (intro lecture) · `03-labs.md` (full lab handbook) · `04-cost-control-plan.md` (required cost policy)

---

## Course Description

This course teaches **agentic AI orchestration** — how to design systems where an AI *orchestrator* reasons about a goal, delegates work to specialized *subagents*, calls *tools* and *integrations*, and runs work on a *schedule* — using the Sim mothership platform as a hands-on laboratory.

The guiding philosophy is **concepts-first, platform-as-lab.** You will learn the durable ideas of orchestration (delegation, tool use, workflows vs. agents, retrieval-augmented generation, multi-model routing, scheduling, and deployment) that transfer to *any* agentic platform. Sim is the vehicle we build in because it is cloud-hosted, visual, multi-model, and lets a complete beginner ship a working agent in a single session — while giving advanced students a real code sandbox and custom-tool API.

The course is deliberately built for a **broad range of students.** Every module runs on **two parallel tracks**:

- **Track A — No-Code:** build with the visual workflow builder and the conversational agent. No programming required.
- **Track B — Code:** the same objective, built with the code sandbox, custom tools, and configuration-as-data. Basic scripting recommended.

Students may stay in one track or cross over week to week. Both tracks reach the same learning outcomes.

---

## Target Audience

- **Non-technical professionals** (operations, education, policy, small-business owners) who want to automate real work with AI — Track A.
- **Analysts and "power users"** comfortable with spreadsheets and logic but not full programming — Track A with occasional Track B.
- **Developers, data scientists, and IT/network engineers** who want to build production agentic systems — Track B.
- **Educators and trainers** who want a teachable, reproducible model of modern AI orchestration.

No AI background is assumed. Curiosity and a willingness to experiment are the only hard prerequisites.

---

## Prerequisites

- **Track A (No-Code):** None technical. A web browser and a Sim account.
- **Track B (Code):** Basic scripting familiarity helpful (Python or JavaScript) — enough to read a function and edit variables. Not required to *pass*, only to go deeper.
- **All students:** Complete the Week 0 onboarding (account setup + the cost policy in `04-cost-control-plan.md`) before Module 1.

---

## Learning Outcomes

By the end of this course, students will be able to:

1. **Explain agentic orchestration** — describe the orchestrator → subagents → tools → integrations → schedule model and why it differs from a single chatbot prompt.
2. **Build a working agent** from a plain-language goal, choosing an appropriate model for the task and budget.
3. **Give an agent capabilities** by attaching tools and integrations so it can *act*, not just talk.
4. **Distinguish agents from durable workflows** and decide when a task should be a one-off conversation vs. a reliable, repeatable automation.
5. **Route across multiple AI models** and reason about the trade-offs between cost, speed, and quality.
6. **Ground an agent in private knowledge** using retrieval-augmented generation (RAG) over a knowledge base.
7. **Schedule and deploy** an agent so it runs unattended and produces real output on its own.
8. **Practice responsible AI operations** — control cost, protect credentials, and evaluate agent output critically.

---

## Design Philosophy: Concepts-First, Platform-as-Lab

> **The platform is a moving target — concepts lead.** Sim adds models and features constantly, and any specific button, menu, or model name may change between now and the next cohort. This course is therefore built around the **durable concepts** of agentic orchestration — delegation, tool use, workflows vs. agents, multi-model routing, RAG, scheduling, and deployment. The platform is our laboratory, not the subject. When the UI shifts, the concepts still hold, and students carry them to any agentic system they meet next.

Every module runs on **two tracks** so a broad audience stays challenged:

- **Track A — No-Code:** the visual workflow builder and conversational agent. For non-technical students.
- **Track B — Code:** the code sandbox, custom tools, and configuration-as-data. For developers and analysts who want depth.

Both tracks target identical outcomes; the difference is *how* you build, not *what* you learn.


---

## Course Modules

Each module lists **duration, objectives, key concepts, in-class demo, Track A lab, Track B lab, and assessment.** Full step-by-step lab instructions live in `03-labs.md`; lecture slides for the opening module live in `02-slide-deck`.

### Module 1 — What Is Agentic Orchestration?

- **Duration:** 1 week (1 session)
- **Objectives:** Define agentic orchestration; distinguish it from a single chatbot prompt; read an architecture map.
- **Key concepts:** Orchestrator, subagents, tools, integrations, scheduling, persistence. The mental model: *an orchestrator reasons over a workspace, delegates to subagents, acts through tools and integrations, and runs on schedules.*
- **In-class demo:** Walk the **mothership architecture diagram** (`../mothership-workspace-map.png`) mapped to a live workspace — show a real scheduled task, a real workflow, and a knowledge base as concrete instances of the abstract boxes.
- **Track A lab:** Annotate the architecture diagram — label each component with a real-world example in your own words.
- **Track B lab:** Explore the workspace as a filesystem: locate a workflow definition, a job config, and a knowledge-base record; describe how the pieces connect.
- **Assessment:** One-page "architecture in your own words" write-up + a labeled diagram.

### Module 2 — Build Your First Agent

- **Duration:** 1 week
- **Objectives:** Turn a plain-language goal into a working single agent; choose a model appropriate to the task and budget.
- **Key concepts:** System vs. user prompt; the model as a swappable component; "cheap-model-first" discipline; temperature and output length.
- **In-class demo:** Build a "summarize this text" agent live on a low-cost model (a mini/flash/haiku-tier model), then show the *same* prompt on a premium model and compare.
- **Track A lab:** Create a single agent in the visual builder that answers questions on a topic you choose; run it on a cheap model.
- **Track B lab:** Build the same agent via the agent block / code sandbox; parameterize the model id and swap it without changing the prompt.
- **Assessment:** A working agent + a short reflection on why you chose your model.



### Module 3 — Tools & Integrations (An Agent That *Does* Something)

- **Duration:** 1 week
- **Objectives:** Give an agent capabilities so it acts on the world, not just chats; connect an external service safely.
- **Key concepts:** Tools vs. integrations; the integration gateway; OAuth credentials vs. API keys; least-privilege and test-account discipline.
- **In-class demo:** An agent that reads a data source (web search or a connected read-only account) and produces a structured summary — showing the tool-call trace so students *see* the agent deciding to act.
- **Track A lab:** Add a tool (web search or a safe read-only integration) to your Module 2 agent so it can pull live information and report back.
- **Track B lab:** Define or wire a **custom tool** in the code sandbox; have the agent call it and handle the returned data.
- **Assessment:** An agent that performs one real action end-to-end + a note on the credential/safety choices you made.

### Module 4 — Workflows vs. Agents (Durable Automation)

- **Duration:** 1 week
- **Objectives:** Distinguish a free-form agent from a durable, repeatable workflow; know when to use each.
- **Key concepts:** Determinism vs. autonomy; a *workflow* as a wired graph of blocks; triggers; logging every run; idempotency and "surface only what changed."
- **In-class demo:** Walk a real scheduled task — the **"check my Gmail every morning at 6am"** job — as the canonical example: a recurring agent prompt with a cron trigger that logs every run and surfaces only new/actionable mail. Contrast it with an ad-hoc chat agent doing the same thing once.
- **Track A lab:** Build a small scheduled task (visual) that runs a prompt on a timer and appends its result to a log file each run.
- **Track B lab:** Build the equivalent as a workflow graph (trigger → agent/tool → output block); inspect the run/execution log.
- **Assessment:** A working repeatable automation + a one-paragraph decision rule: *when would you make this an agent vs. a workflow?*



### Module 5 — Multi-Model Lab (Same Task, Different Brains)

- **Duration:** 1 week
- **Objectives:** Route the same task across multiple models; reason about cost vs. speed vs. quality.
- **Key concepts:** Provider-agnostic design; managed vs. bring-your-own-key models; cost-per-run; when a cheap fast model is "good enough" and when a premium model earns its price.
- **In-class demo:** Run one identical prompt across a GPT-tier, a Claude-tier, a Gemini-tier, and a fast/local-style model side by side; compare output quality, latency, and cost per run.
- **Track A lab:** Duplicate your agent three times, assign a different model to each, run the same input, and score the results on a simple rubric (accuracy, tone, cost).
- **Track B lab:** Parameterize the model id and loop the same task across a list of models programmatically; collect cost/latency into a small comparison table.
- **Assessment:** A model-comparison table + a recommendation memo: *which model would you ship, and why?*

### Module 6 — RAG & Knowledge Bases (Grounding an Agent in Private Knowledge)

- **Duration:** 1 week
- **Objectives:** Ground an agent in a private document collection so it answers from *your* sources, not just its training data.
- **Key concepts:** Retrieval-augmented generation (RAG); chunking and embeddings (conceptually); citation and hallucination control; when RAG beats a bigger model.
- **In-class demo:** Query the **SmartNewDeal Site knowledge base** (KB id `5e07a107-45e2-47ea-a4fe-f62e89516771`) — ask an agent about DS4HS training or a blog post and show it citing the crawled pages rather than inventing answers.
- **Track A lab:** Build (or connect to) a small knowledge base from a handful of documents and attach it to an agent so it answers grounded questions with sources.
- **Track B lab:** Query the knowledge base programmatically, inspect the retrieved chunks, and tune how many results feed the prompt; observe the effect on answer quality.
- **Assessment:** A grounded Q&A agent + a short analysis of one answer where retrieval clearly changed the result.

