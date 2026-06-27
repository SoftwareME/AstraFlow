# AstraFlow

[मुख्य README पर वापस जाएं](../README.md)

**AI-native project workflow blueprint जो rough ideas को designed, tested और deployable software में बदलता है।**

`idea -> PRD -> design direction -> design system -> AI visuals -> Figma handoff -> frontend -> visual QA -> tests -> fixes -> deployment`

## Quickstart

अपने project को AstraFlow दें:
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

[Core Prompt](#the-core-prompt) से शुरू करें, फिर AstraFlow आपके idea को PRD, design system, Figma handoff, frontend implementation, visual QA, tests, fixes और deployment readiness में बदलेगा।

![AstraFlow and Superpowers full-loop workflow](../assets/diagrams/astraflow-superpowers-loop.svg)

कई AI coding projects इसलिए fail होते हैं क्योंकि AI को vague prompt दिया जाता है, बिना stable product context, design rules, acceptance criteria या quality gates के। AstraFlow AI agents के लिए structured project operating system देता है।

## AstraFlow क्यों

AI tools शक्तिशाली हैं, लेकिन कई teams उन्हें chat box की तरह इस्तेमाल करती हैं: "page बेहतर बनाओ", "app बनाओ", "design generate करो", "UI fix करो", "deploy करो"। यह demos के लिए ठीक है, real products के लिए नहीं।

AstraFlow AI को project memory देता है: purpose, users, workflows, design rules, important files, visual quality, tests और deployment expectations।

## यह किन समस्याओं को हल करता है

### 1. Vague prompts vague products बनाते हैं

AstraFlow one-off prompts की जगह `AGENTS.md`, `docs/02-prd.md`, `docs/03-design-system.md`, `docs/05-quality-gates.md` और reusable prompts देता है।

### 2. AI-generated UI अक्सर demo जैसी लगती है

यह real workflows, realistic data, complete states, responsive layouts, no clipped text और no incoherent overlap पर जोर देता है।

### 3. Design और engineering अलग हो जाते हैं

यह product brief, PRD, design system, image generation, Figma handoff, frontend implementation और visual regression checks को जोड़ता है।

### 4. AI agents context खो देते हैं

हर बदलाव से पहले read order और source of truth देता है।

### 5. Shipping सिर्फ code नहीं है

Tests, visual QA, asset management, deployment checklist और self-evolution शुरुआत से शामिल हैं।

## AstraFlow vs Superpowers

[obra/superpowers](https://github.com/obra/superpowers) coding agents के लिए strong software-development methodology है। AstraFlow अलग है: यह AI-native product delivery system है।

Superpowers AI coding agent के काम करने के तरीके को बेहतर बनाता है। AstraFlow product project को idea से design, Figma, frontend, QA और deployment तक structure करता है।

Comparison: [../docs/06-positioning-vs-superpowers.md](../docs/06-positioning-vs-superpowers.md)  
Integration loop: [../docs/08-full-loop-with-superpowers.md](../docs/08-full-loop-with-superpowers.md)

## Self-Evolution

AstraFlow समय के साथ बेहतर होता है। Repeated failures को stronger prompts, clearer requirements, tighter design rules, better QA checks, Figma rules, asset constraints, tests या deployment checklist items में बदलना चाहिए।

Read: [../docs/07-self-evolution.md](../docs/07-self-evolution.md), [../docs/evolution/ledger.md](../docs/evolution/ledger.md)

## Key Advantages

- AI-first project structure
- Perfect prompts की जरूरत नहीं
- Commercial UI quality bar
- Figma-ready handoff
- Image generation और asset pipeline
- Built-in quality gates
- Stack-agnostic
- Agent-readable source of truth
- Docs template, bootstrap, CLI foundation या Codex skill/plugin base के रूप में उपयोगी

## किसके लिए

Indie hackers, founders, design engineers, product teams, agencies, developers, और teams जो Figma, screenshots और ideas को real software में बदलना चाहते हैं।

## यह कैसे काम करता है

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

देखें [../README.md#repository-structure](../README.md#repository-structure).

## Quick Start

1. इस repository को clone या copy करें।
2. `docs/00-project-context.md` भरें।
3. `docs/01-product-brief.md` भरें।
4. AI coding agent से कहें:

```text
Read AGENTS.md and the docs folder.
Use AstraFlow's workflow to turn this product idea into a PRD, 3 design directions, a design system, implementation plan, visual QA plan, and deployment checklist.
If anything is unclear, give me 3 options instead of asking me to write a perfect prompt.
```

5. एक design direction चुनें।
6. Implementation और QA जारी रखें।

### Codex App

Codex App में repository खोलें और `AGENTS.md` पढ़ने को कहें।

### Codex CLI

Repository root से Codex चलाएं और core prompt से शुरू करें।

### Claude Code

Claude Code में repository खोलें और `AGENTS.md` follow करवाएं।

### Cursor

Cursor Agent से `AGENTS.md` और `docs/` पढ़ने को कहें।

### Gemini CLI

Repository root से Gemini CLI चलाएं और AstraFlow follow करवाएं।

### GitHub Copilot CLI

Repository files को source of truth बनाकर plans और changes generate करें।

### Kimi Code

Kimi Code में AstraFlow read order follow करें।

### OpenCode

Repository root से OpenCode चलाएं और core prompt से शुरू करें।

### Figma

`figma/figma-handoff.md` और `prompts/figma-generation.md` इस्तेमाल करें।

### Superpowers Integration

AstraFlow define करता है कि अच्छा क्या है; Superpowers उसे सही तरीके से build करने में मदद करता है।

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

देखें [README.md](README.md).

## Roadmap

- AstraFlow CLI
- Codex skill/plugin package
- Figma generation helpers
- Visual QA automation templates
- Example projects
- Multi-agent workflow templates

## License

Apache-2.0

