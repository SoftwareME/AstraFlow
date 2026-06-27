---
name: astraflow
description: Use when the user says AstraFlow, astraflow, "Use AstraFlow", "使用 AstraFlow", "我不会写提示词", "不会提示词", "给我 3 个方案", or asks to turn a rough product idea into PRD, design system, implementation plan, visual QA, deployment readiness, or AI-native project workflow. This is a workflow skill; do not search for dynamic tools.
---

# AstraFlow

AstraFlow is a workflow skill, not a dynamic tool.

If this skill activates, do not say "I will look for AstraFlow tools/capabilities" and then stop. Execute the workflow directly.

## Immediate Behavior

If the user gives a rough idea:

1. Produce a structured product brief.
2. Produce 3 MVP/product/design directions.
3. Ask the user to choose one direction.
4. If the user asked for project artifacts, create or update:
   - `AGENTS.md`
   - `docs/00-project-context.md`
   - `docs/01-product-brief.md`
   - `docs/02-prd.md`
   - `docs/03-design-system.md`
   - `docs/05-quality-gates.md`

If the repository already contains `skills/astraflow-project-delivery`, use that skill's fuller workflow.

## Core Flow

```text
rough idea
-> product brief
-> PRD
-> 3 directions
-> design system
-> implementation contract
-> visual QA
-> tests
-> deployment readiness
```

## Do Not Stop At

```text
I will check whether AstraFlow is available.
```

That is not progress. Continue with the structured brief and 3 directions.

