# Figma Handoff

## Purpose

Use Figma when the product needs editable design review, reusable components, design tokens, or stakeholder handoff.

## Inputs

- `docs/02-prd.md`
- `docs/03-design-system.md`
- `assets/references/`
- `assets/generated/`
- live frontend URL when available

## Output Structure

Recommended Figma pages:

1. Cover
2. Product Flow
3. Design System
4. Components
5. Desktop Screens
6. Mobile Screens
7. States
8. Archive

## Component Rules

- Use components for repeated navigation, buttons, inputs, filters, cards, tables, modals, and status badges.
- Use variants for states and sizes.
- Use Auto Layout where practical.
- Use token names aligned with `docs/03-design-system.md`.

## Anti-Overlap Rules

- Text layers must have explicit width and Auto Layout constraints.
- Buttons must have minimum width or content-aware padding.
- Cards must use Auto Layout or stable internal spacing.
- Tables must define column behavior.
- Mobile frames must use stacked layouts instead of compressed desktop layouts.

## Handoff Checklist

- Frames named clearly.
- Components named clearly.
- Variables documented.
- Critical states included.
- Desktop and mobile frames included.
- No overlapping text.
- No clipped labels.
- No decorative artifacts that cannot be implemented.

