Subject: Sim modular workflow building blocks
From: Unitedwithcode <unitedwithcode@gmail.com>
To: Unitedwithcode <unitedwithcode@gmail.com>
Messages: 1

--- Unitedwithcode <unitedwithcode@gmail.com> (Wed, 14 Oct 2026 13:52:40 -0400) ---
Most people’s first impression of Sim is that it is a relatively simple
interface that visually creates and displays agentic AI workflows on a
canvas. While it is correct that Sim creates and displays workflows
visually on a canvas, it is not a simple and limited agentic AI workflow
architecture.

The Sim workflow architecture is “block based” and each block is modular,
compartmentalized and containerized

Think of sim workflow blocks as functions in a conventional computer
program.

Given that Sim creates Agentic AI workflows, the most important workflow
blocks are the blocks that call AI Models. At the top of this list is the
Sim Workflow Agent Block followed by other blocks that also call AI Models.

The Critical Probabilistic “AI Reasoning” Blocks

[image: image.png][image: image.png]

[image: image.png][image: image.png]

The Deterministic Block: The Function Block

[image: image.png]

You Have Options: A Probabilistic and a Deterministic Option

[image: image.png][image: image.png]

https://docs.sim.ai/workflows/blocks/router

Options for Deploying Sim’s Native RAG Implementation

[image: image.png][image: image.png]

The Guardrails Block

[image: image.png]

Dynamically Adding Hundreds of Sim Blocks to a Workflow

[image: image.png][image: image.png]

Sim Variables

A variable is a value you set yourself and reuse across a workflow. Sim has
two kinds. Workflow variables hold data during a run, like a counter or a
config object, and you reference them with <variable.name>. Environment
variables hold secrets and configuration, like API keys, and you reference
them with {{KEY}}.

https://docs.sim.ai/workflows/variables

Each Sim workflow block is given a name that is displayed at the top of the
block. Workflow block variables maintain the following format:

<buildReq.result.body>

 <gmailtrigger.email.to>

<gmailtrigger.email.bodyText>

From Agent Block “Answer” in the workflow “netprog-qa-smartnewdeal-kb”

<normalizeinput.result.question>

<buildContext.result.context>

 From Agent Block “Origin Agent in the workflow collaborate-meeting-log-v7

<collectsignals.result.ips>

{{SIM_API_KEY}}

example: a start variable and the conversationid variable in your RAG
workflow deployed on localhost:3000.

At Least Two Ways to Determine Whether a Task Should be Deployed as a Sim
Workflow

Sim is very useful for large organizations deploying agentic AI. Large
organizations will realize two things: (1) not every employee needs to be
running agentic AI sessions from their personal harness and (2) many
agentic AI tasks are repeatable workflows that can be deployed using Sim
workflows. Organizations must identify which of their employees should be
running agentic AI sessions from a personal harness and which workflows
should be deployed as Sim workflows. Not all workflows of an organization
will be deployed as Sim workflow but those that can be should be deployed
as Sim workflows because this will reduce the attack surface of potential
agentic AI rogue activities as well as reduces the blast radius of an
unforeseen agentic AI mishap.

Here are two methods an organization can use to determine what tasks should
be deployed as Sim workflows:

 1.

 Using a tool such as format_sessions.py review your Claude, OpenAI
 agentic AI sessions and determine which sessions need to be converted into
 a Sim workflow.

 2.

 Identify agentic AI workflows that will be used by people who do not
 need to interact with an AI harness and directly initiate an agentic AI
 session. You build into the Sim workflow just the right amount of agentic
 AI reasoning needed to perform the users task.

Deploying Sim workflows can reduce the attack surface of potential agentic
AI rogue activities as well as reduces the blast radius of an unforeseen
agentic AI mishap.

[image: image.png]
