# Visual Regression

## Required Checks

Run visual inspection at:

- 1440x900
- 1024x768
- 390x844

## Failure Conditions

- Text overlap
- Text clipping
- Broken images
- Blank page
- Unintended horizontal scroll
- Primary action not visible
- Navigation unusable
- Modal or drawer inaccessible
- Table columns unreadable
- Form fields compressed beyond usability

## Recommended Automation

Use browser automation to:

1. Start the app.
2. Visit critical routes.
3. Capture screenshots.
4. Compare screenshots against baselines when available.
5. Inspect DOM for horizontal scroll and oversized elements.
6. Fail the check when critical visual issues exist.

