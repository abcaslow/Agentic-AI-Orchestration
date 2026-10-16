Subject: recommendations for deploying jev with sim.ai workflows
From: Unitedwithcode <unitedwithcode@gmail.com>
To: Unitedwithcode <unitedwithcode@gmail.com>
Messages: 1

--- Unitedwithcode <unitedwithcode@gmail.com> (Thu, 15 Oct 2026 17:16:22 -0400) ---
# TypeSafe Jev AI Integration & Optimization Guide for Sim.ai

## 1. Overview of Jev AI & Evaluation-States
* **Core Definition:** Jev AI is a non-autoregressive "System One" decision
model and evaluation engine. Rather than writing conversational prose
token-by-token, Jev evaluates an input payload against strict typed
questions, rubrics, and criteria, instantly returning typed decisions with
probability distributions and confidence scores.
* **Evaluation-State (The Core Payload):** The material, context, or data
payload assessed by Jev. Depending on the application, it can be formatted
as:
 * Raw text or strings (customer reviews, chat messages, documents).
 * JSON objects or arrays.
 * Application records or databases.
 * Agent traces and histories (frozen domain policies, conversation
transcripts, tool calls/results, final responses).
* **Core Request Components:** Every Jev request combines three primitives:
 1. **The Evaluation-State:** The data/context being inspected.
 2. **Judging Instructions / Questions:** The deterministic criteria or
questions.
 3. **Allowed Outputs:** Predefined label spaces, choice options, or score
ranges.

---

## 2. Jev AI vs. Generative LLMs (e.g., Claude Sonnet)
Unlike autoregressive LLMs, Jev does not accept free-form conversational
system prompts or behavioral personas.

| Feature | Claude Sonnet (Generative LLM) | Jev (System One Decision
Model) |
| :--- | :--- | :--- |
| **Primary Input** | Conversational System Prompt + User Message | Raw
state (evidence packet / context) |
| **Instruction Layer** | Free-form text instructions telling the model how
to act and reason | Atomic questions paired directly with hardcoded rubrics
|
| **Output Type** | Autoregressive text (token-by-token prose or markdown)
| Non-autoregressive typed decisions (Boolean, choice, or score) with
probabilities |

---

## 3. Deploying Jev AI inside Sim.ai Workflows
Jev is natively supported as an evaluation and structured-decision provider
inside Sim.ai's Agent block architecture.

### Step-by-Step Deployment Pattern
1. **Add the Jev Model:** Open your visual workflow canvas in Sim, add an
**Agent block**, open the **Model selector**, and choose a TypeSafe variant
under the TypeSafe section (`jev-latest`, `jev-1.13.0`, or `jev-preview`).
Supply your TypeSafe API key in environment or block credentials if
self-hosting.
2. **Pass the "State" Input:** Locate the **State** input option inside the
Sim Agent block and map it to inbound raw text, triggers, or JSON
objects/arrays.
3. **Configure Questions (Rubric JSON):** Define your questions and output
spaces using native primitives (`choice`, `score`). Example schema:
 ```json
 {
 "category": {
 "type": "choice",
 "options": ["billing", "technical_support", "sales", "spam"]
 },
 "urgency_score": {
 "type": "score",
 "min": 1,
 "max": 5
 },
 "needs_refund": {
 "type": "choice",
 "options": ["true", "false"]
 }
 }
 ```
4. **Map Outputs to Workflow Routing:** Connect the Jev Agent block output
to a Sim **Router block** or **Switch node** using condition builders
(e.g., `IF steps.jev_agent.output.category == "billing"`).
5. **Publish & Test:** Run a live mock execution using the Play icon, then
deploy as a web-accessible API endpoint or custom MCP Server tool. ## 4. Top Use Cases for Jev + Sim.ai

### Use Case 1: Inbound Lead Triage & Enrichment Guardrails
* **Workflow:** Webhook triggers Sim workflow on form submission; Jev
evaluates the form as state.
* **Primitives:** `is_spam` (Choice: `["true", "false"]`),
`company_size_tier` (Choice: `["enterprise", "mid-market", "smb"]`).
* **Sim Action:** If `is_spam` is true, terminate workflow to save token
costs. If enterprise, pass to enrichment block, update Sim Table, and sync
to Salesforce.

### Use Case 2: Cost-Effective Agent Loop Monitoring & Safeguarding
* **Workflow:** Intercepts multi-step generative agent traces before
executing sensitive tools (Stripe, GitHub).
* **Primitives:** `policy_violation_detected` (Choice: `["yes", "no"]`),
`confidence_score` (Score: `0.0` to `1.0`).
* **Sim Action:** If high-confidence violation is flagged, pivot workflow
away from tool execution and route a Slack warning.

### Use Case 3: High-Volume Support Ticket Routing
* **Workflow:** Zendesk or email ticket lands in Sim; Jev evaluates raw
customer text.
* **Primitives:** `intent` (Choice: `["refund_request", "password_reset",
"bug_report", "general_inquiry"]`), `sentiment_urgency` (Score: `1` to `5`).
* **Sim Action:** Route paths via Router block; automate password resets
via script blocks or open high-urgency bug reports in Jira.

---

## 5. Optimizing Sim.ai RAG Pipelines with Jev AI
Use Jev as an intelligent routing, gating, and pruning engine directly
before and after Sim.ai Knowledge Base calls to eliminate wasted compute
and context token bloat.

### Pattern 1: Pre-Retrieval — Semantic Intent Routing & Vector Skipping
* **Setup:** Place a Jev block at the start of the workflow to evaluate
incoming messages.
* **Rubric Configuration:**
 ```json
 {
 "requires_knowledge_lookup": {
 "type": "choice",
 "options": ["true", "false"]
 },
 "knowledge_domain": {
 "type": "choice",
 "options": ["hr_policies", "technical_api_docs", "sales_pricing",
"none"]
 }
 }
 ```
* **Optimization:** If `requires_knowledge_lookup` is false, bypass the
Knowledge Base entirely. If true, use `knowledge_domain` to dynamically
point the Sim Knowledge Base block to a specific folder or tag, shrinking
search space.

### Pattern 2: Query Rewriting via State Structuring
* **Setup:** Pass chat history into Jev's state to extract atomic search
terms from messy user prompts.
* **Rubric Configuration:**
 ```json
 {
 "primary_search_term": {
 "type": "choice",
 "options": ["password_reset", "mfa_setup", "api_keys",
"sso_provisioning"]
 }
 }
 ```
* **Optimization:** Map the Sim Knowledge Base search query field directly
to Jev's categorical output (`steps.jev_router.output.primary_search_term`)
to match against curated internal document terminology.

### Pattern 3: Post-Retrieval — Reranking & Context Pruning
* **Setup:** Position a Jev block *after* the Sim Knowledge Base block,
feeding returned document chunks as state.
* **Rubric Configuration:**
 ```json
 {
 "chunk_1_relevance": { "type": "choice", "options": ["highly_relevant",
"irrelevant"] },
 "chunk_2_relevance": { "type": "choice", "options": ["highly_relevant",
"irrelevant"] },
 "chunk_3_relevance": { "type": "choice", "options": ["highly_relevant",
"irrelevant"] }
 }
 ```
* **Optimization:** Use a Sim Function (Code) block to strip chunks flagged
as irrelevant before data reaches the final generative LLM block, lowering
latency and token costs.

### Recommended RAG Architecture Sequence
1. **Trigger:** Webhook / Slack message arrives.
2. **Step 1 (Jev Block):** Evaluates if database search is required.
3. **Step 2 (Sim Router):** Branches out based on intent.
4. **Step 3 (Sim Knowledge Base Block):** Targets specific sources using
Jev-extracted domain context.
5. **Step 4 (Jev Block #2):** Discards low-confidence or irrelevant
retrieved chunks.
6. **Step 5 (Claude/GPT Block):** Generates final response using clean,
pruned data.
