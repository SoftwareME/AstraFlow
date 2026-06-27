# AstraFlow

**AI-native project workflow blueprint for turning rough ideas into designed, tested, and deployable software.**

`idea -> PRD -> design direction -> design system -> AI visuals -> Figma handoff -> frontend -> visual QA -> tests -> fixes -> deployment`

Most AI coding projects fail for the same reason: the AI is asked to build from a vague prompt, without stable product context, design rules, acceptance criteria, or quality gates.

AstraFlow fixes that.

It gives your project a structured operating system for AI agents, so product planning, UI design, implementation, testing, and deployment can happen as one repeatable workflow instead of a pile of disconnected prompts.

## Why AstraFlow

Modern AI tools are powerful, but most teams still use them like a chat box:

- "Make this page look better."
- "Build me an app."
- "Generate a design."
- "Fix the UI."
- "Deploy it."

That works for demos. It breaks for real products.

AstraFlow gives AI the missing project memory:

- what the product is
- who the users are
- what the screen must accomplish
- what design system to follow
- what files matter
- what visual issues are unacceptable
- what tests must pass
- how to prepare for Figma and deployment

Instead of asking AI to guess, AstraFlow teaches AI how your project thinks.

## What Problems It Solves

### 1. Vague Prompts Create Vague Products

AstraFlow replaces one-off prompting with structured project files:

- `AGENTS.md` for AI operating rules
- `docs/02-prd.md` for product requirements
- `docs/03-design-system.md` for design tokens and layout rules
- `docs/05-quality-gates.md` for acceptance criteria
- `prompts/` for reusable high-quality prompts

### 2. AI-Generated UI Often Looks Like a Demo

AstraFlow pushes AI toward commercial-grade product interfaces:

- realistic data
- real workflows
- loading, empty, error, disabled, hover, active, and selected states
- responsive layouts
- no clipped text
- no incoherent overlap
- no placeholder-heavy screens

### 3. Design And Engineering Drift Apart

AstraFlow connects:

- product brief
- PRD
- design system
- image generation
- Figma handoff
- frontend implementation
- visual regression checks

Design decisions become implementation constraints, not forgotten screenshots.

### 4. AI Agents Lose Context

AstraFlow gives every AI agent a read order and source of truth. Before changing anything, agents know which files to inspect and which quality rules to follow.

### 5. Shipping Requires More Than Code

AstraFlow includes testing, visual QA, asset management, and deployment checklists from the beginning.

## Key Advantages

- **AI-first project structure**: Built for Codex, Cursor, Claude Code, Copilot, and other AI coding agents.
- **Promptless workflow**: Users can choose from options instead of writing perfect prompts.
- **Commercial UI quality bar**: Explicit rules for hierarchy, spacing, typography, responsive design, and anti-overlap QA.
- **Figma-ready handoff**: Includes Figma structure, component rules, Auto Layout guidance, and token mapping.
- **Image generation pipeline**: Defines where generated visuals, references, and production cut assets belong.
- **Quality gates included**: Product, design, frontend, visual QA, test, and deployment gates.
- **Stack-agnostic**: Works with any frontend or app framework.
- **Agent-readable**: Every major workflow is documented in plain files AI can reliably follow.
- **Open-ended by design**: Use it as a docs template, project bootstrap, CLI foundation, or Codex skill/plugin base.

## Who Should Use It

AstraFlow is for:

- indie hackers building with AI
- founders prototyping products
- design engineers creating polished interfaces
- product teams standardizing AI workflows
- agencies delivering client projects faster
- developers who want AI output to be more reliable
- teams turning Figma, screenshots, and product ideas into real software

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

```text
.
├── AGENTS.md
├── docs/
│   ├── 00-project-context.md
│   ├── 01-product-brief.md
│   ├── 02-prd.md
│   ├── 03-design-system.md
│   ├── 04-ai-workflow.md
│   └── 05-quality-gates.md
├── prompts/
│   ├── design-prompt-assistant.md
│   ├── product-planning.md
│   ├── design-direction.md
│   ├── image-generation.md
│   ├── figma-generation.md
│   ├── frontend-implementation.md
│   └── visual-qa.md
├── figma/
│   └── figma-handoff.md
├── assets/
│   ├── asset-pipeline.md
│   ├── references/
│   ├── generated/
│   ├── cut/
│   └── icons/
├── qa/
│   ├── test-plan.md
│   └── visual-regression.md
└── deploy/
    └── deployment-checklist.md
```

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

## The Core Prompt

Use this when you do not know how to write a good prompt:

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

AstraFlow rejects weak AI output by default.

Before delivery, the project should pass:

- **Product gate**: clear users, workflow, and acceptance criteria
- **Design gate**: documented tokens, states, and responsive rules
- **Figma gate**: reusable components, clean layers, no overlap
- **Frontend gate**: no clipping, no broken layout, no missing critical states
- **Visual QA gate**: checked at 1440px, 1024px, and 390px
- **Test gate**: lint, typecheck, unit, integration, or e2e where applicable
- **Deployment gate**: build, preview, smoke test, rollback path

## Multilingual Overview

### English

AstraFlow is an AI-native project workflow blueprint that helps teams turn rough ideas into PRDs, design systems, Figma-ready designs, production frontend code, visual QA, automated tests, iterative fixes, and deployable software. It gives AI agents the context and rules they need to produce reliable product work.

### 中文

AstraFlow 是一个面向 AI 原生研发的项目工作流蓝图，帮助团队把粗略想法转化为 PRD、设计系统、可交付 Figma 设计、前端实现、视觉 QA、自动化测试、自动修复和可部署软件。它为 AI 代理提供稳定上下文和质量规则，让 AI 不再只靠临时提示词猜测。

### 日本語

AstraFlow は、AI ネイティブなプロジェクトワークフローのブループリントです。粗いアイデアを PRD、デザインシステム、Figma 向けデザイン、フロントエンド実装、ビジュアル QA、自動テスト、反復修正、デプロイ可能なソフトウェアへ変換するための構造を提供します。AI エージェントに必要な文脈と品質ルールを与えます。

### 한국어

AstraFlow는 AI 네이티브 프로젝트 워크플로우 블루프린트입니다. 막연한 아이디어를 PRD, 디자인 시스템, Figma 핸드오프, 프론트엔드 구현, 시각 QA, 자동화 테스트, 반복 수정, 배포 가능한 소프트웨어로 발전시키는 구조를 제공합니다. AI 에이전트가 안정적으로 일할 수 있도록 맥락과 품질 기준을 제공합니다.

### Español

AstraFlow es un blueprint de flujo de trabajo nativo para IA que ayuda a convertir ideas iniciales en PRD, sistemas de diseño, diseños listos para Figma, código frontend, QA visual, pruebas automatizadas, correcciones iterativas y software desplegable. Proporciona a los agentes de IA el contexto y las reglas necesarias para trabajar con fiabilidad.

### Français

AstraFlow est un blueprint de workflow natif pour l'IA qui transforme des idées brutes en PRD, systèmes de design, maquettes prêtes pour Figma, code frontend, QA visuelle, tests automatisés, corrections itératives et logiciel déployable. Il donne aux agents IA le contexte et les règles nécessaires pour produire un travail fiable.

### Deutsch

AstraFlow ist ein KI-natives Projekt-Workflow-Blueprint, das grobe Ideen in PRDs, Designsysteme, Figma-fähige Designs, Frontend-Code, visuelle QA, automatisierte Tests, iterative Korrekturen und deploybare Software überführt. Es gibt KI-Agenten den Kontext und die Regeln, die sie für zuverlässige Produktarbeit benötigen.

### Português

AstraFlow é um blueprint de fluxo de trabalho nativo para IA que ajuda equipes a transformar ideias iniciais em PRDs, sistemas de design, designs prontos para Figma, código frontend, QA visual, testes automatizados, correções iterativas e software implantável. Ele fornece aos agentes de IA o contexto e as regras de qualidade necessárias.

### Русский

AstraFlow — это AI-native blueprint рабочего процесса проекта, который помогает превращать сырые идеи в PRD, дизайн-системы, Figma-ready макеты, frontend-код, визуальный QA, автоматические тесты, итеративные исправления и готовое к развертыванию ПО. Он дает AI-агентам контекст и правила качества для надежной работы.

### العربية

AstraFlow هو مخطط عمل مخصص للمشاريع المعتمدة على الذكاء الاصطناعي. يساعد الفرق على تحويل الأفكار الأولية إلى PRD، وأنظمة تصميم، وتصاميم جاهزة لـ Figma، وواجهات أمامية، وفحص بصري، واختبارات آلية، وتحسينات متكررة، وبرمجيات قابلة للنشر. يمنح وكلاء الذكاء الاصطناعي السياق والقواعد اللازمة للعمل بثبات.

### हिन्दी

AstraFlow एक AI-native project workflow blueprint है, जो शुरुआती विचारों को PRD, design systems, Figma-ready designs, frontend implementation, visual QA, automated tests, iterative fixes और deployable software में बदलने में मदद करता है। यह AI agents को बेहतर और भरोसेमंद काम के लिए जरूरी context और quality rules देता है।

## Roadmap

- AstraFlow CLI: `astraflow init`, `astraflow plan`, `astraflow design`, `astraflow qa`, `astraflow deploy`
- Codex skill/plugin package
- Figma generation helpers
- Visual QA automation templates
- Example projects
- Multi-agent workflow templates

## License

MIT

