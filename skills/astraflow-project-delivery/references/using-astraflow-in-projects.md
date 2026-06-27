# Using AstraFlow In Real Projects

## Two Modes

Use AstraFlow as:

1. **Project template**: copy the AstraFlow files into a product repository.
2. **Skill**: install `skills/astraflow-project-delivery` so Codex can apply the workflow in any repository.
3. **Fallback instruction**: if skill discovery fails, copy `docs/09-skill-fallback-instructions.md` into the target project's `AGENTS.md`.

The best setup is both: install the skill globally, then add AstraFlow project files to each serious product repo.

For better trigger reliability, also install the short alias skill `skills/astraflow`.

## Minimal Project Files

For an existing project, add:

- `AGENTS.md`
- `docs/00-project-context.md`
- `docs/01-product-brief.md`
- `docs/02-prd.md`
- `docs/03-design-system.md`
- `docs/04-ai-workflow.md`
- `docs/05-quality-gates.md`
- `prompts/design-prompt-assistant.md`
- `prompts/frontend-implementation.md`
- `prompts/visual-qa.md`
- `qa/test-plan.md`
- `deploy/deployment-checklist.md`

For UI/Figma-heavy projects, also add:

- `figma/figma-handoff.md`
- `assets/asset-pipeline.md`
- `prompts/figma-generation.md`
- `prompts/image-generation.md`

For long-running projects, also add:

- `docs/07-self-evolution.md`
- `docs/evolution/ledger.md`

## Practical Use

User says:

```text
Use AstraFlow on this project. I have a rough idea, but I do not know how to write the prompt.
```

Agent should:

1. Read or create AstraFlow files.
2. Infer product type and goal.
3. Offer 3 design/product directions.
4. Wait for selection if the direction affects product/design.
5. Generate PRD and design system.
6. Create implementation contract.
7. Execute or hand off engineering.
8. Run visual QA and tests.
9. Prepare deployment checklist.
10. Record durable lessons.

## Superpowers Integration

Use Superpowers after AstraFlow creates the implementation contract.

Recommended handoff:

```text
Use Superpowers as the engineering execution engine for this AstraFlow implementation contract.

Read:
- AGENTS.md
- docs/00-project-context.md
- docs/01-product-brief.md
- docs/02-prd.md
- docs/03-design-system.md
- docs/05-quality-gates.md

Your job:
1. Resolve only engineering ambiguity.
2. Write an implementation plan from the PRD and design system.
3. Use TDD where code behavior is testable.
4. Use subagent-driven development when tasks are independent.
5. Review code against AstraFlow requirements.
6. Verify before claiming completion.
7. Return implementation evidence, test evidence, and gaps.

Do not replace AstraFlow's product, design, Figma, visual QA, asset, or deployment rules.
```

## Completion Evidence

Do not claim completion until evidence covers:

- PRD or product scope
- design system constraints
- implementation changes
- required states
- visual QA breakpoints
- tests or justified test gaps
- deployment readiness
- self-evolution record if the task exposed a durable lesson
