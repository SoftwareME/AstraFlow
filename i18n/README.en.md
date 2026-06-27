# AstraFlow

[Back to main README](../README.md)

**AI-native project workflow blueprint for turning rough ideas into designed, tested, and deployable software.**

`idea -> PRD -> design direction -> design system -> AI visuals -> Figma handoff -> frontend -> visual QA -> tests -> fixes -> deployment`

## Quickstart

Give your project AstraFlow:
[Codex App](#codex-app),
[Codex CLI](#codex-cli),
[Claude Code](#claude-code),
[Cursor](#cursor),
[Gemini CLI](#gemini-cli),
[GitHub Copilot CLI](#github-copilot-cli),
[Kimi Code](#kimi-code),
[OpenCode](#opencode),
[Figma](#figma),
[Superpowers](#superpowers-integration).

Start with the [Core Prompt](#the-core-prompt), then let AstraFlow turn your idea into a PRD, design system, Figma-ready handoff, frontend implementation, visual QA, tests, fixes, and deployment readiness.

![AstraFlow and Superpowers full-loop workflow](../assets/diagrams/astraflow-superpowers-loop.svg)

Most AI coding projects fail because the AI is asked to build from a vague prompt, without stable product context, design rules, acceptance criteria, or quality gates. AstraFlow gives your project a structured operating system for AI agents.

## Why AstraFlow

Modern AI tools are powerful, but teams still use them like a chat box: "make this page better", "build an app", "generate a design", "fix the UI", "deploy it". That works for demos. It breaks for real products.

AstraFlow gives AI the missing project memory: product purpose, users, workflows, design rules, important files, visual quality rules, tests, and deployment expectations.

## What Problems It Solves

### 1. Vague Prompts Create Vague Products

AstraFlow replaces one-off prompting with structured project files: `AGENTS.md`, `docs/02-prd.md`, `docs/03-design-system.md`, `docs/05-quality-gates.md`, and reusable prompts.

### 2. AI-Generated UI Often Looks Like a Demo

AstraFlow pushes AI toward real workflows, realistic data, complete states, responsive layouts, no clipped text, no incoherent overlap, and no placeholder-heavy screens.

### 3. Design And Engineering Drift Apart

AstraFlow connects product brief, PRD, design system, image generation, Figma handoff, frontend implementation, and visual regression checks.

### 4. AI Agents Lose Context

AstraFlow gives every AI agent a read order and source of truth before changing anything.

### 5. Shipping Requires More Than Code

AstraFlow includes testing, visual QA, asset management, deployment checklists, and self-evolution from the beginning.

## AstraFlow vs Superpowers

[obra/superpowers](https://github.com/obra/superpowers) is a strong software-development methodology for coding agents. AstraFlow is different: it is an AI-native product delivery system.

Superpowers improves how an AI coding agent works. AstraFlow improves how an AI-native product project is structured from idea to design, Figma, frontend, QA, and deployment.

Use both when you want Superpowers for engineering discipline and AstraFlow for product, design, visual QA, assets, Figma handoff, and deployment structure.

Read the comparison: [../docs/06-positioning-vs-superpowers.md](../docs/06-positioning-vs-superpowers.md)  
See the integration loop: [../docs/08-full-loop-with-superpowers.md](../docs/08-full-loop-with-superpowers.md)

## Self-Evolution

AstraFlow improves over time. Repeated failures should become durable artifacts: stronger prompts, clearer requirements, tighter design rules, better visual QA checks, Figma rules, asset constraints, tests, or deployment checklist items.

Read: [../docs/07-self-evolution.md](../docs/07-self-evolution.md) and [../docs/evolution/ledger.md](../docs/evolution/ledger.md).

## Key Advantages

- AI-first project structure
- Promptless workflow with user-friendly options
- Commercial UI quality bar
- Figma-ready handoff
- Image generation and asset pipeline
- Built-in quality gates
- Stack-agnostic
- Agent-readable source of truth
- Usable as docs template, bootstrap, CLI foundation, or Codex skill/plugin base

## Who Should Use It

Indie hackers, founders, design engineers, product teams, agencies, developers, and teams turning Figma, screenshots, and product ideas into real software.

## How It Works

```text
1. Capture product context
2. Generate or refine the PRD
3. Ask AI to propose 3 design directions
4. Choose a direction
5. Create a design system
6. Generate visual references or product imagery
7. Prepare Figma handoff
8. Implement real frontend screens
9. Run visual QA at desktop, tablet, and mobile sizes
10. Run tests, fix issues, and deploy
```

## Repository Structure

See the main repository structure in [../README.md#repository-structure](../README.md#repository-structure).

## Quick Start

1. Clone or copy this repository.
2. Fill in `docs/00-project-context.md`.
3. Fill in `docs/01-product-brief.md`.
4. Ask your AI coding agent:

```text
Read AGENTS.md and the docs folder.
Use AstraFlow's workflow to turn this product idea into a PRD, 3 design directions, a design system, implementation plan, visual QA plan, and deployment checklist.
If anything is unclear, give me 3 options instead of asking me to write a perfect prompt.
```

5. Choose one design direction.
6. Let the AI continue through implementation and QA.

### Codex App

Open this repository in Codex App and ask it to read `AGENTS.md` and use AstraFlow.

### Codex CLI

Run Codex from the repository root and start with the core prompt below.

### Claude Code

Open the repository in Claude Code and ask it to follow `AGENTS.md`.

### Cursor

Open the repository in Cursor Agent and ask it to read `AGENTS.md` plus `docs/`.

### Gemini CLI

Run Gemini CLI from the repository root and ask it to follow the AstraFlow workflow.

### GitHub Copilot CLI

Use the repository files as the source of truth for plans and implementation changes.

### Kimi Code

Open the project in Kimi Code and follow the AstraFlow read order.

### OpenCode

Run OpenCode from the repository root and begin with the core prompt.

### Figma

Use `figma/figma-handoff.md` and `prompts/figma-generation.md`.

### Superpowers Integration

Use AstraFlow to define what good means, then use Superpowers as the engineering execution engine.

## The Core Prompt

```text
I do not know how to write design or product prompts.

Use AstraFlow as a Design Prompt Assistant.

First, read AGENTS.md and the docs folder.
Then infer my product goal and give me 3 options:
A. Conservative/professional
B. Premium/product-led
C. Dense/operational

Explain the tradeoffs in plain language.
After I choose one, generate the full professional prompt automatically and execute the workflow:
product planning, PRD, design system, AI visual direction, Figma handoff plan, frontend implementation, visual QA, testing, fixes, and deployment readiness.
```

## Built-In Quality Gates

- Product gate
- Design gate
- Figma gate
- Frontend gate
- Visual QA gate
- Test gate
- Deployment gate

## Languages

See [README.md](README.md).

## Roadmap

- AstraFlow CLI
- Codex skill/plugin package
- Figma generation helpers
- Visual QA automation templates
- Example projects
- Multi-agent workflow templates

## License

Apache-2.0

