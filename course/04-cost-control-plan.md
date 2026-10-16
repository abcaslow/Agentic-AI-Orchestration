# Cost-Control &amp; Credit-Budget Plan

### Agentic AI Orchestration with the Sim Mothership Platform — Classroom Policy

**Audience:** a broad-range cohort of \~25 students (mixed technical backgrounds)
**Course length:** 8 weeks
**Purpose:** keep the class educational and hands-on while preventing runaway credit/dollar spend.

---

## 1. The Core Risk — Why This Plan Exists

Agentic AI is *pay-per-use*, and the meter runs on every model call — including the ones an agent makes to itself while looping, retrying, and calling tools. A single agent that "just checks something once a day" is not free.

**Real data from this workspace.** The scheduled task *"check my gmail account every morning at 6am"* is one agent doing one small job per day. Its retained per-run costs:

| Date        | Cost (USD)        |
| ----------- | ----------------- |
| 2026-07-15  | $0.188069         |
| 2026-07-16  | $0.212624         |
| 2026-07-17  | $0.595549         |
| 2026-07-18  | $0.191988         |
| 2026-07-19  | $0.208222         |
| **Average** | **\~$0.28 / run** |

Note the spread: a "normal" run is \~$0.19, but one run hit **$0.60 — 3x the baseline** — simply because that day had more email to reason over. Agent cost is *variable and input-dependent*; you cannot assume the average.

**Now scale it to a classroom.** One student running one agent a handful of times per lab is fine. But **25 students × multiple agents × iterative debugging × "let me just run it again"** compounds fast:

- 25 students × 20 agent runs in a single lab × ~~$0.28 avg = \*\*~~$140 in one afternoon\*\*.
- One student who leaves a loop or an aggressive schedule running unattended can *alone* out-spend the rest of the class.

The rest of this document is the guardrail system that keeps that from happening.

---

## 2. Workspace Model — Shared vs. Individual Accounts

| Model | Pros | Cons |
|-------|------|------|
| **Single shared workspace** (all 25 students in one) | One billing pool; instructor sees everything in one place; easy to seed starter workflows/tables | Students can see/edit each other's work; one runaway agent hurts everyone; hard to attribute spend to a person |
| **Individual accounts/workspaces** (free/low tier each) | Clean isolation; per-student spend caps enforced by the tier itself; a runaway loop only burns *that* student's credits | Harder to monitor centrally; more setup; feature limits on free tiers may block some labs |
| **Hybrid (recommended)** | Individual student workspaces for daily labs + one shared "class demo" workspace the instructor owns for walkthroughs and the capstone showcase | Slightly more admin, but best isolation + best teaching surface |

**Recommendation for a class of 25:** **Hybrid** — each student works in their **own workspace on a capped/low tier** (so a runaway agent can only spend that student's allotment, not the class pool), plus **one instructor-owned shared demo workspace** for live walkthroughs and starter templates. This is the single most effective structural control: isolation caps blast radius *by design*, before any policy is even needed.

---

## 3. Per-Student Budget — 8-Week Course

Anchored to observed cost: a small agent run averages **~$0.28** and can spike to **~$0.60**. Routine labs on cheap models (see §4) run **far** below this — typically **$0.01–$0.05 per run**. Budget for the cheap default, with headroom.

**Assumptions per student, per week:** ~40–60 agent runs across practice + one graded lab, mostly on cheap models.

| Line item | Per run | Runs/wk | Weekly | 8-week |
|-----------|---------|---------|--------|--------|
| Routine labs (cheap models) | ~$0.03 | 50 | $1.50 | $12.00 |
| Multi-model comparison lab (premium, Week 5 only) | ~$0.30 | 10 (one week) | — | $3.00 |
| Debugging / re-runs buffer | — | — | — | $5.00 |
| **Per-student subtotal** | | | | **~$20.00** |

**Per-student pool: $25** (includes a 25% safety margin).
**Per-lab hard cap: $3** per student per weekly lab — if a student hits it, the lab pauses and the instructor reviews before more spend.
**Class pool (25 students): $25 × 25 = $625**, plus a **$125 instructor/demo + contingency reserve** = **~$750 total** for the 8-week course.


---

## 4. Model-Tier Policy — Cheap by Default, Premium by Exception

The biggest single lever on cost is **which model each agent uses**. Policy:

### Default tier (use for ALL routine labs, Weeks 1–4, 6–8)
Sim-hosted **managed** models — **no student API keys required**, low per-token cost, plenty capable for teaching orchestration concepts:

- **Anthropic Claude Haiku 4.5** (`claude-haiku-4-5`) — speed-optimized, cheap
- **Google Gemini 3.5 Flash / 3.1 Flash-Lite** (`gemini-3.5-flash`, `gemini-3.1-flash-lite`) — cheapest tier
- **OpenAI mini/nano** (`gpt-5-mini`, `gpt-5-nano`, `gpt-5.4-mini`, `gpt-5.4-nano`)

> **Rule:** every lab template ships pre-set to a default-tier model. Students do not change the model unless the lab explicitly says so.

### Premium tier (RESERVED — Week 5 multi-model comparison lab ONLY)
- **OpenAI GPT-5.6** (`gpt-5.6-sol`/`terra`/`luna`), **GPT-5.5-pro / GPT-5-pro**
- **Anthropic Claude Sonnet 5 / Opus 4.8–4.5**
- **Google Gemini 3.1 Pro** (`gemini-3.1-pro-preview`)

> **Rules for the premium lab:**
> - Each student makes **one controlled comparison run per model** (≈3–4 runs total), not open-ended experimentation.
> - **Per-run cap: $0.50** (the observed ceiling of the Gmail task). If a run would exceed it, it stops.
> - Reasoning-heavy settings (high `reasoningEffort` / `thinkingLevel: max`) are **off** unless the lab is specifically about reasoning cost — those multiply token spend several-fold.
> - No premium model may be attached to a *scheduled* or *looping* agent, ever.

---

## 5. Integration & Credential Safety

Cost isn't the only risk — real credentials on student agents are a privacy and security hazard too.

- **Prefer Sim-hosted managed models (no keys).** The default tier requires zero student API keys — this is the safest and simplest path for a broad cohort.
- **No personal accounts.** Students must **not** connect their personal Gmail, Slack, bank, or work accounts to a class agent. The instructor's live Gmail-check task is a *demo the instructor runs*, not a student exercise.
- **Use test/sandbox actions.** For "agent that does something" labs, use safe targets: a shared throwaway/test inbox, a sandbox Slack workspace, mock webhook endpoints, or read-only public APIs — never a production system.
- **Bring-your-own-key providers are opt-in and instructor-approved only.** If an advanced student wants to try xAI/DeepSeek/OpenRouter/etc., they use *their own* key on *their own* budget, with the instructor aware.
- **Never paste secrets into prompts or shared files.** Keys live in environment variables / the credential store, referenced by name — never typed into an agent's message body or a workspace doc.


---

## 6. Loop & Runaway Prevention

Runaway agents are the biggest source of surprise cost. Hard controls:

- **Iteration caps.** Every agent/workflow has a max-iteration (max tool-call/loop) limit. Set a class default of **≤5–8 iterations** per run for labs. No unbounded "keep going until done" agents.
- **Schedule frequency limits.** If a lab uses a scheduled trigger, the *minimum* interval is **daily** (not hourly, not every-5-minutes). Students demonstrate scheduling with a single run or a 1x/day cron, then **disable it** at end of lab.
- **No unattended infinite schedules.** No scheduled or looping agent may be left enabled past the end of a class session. End-of-lab checklist: **pause/disable every schedule you created.** (The instructor's own Gmail task is a cautionary example — it quietly ran 17 times before being paused.)
- **No premium model on any loop/schedule.** Loops + expensive models is the worst-case cost multiplier — banned.
- **Cancel runaway runs.** Teach students to recognize and **cancel** a run that's iterating without converging, and to tell the instructor. Cancelling early is always correct.
- **Timeouts.** Where available, set a per-run wall-clock timeout so a stuck agent self-terminates.

---

## 7. Instructor Monitoring Checklist

**Weekly (every week of the course):**
- [ ] Review **spend per student** for the week; flag anyone above ~$3.
- [ ] Confirm no student is above the **$25 per-student pool** trajectory (should be ~$2.50/wk).
- [ ] Scan for **premium models used outside Week 5** — investigate any.
- [ ] Check for **enabled schedules** left running from prior labs; disable stragglers.
- [ ] Look for **stuck/looping runs** and unusually long or expensive individual runs.
- [ ] Verify **no personal credentials** (Gmail/Slack/etc.) got connected to student agents.

**Before each lab:**
- [ ] Confirm lab template is pinned to a **default-tier model**.
- [ ] Remind students of the **per-lab $3 cap** and end-of-lab **disable-your-schedules** step.

**End of course:**
- [ ] Confirm **all student schedules are disabled**.
- [ ] Reconcile total spend against the **$750 budget** and note variance for next cohort.

---

## 8. Estimated Total Course Budget

| Category | Basis | Estimate |
|----------|-------|----------|
| Routine labs — 25 students × cheap models | 25 × $12.00 | $300.00 |
| Multi-model comparison lab (Week 5) | 25 × $3.00 | $75.00 |
| Debugging / re-run buffer | 25 × $5.00 | $125.00 |
| **Student subtotal** | | **$500.00** |
| Instructor demos + starter templates | shared workspace | $100.00 |
| Contingency reserve (~20%) | | $150.00 |
| **Grand total (8-week, 25 students)** | | **~$750.00** |
| **Per-student effective cost** | $750 ÷ 25 | **~$30.00** |

**Bottom line:** with the Hybrid workspace model, a cheap-by-default model policy, hard iteration/schedule caps, and weekly spend monitoring, a broad-cohort 8-week course of 25 students can run comfortably on a **~$750 total budget (~$30/student)** — while a single unmanaged runaway agent could otherwise eat a meaningful chunk of that in an afternoon.

---
*Grounded in observed workspace data: the "check my gmail account every morning at 6am" scheduled task (avg ~$0.28/run, range $0.19–$0.60 across 5 retained runs, 2026-07-15 → 2026-07-19). Model tiers reflect the Sim Agent-block catalog as of 2026-07-19.*
