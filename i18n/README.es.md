# AstraFlow

[Volver al README principal](../README.md)

**Blueprint de flujo de trabajo nativo para IA que convierte ideas iniciales en software diseñado, probado y desplegable.**

`idea -> PRD -> design direction -> design system -> AI visuals -> Figma handoff -> frontend -> visual QA -> tests -> fixes -> deployment`

## Quickstart

Dale AstraFlow a tu proyecto:
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

Empieza con el [Core Prompt](#the-core-prompt), y deja que AstraFlow convierta tu idea en PRD, sistema de diseño, handoff para Figma, frontend, QA visual, pruebas, correcciones y preparación para despliegue.

![AstraFlow and Superpowers full-loop workflow](../assets/diagrams/astraflow-superpowers-loop.svg)

Muchos proyectos de IA fallan porque se pide construir desde un prompt vago, sin contexto estable de producto, reglas de diseño, criterios de aceptación ni puertas de calidad. AstraFlow proporciona un sistema operativo de proyecto para agentes de IA.

## Por qué AstraFlow

Las herramientas de IA son potentes, pero muchos equipos las usan como un chat: "mejora esta página", "crea una app", "genera un diseño", "corrige la UI", "despliégalo". Funciona para demos. Falla en productos reales.

AstraFlow da a la IA memoria de proyecto: propósito, usuarios, flujos, reglas de diseño, archivos importantes, calidad visual, pruebas y expectativas de despliegue.

## Problemas que resuelve

### 1. Prompts vagos crean productos vagos

AstraFlow reemplaza prompts aislados por `AGENTS.md`, `docs/02-prd.md`, `docs/03-design-system.md`, `docs/05-quality-gates.md` y prompts reutilizables.

### 2. La UI generada por IA suele parecer una demo

Promueve flujos reales, datos realistas, estados completos, layouts responsivos, sin texto cortado, sin superposiciones incoherentes y sin exceso de placeholders.

### 3. Diseño e ingeniería se separan

Conecta product brief, PRD, sistema de diseño, generación de imágenes, handoff Figma, implementación frontend y checks visuales.

### 4. Los agentes de IA pierden contexto

Define un orden de lectura y una fuente de verdad antes de modificar nada.

### 5. Enviar producto requiere más que código

Incluye pruebas, QA visual, gestión de assets, checklist de despliegue y autoevolución desde el inicio.

## AstraFlow vs Superpowers

[obra/superpowers](https://github.com/obra/superpowers) es una metodología sólida para coding agents. AstraFlow es diferente: es un sistema de entrega de producto nativo para IA.

Superpowers mejora cómo trabaja un AI coding agent. AstraFlow mejora cómo se estructura un producto AI-native desde idea hasta diseño, Figma, frontend, QA y despliegue.

Comparación: [../docs/06-positioning-vs-superpowers.md](../docs/06-positioning-vs-superpowers.md)  
Bucle de integración: [../docs/08-full-loop-with-superpowers.md](../docs/08-full-loop-with-superpowers.md)

## Autoevolución

AstraFlow mejora con el tiempo. Cada fallo repetido debe convertirse en prompts más fuertes, requisitos más claros, reglas de diseño más estrictas, QA visual, reglas Figma, restricciones de assets, pruebas o checklist de despliegue.

Lee: [../docs/07-self-evolution.md](../docs/07-self-evolution.md) y [../docs/evolution/ledger.md](../docs/evolution/ledger.md).

## Ventajas clave

- Estructura de proyecto AI-first
- Flujo sin prompts perfectos
- Estándar de UI comercial
- Handoff listo para Figma
- Pipeline de imágenes y assets
- Quality gates incorporados
- Independiente del stack
- Fuente de verdad legible por agentes
- Útil como plantilla, bootstrap, base CLI o base Codex skill/plugin

## Para quién es

Indie hackers, founders, design engineers, equipos de producto, agencias, developers y equipos que convierten Figma, screenshots e ideas en software real.

## Cómo funciona

```text
1. Capturar contexto de producto
2. Generar o refinar el PRD
3. Pedir a la IA 3 direcciones de diseño
4. Elegir una dirección
5. Crear un sistema de diseño
6. Generar referencias visuales o imágenes de producto
7. Preparar handoff Figma
8. Implementar pantallas frontend reales
9. Ejecutar QA visual en desktop, tablet y móvil
10. Probar, corregir y desplegar
```

## Estructura del repositorio

Consulta [../README.md#repository-structure](../README.md#repository-structure).

## Inicio rápido

1. Clona o copia este repositorio.
2. Completa `docs/00-project-context.md`.
3. Completa `docs/01-product-brief.md`.
4. Pide a tu agente de IA:

```text
Read AGENTS.md and the docs folder.
Use AstraFlow's workflow to turn this product idea into a PRD, 3 design directions, a design system, implementation plan, visual QA plan, and deployment checklist.
If anything is unclear, give me 3 options instead of asking me to write a perfect prompt.
```

5. Elige una dirección.
6. Continúa con implementación y QA.

### Codex App

Abre el repositorio en Codex App y pídele que lea `AGENTS.md` y use AstraFlow.

### Codex CLI

Ejecuta Codex desde la raíz y empieza con el core prompt.

### Claude Code

Abre el repositorio en Claude Code y pídele que siga `AGENTS.md`.

### Cursor

Abre el proyecto en Cursor Agent y pídele que lea `AGENTS.md` y `docs/`.

### Gemini CLI

Ejecuta Gemini CLI desde la raíz y pídele que siga AstraFlow.

### GitHub Copilot CLI

Usa los archivos del repositorio como fuente de verdad para planes y cambios.

### Kimi Code

Abre el proyecto en Kimi Code y sigue el orden de lectura de AstraFlow.

### OpenCode

Ejecuta OpenCode desde la raíz y empieza con el core prompt.

### Figma

Usa `figma/figma-handoff.md` y `prompts/figma-generation.md`.

### Superpowers Integration

Usa AstraFlow para definir qué significa "bueno" y Superpowers como motor de ejecución de ingeniería.

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

## Quality Gates incorporados

- Product gate
- Design gate
- Figma gate
- Frontend gate
- Visual QA gate
- Test gate
- Deployment gate

## Idiomas

Consulta [README.md](README.md).

## Roadmap

- AstraFlow CLI
- Codex skill/plugin package
- Figma generation helpers
- Visual QA automation templates
- Example projects
- Multi-agent workflow templates

## License

Apache-2.0

