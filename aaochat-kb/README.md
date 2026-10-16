# aaochat Knowledge Base — Agentic AI Orchestration (AAO)

Source documents for **aaochat**, a [Sim](https://sim.ai) knowledge base used for retrieval-augmented generation (RAG) about
open-source Agentic AI Orchestration: core AI terminology, Sim workflow building blocks, the Jev decision model,
combining RAG with LLMs, post-training methods, ontologies and related course notes.

Exported from Sim on 2026-10-15. **31 documents, about 6.7 MB** (the PDF is 6.5 MB; everything else is about 140 KB of text).

## Contents

```
documents/
  1 Definition of Terms.pdf                              AAO Definition of Terms (the main reference)
  combining-jev-llm-rag-notes-from-sf-oct-10.md
  sim-aggregate-workflow-block-frequency-analysis.md
  sim-jev-notes-9-oct-in-sf.md
  emails/                                                27 short notes, one per email thread
```

| File | Original title |
|---|---|
| `documents/emails/a-comparison-of-sim-workflows-to-jupyter-notebooks.md` | a comparison of sim workflows to jupyter notebooks |
| `documents/emails/bash-as-an-agentic-ai-tool.md` | bash as an agentic ai tool |
| `documents/emails/benefits-of-hosting-locally.md` | benefits of hosting locally |
| `documents/emails/bluehost-review-of-sim.md` | Bluehost review of Sim |
| `documents/emails/competing-jev-models.md` | competing jev models |
| `documents/emails/deploying-jev-and-llama-in-the-same-workflow.md` | deploying jev and llama in the same workflow |
| `documents/emails/deploying-rag-jev-and-llama-in-the-same-workflow.md` | deploying rag, Jev and llama in the same workflow |
| `documents/emails/details-on-the-sim-function-block.md` | details on the sim function block |
| `documents/emails/fortune-mag-on-jev.md` | fortune mag on jev |
| `documents/emails/instinct-ai-harness.md` | instinct ai harness |
| `documents/emails/javascript-cheat-sheet-for-sim.md` | Javascript cheat sheet for sim |
| `documents/emails/javascript-notes-for-the-sim-function-workflow-block.md` | javascript notes for the sim function workflow block |
| `documents/emails/knowledge-base-ingestion-post-training-paradigms-rlhf-rlvr-rlcd.md` | Knowledge Base Ingestion: Post-Training Paradigms (RLHF, RLVR, RLCD) |
| `documents/emails/knowledge-base-socratic-architecture-pattern-in-hybrid-ai-stacks.md` | Knowledge Base: Socratic Architecture Pattern in Hybrid AI Stacks → |
| `documents/emails/ontologies.md` | Ontologies |
| `documents/emails/rag-notes.md` | RAG Notes |
| `documents/emails/rationale-for-our-aao-course-and-diogo-interview.md` | rationale for our AAO course and Diogo interview |
| `documents/emails/recommendations-for-deploying-jev-with-sim-ai-workflows.md` | recommendations for deploying jev with sim.ai workflows |
| `documents/emails/recommended-sim-workflows-to-start-with.md` | recommended sim workflows to start with |
| `documents/emails/sim-loops-custom-blocks-and-quick-reference.md` | sim loops custom blocks and quick reference |
| `documents/emails/sim-modular-workflow-building-blocks.md` | Sim modular workflow building blocks |
| `documents/emails/snd-blog-post-on-future-of-work-with-nyu-professor.md` | snd blog post on future of work with nyu professor |
| `documents/emails/the-cost-statement-in-javascript.md` | The cost statement in javascript |
| `documents/emails/the-origin-of-the-name-jev.md` | the origin of the name jev |
| `documents/emails/the-sim-embedding-block.md` | The sim embedding block |
| `documents/emails/topaz-agents-in-2026.md` | topaz agents in 2026 |
| `documents/emails/vector-store-data-for-rag.md` | Vector store data for RAG |

The `emails/` notes were synced into the knowledge base from Gmail. Each file is the indexed text of one email thread
and begins with its Subject / From / To header lines, followed by each message with its sender and date.

## Load it into your own Sim workspace

1. Download or clone this repository.
2. In Sim, open **Knowledge** and create a new knowledge base (for example `aaochat`).
   Settings used for the original: embedding model `text-embedding-3-small`, max chunk size 1024,
   min chunk size 100, overlap 200. The defaults work fine too.
3. Upload every file in `documents/` and `documents/emails/`. Sim chunks and embeds them in your account.
4. Wait until every document shows as processed, then try a search such as
   *"Who coined the term Artificial Intelligence?"*.

### Use it in a chat workflow

A minimal RAG chat in Sim is: **Start** (a question input) → **Knowledge** block (operation *Search*, pointed at your
knowledge base, query = the question) → **Agent** block whose prompt includes the question and the Knowledge block's
results, with instructions to answer only from those excerpts and cite the source document names.

## License / reuse

Shared for personal and educational use by Sim users. Some material quotes or summarizes third-party sources
(for example Wikipedia and news articles); those sources keep their own rights.
