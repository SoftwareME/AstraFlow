# AstraFlow

[Вернуться к основному README](../README.md)

**AI-native blueprint рабочего процесса проекта, который превращает сырые идеи в спроектированное, протестированное и готовое к развертыванию ПО.**

`idea -> PRD -> design direction -> design system -> AI visuals -> Figma handoff -> frontend -> visual QA -> tests -> fixes -> deployment`

## Quickstart

Дайте проекту AstraFlow:
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

Начните с [Core Prompt](#the-core-prompt), затем AstraFlow превратит идею в PRD, дизайн-систему, Figma handoff, frontend, visual QA, тесты, исправления и готовность к deployment.

![AstraFlow and Superpowers full-loop workflow](../assets/diagrams/astraflow-superpowers-loop.svg)

Многие AI coding проекты проваливаются, потому что AI получает размытый prompt без стабильного продуктового контекста, дизайн-правил, критериев приемки и quality gates. AstraFlow дает AI-агентам структурированную систему работы.

## Зачем AstraFlow

AI-инструменты мощные, но команды часто используют их как чат: "улучши страницу", "создай приложение", "сгенерируй дизайн", "исправь UI", "задеплой". Это работает для demos, но ломается в реальных продуктах.

AstraFlow дает AI память проекта: цель, пользователей, workflows, дизайн-правила, важные файлы, визуальное качество, тесты и ожидания deployment.

## Какие проблемы решает

### 1. Размытые prompts создают размытые продукты

AstraFlow заменяет разовые prompts на `AGENTS.md`, `docs/02-prd.md`, `docs/03-design-system.md`, `docs/05-quality-gates.md` и reusable prompts.

### 2. AI-generated UI часто выглядит как demo

Требует реальные workflows, реалистичные данные, полные states, responsive layout, без обрезанного текста и хаотичных overlap.

### 3. Design и engineering расходятся

Соединяет product brief, PRD, design system, image generation, Figma handoff, frontend implementation и visual regression.

### 4. AI agents теряют context

Дает порядок чтения и source of truth перед изменениями.

### 5. Shipping требует больше, чем код

Включает tests, visual QA, asset management, deployment checklist и self-evolution.

## AstraFlow vs Superpowers

[obra/superpowers](https://github.com/obra/superpowers) — сильная методология software development для coding agents. AstraFlow отличается: это AI-native product delivery system.

Superpowers улучшает работу AI coding agent. AstraFlow улучшает структуру AI-native product project от идеи до design, Figma, frontend, QA и deployment.

Сравнение: [../docs/06-positioning-vs-superpowers.md](../docs/06-positioning-vs-superpowers.md)  
Integration loop: [../docs/08-full-loop-with-superpowers.md](../docs/08-full-loop-with-superpowers.md)

## Саморазвитие

AstraFlow улучшается со временем. Повторяющиеся failures должны превращаться в более сильные prompts, понятные requirements, строгие design rules, QA checks, Figma rules, asset constraints, tests или deployment checklist.

См.: [../docs/07-self-evolution.md](../docs/07-self-evolution.md), [../docs/evolution/ledger.md](../docs/evolution/ledger.md)

## Ключевые преимущества

- AI-first структура проекта
- Workflow без идеальных prompts
- Коммерческий уровень UI качества
- Figma-ready handoff
- Pipeline для images и assets
- Built-in quality gates
- Stack-agnostic
- Source of truth, понятный агентам
- Подходит как docs template, bootstrap, CLI foundation или Codex skill/plugin base

## Для кого

Indie hackers, founders, design engineers, product teams, agencies, developers и команды, превращающие Figma, screenshots и идеи в реальное ПО.

## Как работает

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

## Структура репозитория

См. [../README.md#repository-structure](../README.md#repository-structure).

## Быстрый старт

1. Clone или copy этот repository.
2. Заполните `docs/00-project-context.md`.
3. Заполните `docs/01-product-brief.md`.
4. Попросите AI coding agent:

```text
Read AGENTS.md and the docs folder.
Use AstraFlow's workflow to turn this product idea into a PRD, 3 design directions, a design system, implementation plan, visual QA plan, and deployment checklist.
If anything is unclear, give me 3 options instead of asking me to write a perfect prompt.
```

5. Выберите design direction.
6. Продолжайте implementation и QA.

### Codex App

Откройте repository в Codex App и попросите прочитать `AGENTS.md`.

### Codex CLI

Запустите Codex из root и начните с core prompt.

### Claude Code

Откройте repository в Claude Code и попросите следовать `AGENTS.md`.

### Cursor

Попросите Cursor Agent прочитать `AGENTS.md` и `docs/`.

### Gemini CLI

Запустите Gemini CLI из root и следуйте AstraFlow.

### GitHub Copilot CLI

Используйте файлы repository как source of truth для plans и changes.

### Kimi Code

Следуйте AstraFlow read order в Kimi Code.

### OpenCode

Запустите OpenCode из root и начните с core prompt.

### Figma

Используйте `figma/figma-handoff.md` и `prompts/figma-generation.md`.

### Superpowers Integration

AstraFlow определяет, что хорошо; Superpowers помогает построить это правильно.

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

## Языки

См. [README.md](README.md).

## Roadmap

- AstraFlow CLI
- Codex skill/plugin package
- Figma generation helpers
- Visual QA automation templates
- Example projects
- Multi-agent workflow templates

## License

Apache-2.0

