# AstraFlow

[Voltar ao README principal](../README.md)

**Blueprint de fluxo de trabalho nativo para IA que transforma ideias iniciais em software desenhado, testado e implantável.**

`idea -> PRD -> design direction -> design system -> AI visuals -> Figma handoff -> frontend -> visual QA -> tests -> fixes -> deployment`

## Quickstart

Dê AstraFlow ao seu projeto:
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

Comece com o [Core Prompt](#the-core-prompt) e deixe o AstraFlow transformar sua ideia em PRD, sistema de design, handoff Figma, frontend, QA visual, testes, correções e preparação para implantação.

![AstraFlow and Superpowers full-loop workflow](../assets/diagrams/astraflow-superpowers-loop.svg)

Muitos projetos de IA falham porque a IA recebe um prompt vago, sem contexto de produto, regras de design, critérios de aceitação ou quality gates. AstraFlow fornece um sistema operacional de projeto para agentes de IA.

## Por que AstraFlow

Ferramentas de IA são poderosas, mas muitas equipes ainda as usam como chat: "melhore esta página", "crie um app", "gere um design", "corrija a UI", "implante". Funciona para demos. Falha em produtos reais.

AstraFlow dá memória de projeto à IA: objetivo, usuários, fluxos, regras de design, arquivos importantes, qualidade visual, testes e expectativas de implantação.

## Problemas que resolve

### 1. Prompts vagos criam produtos vagos

AstraFlow troca prompts isolados por `AGENTS.md`, `docs/02-prd.md`, `docs/03-design-system.md`, `docs/05-quality-gates.md` e prompts reutilizáveis.

### 2. UI gerada por IA parece demo

Exige fluxos reais, dados realistas, estados completos, layouts responsivos, sem texto cortado e sem sobreposição incoerente.

### 3. Design e engenharia se afastam

Conecta product brief, PRD, sistema de design, geração de imagens, handoff Figma, frontend e regressão visual.

### 4. Agentes de IA perdem contexto

Define ordem de leitura e fonte da verdade antes de qualquer mudança.

### 5. Entregar exige mais que código

Inclui testes, QA visual, gestão de assets, checklist de implantação e autoevolução.

## AstraFlow vs Superpowers

[obra/superpowers](https://github.com/obra/superpowers) é uma metodologia forte para coding agents. AstraFlow é diferente: é um sistema de entrega de produto nativo para IA.

Superpowers melhora como um AI coding agent trabalha. AstraFlow melhora como um projeto AI-native vai de ideia a design, Figma, frontend, QA e implantação.

Comparação: [../docs/06-positioning-vs-superpowers.md](../docs/06-positioning-vs-superpowers.md)  
Loop de integração: [../docs/08-full-loop-with-superpowers.md](../docs/08-full-loop-with-superpowers.md)

## Autoevolução

AstraFlow melhora com o tempo. Falhas repetidas devem virar prompts melhores, requisitos mais claros, regras de design, QA visual, regras Figma, restrições de assets, testes ou checklist de implantação.

Leia: [../docs/07-self-evolution.md](../docs/07-self-evolution.md), [../docs/evolution/ledger.md](../docs/evolution/ledger.md)

## Vantagens principais

- Estrutura AI-first
- Fluxo sem prompts perfeitos
- Padrão comercial de UI
- Handoff pronto para Figma
- Pipeline de imagens e assets
- Quality gates integrados
- Independente de stack
- Source of truth legível por agentes
- Útil como template, bootstrap, base CLI ou base Codex skill/plugin

## Para quem

Indie hackers, fundadores, design engineers, times de produto, agências, desenvolvedores e equipes que transformam Figma, screenshots e ideias em software real.

## Como funciona

```text
1. Capturar contexto de produto
2. Gerar ou refinar PRD
3. IA propõe 3 direções de design
4. Escolher uma direção
5. Criar sistema de design
6. Gerar referências visuais
7. Preparar handoff Figma
8. Implementar telas frontend reais
9. Rodar QA visual em desktop, tablet e mobile
10. Testar, corrigir e implantar
```

## Estrutura do repositório

Veja [../README.md#repository-structure](../README.md#repository-structure).

## Começo rápido

1. Clone ou copie este repositório.
2. Preencha `docs/00-project-context.md`.
3. Preencha `docs/01-product-brief.md`.
4. Peça ao agente de IA:

```text
Read AGENTS.md and the docs folder.
Use AstraFlow's workflow to turn this product idea into a PRD, 3 design directions, a design system, implementation plan, visual QA plan, and deployment checklist.
If anything is unclear, give me 3 options instead of asking me to write a perfect prompt.
```

5. Escolha uma direção.
6. Continue com implementação e QA.

### Codex App

Abra no Codex App e peça para ler `AGENTS.md`.

### Codex CLI

Execute Codex na raiz e comece com o core prompt.

### Claude Code

Abra no Claude Code e peça para seguir `AGENTS.md`.

### Cursor

Peça ao Cursor Agent para ler `AGENTS.md` e `docs/`.

### Gemini CLI

Execute Gemini CLI na raiz e siga AstraFlow.

### GitHub Copilot CLI

Use os arquivos do repositório como source of truth para planos e mudanças.

### Kimi Code

Siga a ordem de leitura do AstraFlow no Kimi Code.

### OpenCode

Execute OpenCode na raiz e comece com o core prompt.

### Figma

Use `figma/figma-handoff.md` e `prompts/figma-generation.md`.

### Superpowers Integration

Use AstraFlow para definir o que é bom e Superpowers como motor de engenharia.

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

## Quality Gates integrados

- Product gate
- Design gate
- Figma gate
- Frontend gate
- Visual QA gate
- Test gate
- Deployment gate

## Idiomas

Veja [README.md](README.md).

## Roadmap

- AstraFlow CLI
- Codex skill/plugin package
- Figma generation helpers
- Visual QA automation templates
- Example projects
- Multi-agent workflow templates

## License

Apache-2.0

