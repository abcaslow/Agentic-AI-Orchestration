# Sim Aggregate Workflow Block Frequency Analysis

Session summary, 2026-10-13. Scope: hosted sim.ai workspace 19e4fb7d-7008-4b24-8217-5c0f83d3b0c0.
Method: listed all workflows through the v1 API, exported each one, and counted blocks by type.

## Totals
- 49 workflows, 389 blocks, 47 distinct block types.

## Top 10 block types
| Rank | Block type | Blocks | Share | Workflows using it |
|---|---|---|---|---|
| 1 | function | 130 | 33.4% | 42 |
| 2 | start_trigger | 39 | 10.0% | 39 |
| 3 | agent | 35 | 9.0% | 29 |
| 4 | response | 24 | 6.2% | 19 |
| 5 | table | 23 | 5.9% | 16 |
| 6 | ssh | 18 | 4.6% | 15 |
| 7 | condition | 17 | 4.4% | 11 |
| 8 | api | 14 | 3.6% | 10 |
| 9 | schedule | 9 | 2.3% | 8 (3 disabled) |
| 10 | note | 9 | 2.3% | 9 |
| | Top 10 total | 318 | 81.7% | |

Next most common: table_v2 (8), loop / knowledge / gmail_v2 (5 each), memory / hubspot (4 each), file_v5 (3).
Twenty-four types appear exactly once.

## Agent blocks: 35 blocks in 29 workflows, all enabled
Models: claude-sonnet-5 (11), gpt-5.4 (5), claude-sonnet-4-6 (4), gpt-5.5 (2), gemini-3.5-flash (2),
gemini-3.5-flash-lite (2), gemini-3.8-flash (2), jev-latest (2), claude-sonnet-5-5 (1),
claude-haiku-4-5 (1), gpt-4o (1), jev-preview (1), openrouter nemotron-3-nano free (1).
By provider: Anthropic 17, OpenAI 8, Google 6, Jev 3, OpenRouter 1.

Tools are attached to only 8 of the 35 agent blocks (12 tools): Exa search 6, Exa get-contents 4,
Knowledge Search 1, LangSmith 1. All are set to auto.
Workflows with tools: demo workflow, demo-for-chris, most-basic-workflow, openrouter-workflow,
research stock prices, snd-aao-self-assessment, student-bio-research.

## Workflows with no agent block: 20 of 49
collaborate-close-tabs, collaborate-meeting-log, competitor-pricing-watcher, Concur Receipt Validation,
default-agent, google drive to youtube channel, netmiko-device-cmds-on-max, pandas function demo,
publish to smartnewdeal, s3-invoice-textract-intake, scp-from-aws, sim credit burn tracker,
sim product comparison, sim spend monitor, snd-page-read-claude, snd-page-write-claude,
ssh-to-collaborate-simmeter, warm-up-collaborate-desktops, warm-up-desktops-with-url, whoop tracker.
Two still use AI without an agent block: Concur Receipt Validation (evaluator) and
competitor-pricing-watcher (browser_use). Never run: default-agent, competitor-pricing-watcher,
google drive to youtube channel, s3-invoice-textract-intake.

## Findings
- Function blocks do most of the work; agents are used mainly for the language step.
- The four ssh-to-* workflows all use gpt-5.4; nl-ssh-dispatcher uses claude-haiku-4-5.
- Four agent blocks still run claude-sonnet-4-6 and are candidates for a model refresh.
- The profile agent in snd-aao-self-assessment has LangSmith attached as a tool; other workflows log from a separate block.
- buildTelemetry in netprog-qa-smartnewdeal-kb has an unwired error handle, so an error there fails the run.

## Limits
Covers only the one workspace the API key can see. Tools attached to agent blocks are not counted as blocks.
