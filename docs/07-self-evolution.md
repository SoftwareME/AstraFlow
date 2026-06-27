# Self-Evolution System

AstraFlow should improve every time the project fails, ships, receives feedback, or discovers a repeated AI weakness.

This document defines the self-evolution loop.

## Principle

Do not rely on memory.

When something goes wrong, convert it into a durable project artifact:

- a better prompt
- a clearer rule
- a stronger quality gate
- a new checklist
- a new test
- a design-system constraint
- an asset-pipeline rule
- a Figma handoff rule

## Evolution Loop

```text
failure or feedback
-> classify
-> identify root cause
-> update durable artifact
-> add verification
-> record in evolution ledger
-> use in future AI runs
```

## Classification

Every improvement should be classified as one of:

- Product: unclear user, goal, workflow, acceptance criteria
- Design: weak hierarchy, bad spacing, poor typography, inconsistent components
- Visual QA: overlap, clipping, horizontal scroll, broken asset, unreadable state
- Figma: poor layer structure, missing components, weak Auto Layout, missing variables
- Asset: bad generation prompt, wrong export format, cut text as image, layout-shifting image
- Engineering: missing state, broken behavior, poor architecture, untested logic
- Testing: missing test, weak assertion, flaky test, incomplete coverage
- Deployment: broken build, missing env var, no preview check, no rollback path
- Prompting: user had to write too much, AI asked the wrong question, unclear option set

## Evolution Ledger

Keep durable records in:

- `docs/evolution/ledger.md`

Each entry should include:

```text
Date:
Trigger:
Category:
Symptom:
Root cause:
Changed artifact:
Verification added:
Future prevention rule:
```

## Required Artifact Updates

When a problem is found, update the smallest durable artifact that prevents recurrence:

| Problem | Update |
| --- | --- |
| User prompt was vague | `prompts/design-prompt-assistant.md` |
| Product intent was missing | `docs/00-project-context.md` or `docs/01-product-brief.md` |
| Requirement was ambiguous | `docs/02-prd.md` |
| UI looked generic | `docs/03-design-system.md` |
| Elements overlapped | `docs/05-quality-gates.md` and `prompts/visual-qa.md` |
| Figma handoff was messy | `figma/figma-handoff.md` |
| Image assets were misused | `assets/asset-pipeline.md` |
| Tests missed a regression | `qa/test-plan.md` |
| Deploy failed | `deploy/deployment-checklist.md` |

## Prompt Evolution

Prompts must evolve when:

- AI asks too many open-ended questions
- AI gives generic design advice
- AI skips visual QA
- AI fails to offer 3 concrete options
- AI implements before product/design direction is selected
- AI claims completion without evidence

Prompt updates should make the next run easier for a weaker agent, not just a stronger one.

## Design Evolution

Design rules must evolve when:

- the UI feels generic
- the layout lacks hierarchy
- controls resize unpredictably
- long text breaks components
- mobile layout compresses desktop UI instead of adapting
- charts, tables, or cards lose meaning with real data

Update `docs/03-design-system.md` with concrete constraints, not taste words.

## QA Evolution

Visual QA rules must evolve when:

- a bug reaches the user
- a screenshot reveals overlap or clipping
- a breakpoint was not checked
- a state was missing
- generated assets caused layout shift

Every visual regression should become either:

- a checklist item
- a browser QA step
- a screenshot baseline
- an automated test

## Completion Rule

An AstraFlow task is not complete until the relevant durable artifact has been updated.

Fixing the current output is not enough. The workflow must become better for the next run.

