---
name: astraflow-project-delivery
description: Use when the user says AstraFlow, astraflow, "Use AstraFlow", "使用 AstraFlow", "我不会写提示词", or wants a rough product idea, existing app, screenshot, Figma design, vague UI request, or Chinese product concept turned into product planning, PRD, design system, Figma/image handoff, frontend implementation, visual QA, tests, deployment readiness, or a full AI-native delivery workflow. This is a skill workflow, not a tool lookup.
---

# AstraFlow Project Delivery

Use AstraFlow as the product delivery operating system for AI-native projects.

## Core Rule

```text
AstraFlow decides what good means.
Engineering agents build it correctly.
Evidence proves it is done.
Failures improve the workflow.
```

## First Move

Do not search for an "AstraFlow tool" or wait after saying you will check for one. AstraFlow is a workflow skill. Once this skill is active, execute the workflow directly.

If the project has AstraFlow files, read them in this order:

1. `AGENTS.md`
2. `docs/00-project-context.md`
3. `docs/01-product-brief.md`
4. `docs/02-prd.md`
5. `docs/03-design-system.md`
6. `docs/04-ai-workflow.md`
7. `docs/05-quality-gates.md`

If files are missing, create the smallest useful version before continuing. For a new project, create at least:

- `AGENTS.md`
- `docs/00-project-context.md`
- `docs/01-product-brief.md`
- `docs/02-prd.md`
- `docs/03-design-system.md`
- `docs/05-quality-gates.md`

If the user gave a rough idea but did not explicitly ask for files, still produce the structured brief and 3 directions in the response, then ask them to choose one.

## Default Workflow

```text
rough idea
-> product context
-> product brief
-> PRD
-> 3 design directions
-> selected direction
-> design system
-> image/Figma/asset handoff
-> implementation contract
-> engineering execution
-> visual QA
-> tests
-> deployment readiness
-> self-evolution record
```

## When The User Cannot Prompt Well

Do not ask for a polished prompt. Do not stop after promising to convert the idea. Offer 3 options:

1. Conservative/professional
2. Premium/product-led
3. Dense/operational

Ask the user to choose one, then generate the professional execution prompt yourself.

## Implementation Contract

Before coding, produce or update:

- product goal
- target users
- primary workflow
- key screens
- acceptance criteria
- design tokens
- component states
- visual QA requirements
- test expectations
- deployment readiness checks

## Design And Visual QA Rules

Require:

- realistic product data and labels
- loading, empty, error, disabled, hover, active, and selected states where relevant
- desktop, tablet, and mobile review
- no incoherent overlap
- no clipped text
- no unintended mobile horizontal scroll
- no broken image assets
- no placeholder-heavy demo screens

## Superpowers Integration

If Superpowers is installed or requested, use it only as the engineering execution engine after AstraFlow defines the implementation contract.

Handoff rule:

```text
AstraFlow owns product, design, Figma, assets, visual QA, deployment, and evolution.
Superpowers owns engineering planning, TDD, subagents, review, debugging, and verification.
```

Read `references/using-astraflow-in-projects.md` when the user asks how to apply AstraFlow in a real project, package it as a skill, integrate Superpowers, or set up the project files.

## Self-Evolution

When a repeated problem, visual defect, prompt failure, QA miss, or deployment issue appears:

1. Fix the current issue.
2. Update the durable artifact that should prevent recurrence.
3. Record the lesson in `docs/evolution/ledger.md`.

Examples:

- vague prompt -> update `prompts/design-prompt-assistant.md`
- generic UI -> update `docs/03-design-system.md`
- overlap/clipping -> update `docs/05-quality-gates.md` and `prompts/visual-qa.md`
- Figma mess -> update `figma/figma-handoff.md`
- bad asset use -> update `assets/asset-pipeline.md`
- missed regression -> update `qa/test-plan.md`
- deploy failure -> update `deploy/deployment-checklist.md`
