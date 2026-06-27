# AI Workflow

## End-To-End Pipeline

```text
rough idea
-> product brief
-> PRD
-> 3 design directions
-> selected direction
-> design system
-> reference images
-> Figma draft
-> frontend implementation
-> browser visual QA
-> automated tests
-> automated fixes
-> deployment
```

## Stage 1: Product Planning

Inputs:

- `docs/00-project-context.md`
- `docs/01-product-brief.md`

Outputs:

- Updated `docs/02-prd.md`
- Key screens
- User stories
- Acceptance criteria

## Stage 2: Design Direction

The AI should propose 3 options:

1. Conservative/professional
2. Premium/product-led
3. Dense/operational

The user selects one. The AI then updates:

- `docs/03-design-system.md`
- `prompts/frontend-implementation.md`
- `prompts/visual-qa.md`

## Stage 3: Image And Asset Generation

Use image generation for:

- Mood direction
- Hero/product imagery
- Icons or illustrations when needed
- Texture or scene references

Generated images must be placed in:

- `assets/generated/`

Reference images must be placed in:

- `assets/references/`

Cut/exported production assets must be placed in:

- `assets/cut/`

## Stage 4: Figma Generation

Use Figma when the project needs editable design files, design system variables, components, or stakeholder review.

Follow:

- `figma/figma-handoff.md`

## Stage 5: Frontend Development

Use the existing stack when present. Otherwise choose a standard app stack and document the decision.

The AI must:

- Implement real screens.
- Preserve business logic.
- Use domain-specific content.
- Add required states.
- Avoid overlapping or clipped UI.
- Keep layout responsive.

## Stage 6: Visual QA

Inspect:

- 1440px desktop
- 1024px tablet
- 390px mobile

Fix:

- Overlap
- Clipping
- Horizontal scroll
- Blank rendering
- Poor contrast
- Broken assets
- Awkward density

## Stage 7: Automated Tests

Run unit, integration, accessibility, and visual checks where available.

## Stage 8: Deployment

Follow:

- `deploy/deployment-checklist.md`

