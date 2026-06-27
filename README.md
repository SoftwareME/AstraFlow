# AstraFlow

**Description**: AstraFlow is an AI-native project workflow blueprint that guides software projects from rough product ideas to PRDs, design systems, AI-generated visual directions, Figma handoff, frontend implementation, visual QA, automated testing, iterative fixes, and deployment.

This repository is a starter skeleton for running a full AI-assisted product workflow:

`idea -> product planning -> design direction -> image/reference generation -> Figma handoff -> frontend development -> visual QA -> automated fixes -> deployment`

The key idea is to make the project understandable to AI agents through stable context files instead of relying on one-off prompts.

## Main Files

- `AGENTS.md`: operating rules for AI agents.
- `docs/00-project-context.md`: permanent project background.
- `docs/01-product-brief.md`: short business and user summary.
- `docs/02-prd.md`: product requirements.
- `docs/03-design-system.md`: design tokens and UI rules.
- `docs/04-ai-workflow.md`: end-to-end AI execution flow.
- `docs/05-quality-gates.md`: acceptance criteria before delivery.
- `prompts/`: reusable prompt templates.
- `figma/`: Figma generation and handoff rules.
- `assets/`: reference images, generated images, cut assets, and asset pipeline.
- `qa/`: visual QA, automated testing, and regression rules.
- `deploy/`: deployment checklist and release flow.

## Recommended Start

1. Fill `docs/00-project-context.md`.
2. Fill `docs/01-product-brief.md`.
3. Let AI generate `docs/02-prd.md`.
4. Let AI propose 3 design directions.
5. Choose one direction.
6. Let AI create or update `docs/03-design-system.md`.
7. Generate reference images and Figma screens.
8. Implement the app.
9. Run visual QA and automated tests.
10. Deploy.

