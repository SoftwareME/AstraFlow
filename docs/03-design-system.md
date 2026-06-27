# Design System

## Brand Feel

Choose 3-5 adjectives:

- TBD
- TBD
- TBD

## Color Tokens

| Token | Value | Usage |
| --- | --- | --- |
| `--color-bg` | TBD | Page background |
| `--color-surface` | TBD | Panels and primary surfaces |
| `--color-border` | TBD | Hairlines and dividers |
| `--color-text` | TBD | Primary text |
| `--color-muted` | TBD | Secondary text |
| `--color-accent` | TBD | Primary action and focus |
| `--color-danger` | TBD | Error and destructive states |

## Typography

| Role | Size | Weight | Line Height | Usage |
| --- | --- | --- | --- | --- |
| Page title | TBD | TBD | TBD | Main screen heading |
| Section title | TBD | TBD | TBD | Panels and sections |
| Body | TBD | TBD | TBD | Default text |
| Label | TBD | TBD | TBD | Forms, filters, metadata |
| Caption | TBD | TBD | TBD | Secondary metadata |

## Spacing Scale

Use a consistent spacing scale. Recommended base: 4px or 8px.

| Token | Value |
| --- | --- |
| `--space-1` | 4px |
| `--space-2` | 8px |
| `--space-3` | 12px |
| `--space-4` | 16px |
| `--space-6` | 24px |
| `--space-8` | 32px |

## Radius

Cards and controls should generally use 8px radius or less unless the product style requires otherwise.

## Components

Required component states:

- Default
- Hover
- Active
- Focus
- Selected
- Disabled
- Loading
- Empty
- Error

## Layout Rules

- Use constrained content width for reading-heavy pages.
- Use dense but calm layouts for dashboards and operational tools.
- Do not place cards inside cards unless representing repeated child records.
- Fixed-format components must have stable dimensions using grid tracks, aspect ratio, min/max sizes, or container constraints.
- Text must fit inside buttons, tabs, cards, table cells, and filters at all supported breakpoints.

## Breakpoints

| Breakpoint | Width | Requirement |
| --- | --- | --- |
| Mobile | 390px | No horizontal page scroll, no clipped controls |
| Tablet | 1024px | Navigation and primary workflow remain clear |
| Desktop | 1440px | Full product workflow visible and polished |

