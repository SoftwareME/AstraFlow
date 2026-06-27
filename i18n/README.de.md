# AstraFlow

[Zurück zum Haupt-README](../README.md)

**KI-natives Projekt-Workflow-Blueprint, das grobe Ideen in gestaltete, getestete und deploybare Software verwandelt.**

`idea -> PRD -> design direction -> design system -> AI visuals -> Figma handoff -> frontend -> visual QA -> tests -> fixes -> deployment`

## Quickstart

Gib deinem Projekt AstraFlow:
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

Starte mit dem [Core Prompt](#the-core-prompt). AstraFlow macht daraus PRD, Designsystem, Figma-Handoff, Frontend, visuelle QA, Tests, Fixes und Deployment-Bereitschaft.

![AstraFlow and Superpowers full-loop workflow](../assets/diagrams/astraflow-superpowers-loop.svg)

Viele KI-Coding-Projekte scheitern, weil die KI aus einem vagen Prompt bauen soll, ohne stabilen Produktkontext, Designregeln, Akzeptanzkriterien oder Quality Gates. AstraFlow gibt KI-Agenten ein strukturiertes Projektbetriebssystem.

## Warum AstraFlow

KI-Tools sind stark, werden aber oft wie ein Chat benutzt: "mach die Seite besser", "bau eine App", "generiere ein Design", "fix die UI", "deploye". Das reicht für Demos, aber nicht für echte Produkte.

AstraFlow gibt der KI Projektgedächtnis: Zweck, Nutzer, Workflows, Designregeln, wichtige Dateien, visuelle Qualität, Tests und Deployment-Erwartungen.

## Welche Probleme es löst

### 1. Vage Prompts erzeugen vage Produkte

AstraFlow ersetzt Einmal-Prompts durch `AGENTS.md`, `docs/02-prd.md`, `docs/03-design-system.md`, `docs/05-quality-gates.md` und wiederverwendbare Prompts.

### 2. KI-generierte UI wirkt oft wie eine Demo

AstraFlow fordert echte Workflows, realistische Daten, vollständige Zustände, responsive Layouts, keinen abgeschnittenen Text und keine chaotischen Überlappungen.

### 3. Design und Engineering driften auseinander

AstraFlow verbindet Product Brief, PRD, Designsystem, Bildgenerierung, Figma-Handoff, Frontend und visuelle Regression.

### 4. KI-Agenten verlieren Kontext

AstraFlow definiert Lesereihenfolge und Source of Truth vor Änderungen.

### 5. Shipping braucht mehr als Code

Tests, visuelle QA, Asset-Management, Deployment-Checklisten und Selbstentwicklung sind von Anfang an enthalten.

## AstraFlow vs Superpowers

[obra/superpowers](https://github.com/obra/superpowers) ist eine starke Softwareentwicklungsmethodik für Coding Agents. AstraFlow ist anders: ein KI-natives Produktliefersystem.

Superpowers verbessert, wie ein AI Coding Agent arbeitet. AstraFlow verbessert, wie ein AI-natives Produktprojekt von Idee zu Design, Figma, Frontend, QA und Deployment strukturiert wird.

Vergleich: [../docs/06-positioning-vs-superpowers.md](../docs/06-positioning-vs-superpowers.md)  
Integrationsloop: [../docs/08-full-loop-with-superpowers.md](../docs/08-full-loop-with-superpowers.md)

## Selbstentwicklung

AstraFlow verbessert sich mit der Zeit. Wiederholte Fehler werden zu stärkeren Prompts, klareren Anforderungen, strengeren Designregeln, besseren QA-Checks, Figma-Regeln, Asset-Grenzen, Tests oder Deployment-Checklisten.

Siehe: [../docs/07-self-evolution.md](../docs/07-self-evolution.md), [../docs/evolution/ledger.md](../docs/evolution/ledger.md)

## Vorteile

- AI-first Projektstruktur
- Workflow ohne perfekte Prompts
- Kommerzielle UI-Qualitätslatte
- Figma-ready Handoff
- Bild- und Asset-Pipeline
- Eingebaute Quality Gates
- Stack-unabhängig
- Agent-lesbare Source of Truth
- Nutzbar als Template, Bootstrap, CLI-Grundlage oder Codex skill/plugin Basis

## Für wen

Indie Hacker, Gründer, Design Engineers, Produktteams, Agenturen, Entwickler und Teams, die Figma, Screenshots und Produktideen in echte Software verwandeln.

## So funktioniert es

```text
1. Produktkontext erfassen
2. PRD erstellen oder verfeinern
3. KI schlägt 3 Designrichtungen vor
4. Richtung wählen
5. Designsystem erstellen
6. Visuelle Referenzen generieren
7. Figma-Handoff vorbereiten
8. Echte Frontend-Screens implementieren
9. Visuelle QA auf Desktop, Tablet, Mobile
10. Testen, fixen, deployen
```

## Repository-Struktur

Siehe [../README.md#repository-structure](../README.md#repository-structure).

## Schnellstart

1. Repository klonen oder kopieren.
2. `docs/00-project-context.md` ausfüllen.
3. `docs/01-product-brief.md` ausfüllen.
4. KI-Agent bitten:

```text
Read AGENTS.md and the docs folder.
Use AstraFlow's workflow to turn this product idea into a PRD, 3 design directions, a design system, implementation plan, visual QA plan, and deployment checklist.
If anything is unclear, give me 3 options instead of asking me to write a perfect prompt.
```

5. Designrichtung wählen.
6. Mit Implementierung und QA fortfahren.

### Codex App

Repository in Codex App öffnen und `AGENTS.md` lesen lassen.

### Codex CLI

Codex im Repository-Root starten und mit dem Core Prompt beginnen.

### Claude Code

Repository in Claude Code öffnen und `AGENTS.md` befolgen lassen.

### Cursor

Cursor Agent `AGENTS.md` und `docs/` lesen lassen.

### Gemini CLI

Gemini CLI im Root starten und AstraFlow folgen lassen.

### GitHub Copilot CLI

Repository-Dateien als Source of Truth für Pläne und Änderungen nutzen.

### Kimi Code

In Kimi Code die AstraFlow-Lesereihenfolge nutzen.

### OpenCode

OpenCode im Root starten und mit dem Core Prompt beginnen.

### Figma

`figma/figma-handoff.md` und `prompts/figma-generation.md` nutzen.

### Superpowers Integration

AstraFlow definiert, was gut ist; Superpowers führt Engineering diszipliniert aus.

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

## Eingebaute Quality Gates

- Product gate
- Design gate
- Figma gate
- Frontend gate
- Visual QA gate
- Test gate
- Deployment gate

## Sprachen

Siehe [README.md](README.md).

## Roadmap

- AstraFlow CLI
- Codex skill/plugin package
- Figma generation helpers
- Visual QA automation templates
- Example projects
- Multi-agent workflow templates

## License

Apache-2.0

