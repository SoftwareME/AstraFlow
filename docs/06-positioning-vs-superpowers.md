# AstraFlow vs Superpowers

This document explains how AstraFlow differs from [obra/superpowers](https://github.com/obra/superpowers), what AstraFlow can learn from it, and where AstraFlow should deliberately solve a different problem.

## Short Version

Superpowers is a software-development methodology for coding agents.

AstraFlow is an AI-native product delivery system for turning product ideas into designed, tested, and deployable software.

They overlap in disciplined agent execution, but they optimize for different layers:

- Superpowers improves how an AI coding agent works.
- AstraFlow improves how an AI-native product project is structured, designed, validated, and shipped.

## Evidence From Superpowers

Superpowers describes itself as:

> a complete software development methodology for your coding agents, built on top of a set of composable skills and some initial instructions that make sure your agent uses them.

Its core workflow emphasizes:

- brainstorming before implementation
- writing plans
- using git worktrees
- subagent-driven development
- test-driven development
- code review
- systematic debugging
- verification before completion
- writing new skills

That makes Superpowers strong at engineering discipline and agent behavior.

## AstraFlow's Different Center Of Gravity

AstraFlow starts earlier and ends later.

It covers:

- product brief
- PRD
- design direction
- design system
- AI visual generation
- asset pipeline
- Figma handoff
- frontend implementation
- visual QA
- automated tests
- deployment readiness
- project-level AI context

Superpowers asks: "How should the coding agent work?"

AstraFlow asks: "What project structure lets AI take an idea through product, design, engineering, QA, and deployment without losing context?"

## Comparison

| Area | Superpowers | AstraFlow |
| --- | --- | --- |
| Primary unit | Agent skills and workflows | Project blueprint and delivery pipeline |
| Main user | Developers using coding agents | Founders, product teams, design engineers, agencies, AI builders |
| Starting point | A coding task or feature idea | A rough product idea, screenshot, product brief, or design need |
| Product planning | Brainstorming and spec refinement | Product context, product brief, PRD, acceptance criteria |
| Design system | Not the primary focus | First-class design tokens, layout rules, component states |
| Figma | Not the primary focus | First-class handoff target |
| Image generation | Not the primary focus | First-class reference and asset pipeline |
| UI visual QA | Covered indirectly through verification | Explicit anti-overlap, clipping, responsive, and visual quality gates |
| Deployment | Branch finishing and verification | Deployment checklist and release readiness |
| Self-improvement | Writing new skills | Project evolution ledger, prompt evolution, design rule evolution, QA failure memory |
| Best use | Make agents better at software engineering | Make AI-native product delivery reliable end to end |

## Problems AstraFlow Can Solve That Superpowers Does Not Primarily Target

### 1. Design Quality Drift

Superpowers improves engineering method, but it does not define a product-specific visual system by default.

AstraFlow gives AI:

- brand feel
- color tokens
- typography scale
- spacing scale
- radius and surface rules
- component states
- responsive rules
- anti-overlap rules

This helps prevent AI-generated UI from looking like a generic demo.

### 2. Figma-To-Code Continuity

AstraFlow treats Figma as part of the delivery pipeline, not a side artifact.

It defines:

- Figma page structure
- component rules
- Auto Layout guidance
- design token mapping
- handoff requirements
- manual cleanup expectations

### 3. AI Image And Asset Governance

AstraFlow separates:

- reference images
- generated visual directions
- cut production assets
- icons

It also says what should not be cut as images: text, buttons, tables, forms, and normal UI controls.

### 4. Product-To-Design-To-Engineering Continuity

AstraFlow gives AI a chain of source-of-truth files:

```text
project context -> product brief -> PRD -> design system -> workflow -> quality gates
```

This reduces the chance that implementation ignores product intent or design constraints.

### 5. Visual Acceptance As A First-Class Gate

AstraFlow makes visual quality explicit:

- check 1440px desktop
- check 1024px tablet
- check 390px mobile
- reject overlap
- reject clipped text
- reject unintended horizontal scroll
- reject broken assets
- reject missing critical states

This is broader than simply verifying tests pass.

### 6. Non-Expert Prompting

AstraFlow is designed for users who cannot write excellent prompts.

Instead of requiring a perfect prompt, it asks AI to offer 3 options and convert the user's selection into a professional execution prompt.

## What AstraFlow Should Learn From Superpowers

AstraFlow should adopt the strongest parts of Superpowers without becoming a clone:

- mandatory verification before completion
- skill-like reusable workflows
- pressure-tested process documentation
- subagent review loops where available
- explicit self-improvement through new rules, prompts, and checks
- evidence-based completion claims

The key is to apply those ideas to product, design, Figma, assets, visual QA, and deployment, not only coding.

## AstraFlow's Defensible Position

AstraFlow should become:

> the AI-native operating system for product delivery, where every artifact an AI needs is structured, reviewable, reusable, and testable.

That means AstraFlow is not "Superpowers but smaller."

It is a complementary layer:

- Superpowers can power the coding agent.
- AstraFlow can define the project delivery system that the agent works inside.

Used together, Superpowers can improve the agent's engineering discipline while AstraFlow gives the project product/design/QA/deployment structure.

