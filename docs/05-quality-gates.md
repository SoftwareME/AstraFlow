# Quality Gates

## Product Gate

- The primary user and workflow are clear.
- The first screen supports a real job.
- The PRD has acceptance criteria.

## Design Gate

- Design direction is selected.
- Design system tokens are documented.
- Components have required states.
- Content is realistic and domain-specific.

## Figma Gate

- Frames use Auto Layout where practical.
- Repeated UI is componentized.
- Variables or token names match `docs/03-design-system.md`.
- Layer names are understandable.
- No overlapping text or incoherent element stacking.

## Frontend Gate

- App renders without console-blocking errors.
- No text clipping in buttons, tabs, cards, tables, or forms.
- No unintended horizontal scroll on mobile.
- Critical states exist: loading, empty, error, disabled.
- Design matches the selected direction.

## Visual QA Gate

Required breakpoints:

- 1440px
- 1024px
- 390px

Reject delivery if any breakpoint has:

- Overlapping primary UI
- Clipped text
- Broken image
- Invisible focus state
- Unusable navigation
- Unclear primary action

## Test Gate

- Lint passes.
- Type check passes when applicable.
- Unit tests pass when applicable.
- End-to-end smoke test passes when applicable.
- Visual checks pass or documented exceptions are approved.

## Deployment Gate

- Environment variables are documented.
- Build succeeds.
- Preview deploy is checked.
- Rollback plan exists.

