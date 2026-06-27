# AI Project Operating Rules

This repository is designed for AI-assisted product, design, engineering, QA, and deployment.

## Read Order

Before making product, design, or code changes, read these files in order:

1. `docs/00-project-context.md`
2. `docs/01-product-brief.md`
3. `docs/02-prd.md`
4. `docs/03-design-system.md`
5. `docs/04-ai-workflow.md`
6. `docs/05-quality-gates.md`
7. `docs/06-positioning-vs-superpowers.md`
8. `docs/07-self-evolution.md`

If a task touches Figma, image generation, visual assets, or UI implementation, also read:

- `figma/figma-handoff.md`
- `assets/asset-pipeline.md`
- `prompts/design-prompt-assistant.md`
- `prompts/visual-qa.md`

## Default Behavior

- If the user's request is vague, offer 3 concrete options and let the user choose.
- Do not require the user to write polished prompts.
- Convert rough user intent into a structured execution prompt before implementation.
- Prefer real product screens over marketing pages.
- Preserve existing business logic unless the user explicitly asks to change it.
- Use realistic content, data density, states, and domain labels.
- Verify UI at desktop, tablet, and mobile breakpoints before final delivery.
- When a repeated failure, unclear prompt, visual defect, or process gap is discovered, update the relevant durable artifact and record the change in `docs/evolution/ledger.md`.

## UI Quality Rules

- No incoherent overlap between elements.
- No clipped button text, tab labels, form labels, table cells, or card content.
- No horizontal scrolling on mobile unless the component is intentionally scrollable.
- No nested cards unless they represent separate repeated objects or modals.
- No decorative blobs, generic gradients, or placeholder-heavy layouts.
- Use stable dimensions for boards, grids, tiles, toolbars, and fixed-format UI.
- Include loading, empty, error, disabled, hover, active, and selected states where relevant.

## Required Delivery Summary

Every completed implementation should report:

- What changed
- Which files changed
- Which checks were run
- Which visual breakpoints were inspected
- Remaining risks or manual follow-ups

## Self-Evolution Rule

Fixing the current output is not enough when the project reveals a recurring weakness.

If the task exposes a durable lesson, update at least one of:

- `docs/02-prd.md`
- `docs/03-design-system.md`
- `docs/05-quality-gates.md`
- `docs/07-self-evolution.md`
- `prompts/`
- `figma/figma-handoff.md`
- `assets/asset-pipeline.md`
- `qa/`
- `deploy/`

Then record the reason in `docs/evolution/ledger.md`.
