# Design System

## Design Direction

Dense operational command center.

The product should feel like:

- enterprise control plane
- financial operations dashboard
- AI workforce command center
- strategy execution map

Avoid:

- consumer chatbot layout
- oversized marketing hero
- playful agent avatars as primary interface
- vague decorative gradients
- card stacks without operational density

## Brand Feel

- strategic
- precise
- institutional
- intelligent
- operational

## Layout

Recommended first screen:

- left navigation for company, strategy, org, agents, finance, projects, reports
- top bar with company stage, readiness score, token treasury health, active risks
- main canvas with strategy stage map and milestone blockers
- right panel with agent gaps, reward alerts, and approval items
- lower section with project portfolio and token flow summary

## Color Tokens

| Token | Use |
| --- | --- |
| `--color-bg` | neutral application background |
| `--color-surface` | panels and table surfaces |
| `--color-border` | dividers and grid lines |
| `--color-text` | primary operational text |
| `--color-muted` | labels and secondary metrics |
| `--color-strategy` | strategy stage and milestone indicators |
| `--color-agent` | agent and skill indicators |
| `--color-finance` | treasury and token indicators |
| `--color-risk` | warnings, gaps, failures |

## Component Inventory

- stage timeline
- org tree
- agent table
- skill matrix
- token ledger
- project dispatch board
- milestone checklist
- reward rule editor
- finance summary cards
- risk queue
- evidence drawer
- performance decision modal

## Required States

- loading
- empty
- error
- disabled
- selected
- active
- pending approval
- risk
- archived/eliminated

## Visual QA

Check:

- 1440px dashboard
- 1024px compressed operations view
- 390px mobile inspection view

Reject:

- overlapping tables and panels
- clipped role names
- clipped currency or token amounts
- unreadable org tree
- hidden primary action
- horizontal page scroll on mobile

