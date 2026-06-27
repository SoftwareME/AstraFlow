# AstraFlow

[Retour au README principal](../README.md)

**Blueprint de workflow natif pour l'IA qui transforme des idées brutes en logiciel conçu, testé et déployable.**

`idea -> PRD -> design direction -> design system -> AI visuals -> Figma handoff -> frontend -> visual QA -> tests -> fixes -> deployment`

## Quickstart

Donnez AstraFlow à votre projet:
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

Commencez avec le [Core Prompt](#the-core-prompt), puis laissez AstraFlow transformer votre idée en PRD, système de design, handoff Figma, frontend, QA visuelle, tests, corrections et préparation au déploiement.

![AstraFlow and Superpowers full-loop workflow](../assets/diagrams/astraflow-superpowers-loop.svg)

Beaucoup de projets IA échouent parce que l'IA doit construire à partir d'un prompt vague, sans contexte produit stable, règles de design, critères d'acceptation ni quality gates. AstraFlow fournit un système d'exploitation de projet pour agents IA.

## Pourquoi AstraFlow

Les outils IA sont puissants, mais beaucoup d'équipes les utilisent comme un chat: "améliore cette page", "crée une app", "génère un design", "corrige l'UI", "déploie". Cela marche pour les démos, pas pour les vrais produits.

AstraFlow donne à l'IA une mémoire de projet: objectif, utilisateurs, workflows, règles de design, fichiers importants, qualité visuelle, tests et attentes de déploiement.

## Problèmes résolus

### 1. Les prompts vagues créent des produits vagues

AstraFlow remplace les prompts ponctuels par `AGENTS.md`, `docs/02-prd.md`, `docs/03-design-system.md`, `docs/05-quality-gates.md` et des prompts réutilisables.

### 2. Les UI générées par IA ressemblent souvent à des démos

Il impose de vrais workflows, des données réalistes, des états complets, des layouts responsives, pas de texte coupé, pas de chevauchement incohérent.

### 3. Le design et l'ingénierie divergent

AstraFlow relie product brief, PRD, système de design, génération d'images, handoff Figma, frontend et checks visuels.

### 4. Les agents IA perdent le contexte

Il donne un ordre de lecture et une source de vérité avant tout changement.

### 5. Livrer demande plus que du code

Il inclut tests, QA visuelle, gestion d'assets, checklist de déploiement et auto-évolution.

## AstraFlow vs Superpowers

[obra/superpowers](https://github.com/obra/superpowers) est une solide méthodologie de développement pour coding agents. AstraFlow est différent: c'est un système de livraison produit natif pour l'IA.

Superpowers améliore la façon dont un AI coding agent travaille. AstraFlow structure un projet produit AI-native de l'idée au design, Figma, frontend, QA et déploiement.

Comparaison: [../docs/06-positioning-vs-superpowers.md](../docs/06-positioning-vs-superpowers.md)  
Boucle d'intégration: [../docs/08-full-loop-with-superpowers.md](../docs/08-full-loop-with-superpowers.md)

## Auto-évolution

AstraFlow s'améliore avec le temps. Chaque échec répété doit devenir un prompt plus fort, une exigence plus claire, une règle de design, un check QA, une règle Figma, une contrainte d'asset, un test ou une checklist de déploiement.

Lire: [../docs/07-self-evolution.md](../docs/07-self-evolution.md) et [../docs/evolution/ledger.md](../docs/evolution/ledger.md).

## Avantages clés

- Structure de projet AI-first
- Workflow sans prompts parfaits
- Niveau de qualité UI commercial
- Handoff prêt pour Figma
- Pipeline d'images et d'assets
- Quality gates intégrés
- Indépendant du stack
- Source de vérité lisible par agents
- Utilisable comme template, bootstrap, base CLI ou base Codex skill/plugin

## Pour qui

Indie hackers, fondateurs, design engineers, équipes produit, agences, développeurs et équipes transformant Figma, captures et idées en logiciels réels.

## Fonctionnement

```text
1. Capturer le contexte produit
2. Générer ou affiner le PRD
3. Demander 3 directions de design à l'IA
4. Choisir une direction
5. Créer un système de design
6. Générer des références visuelles
7. Préparer le handoff Figma
8. Implémenter de vrais écrans frontend
9. Lancer la QA visuelle desktop, tablette, mobile
10. Tester, corriger et déployer
```

## Structure du dépôt

Voir [../README.md#repository-structure](../README.md#repository-structure).

## Démarrage rapide

1. Clonez ou copiez ce dépôt.
2. Remplissez `docs/00-project-context.md`.
3. Remplissez `docs/01-product-brief.md`.
4. Demandez à votre agent IA:

```text
Read AGENTS.md and the docs folder.
Use AstraFlow's workflow to turn this product idea into a PRD, 3 design directions, a design system, implementation plan, visual QA plan, and deployment checklist.
If anything is unclear, give me 3 options instead of asking me to write a perfect prompt.
```

5. Choisissez une direction.
6. Continuez vers l'implémentation et la QA.

### Codex App

Ouvrez ce dépôt dans Codex App et demandez-lui de lire `AGENTS.md`.

### Codex CLI

Lancez Codex depuis la racine et commencez par le core prompt.

### Claude Code

Ouvrez le dépôt dans Claude Code et demandez-lui de suivre `AGENTS.md`.

### Cursor

Ouvrez le dépôt dans Cursor Agent et demandez-lui de lire `AGENTS.md` et `docs/`.

### Gemini CLI

Lancez Gemini CLI depuis la racine et demandez-lui de suivre AstraFlow.

### GitHub Copilot CLI

Utilisez les fichiers du dépôt comme source de vérité pour les plans et changements.

### Kimi Code

Ouvrez le projet dans Kimi Code et suivez l'ordre de lecture AstraFlow.

### OpenCode

Lancez OpenCode depuis la racine et commencez par le core prompt.

### Figma

Utilisez `figma/figma-handoff.md` et `prompts/figma-generation.md`.

### Superpowers Integration

Utilisez AstraFlow pour définir ce qui est bon, puis Superpowers comme moteur d'exécution engineering.

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

## Quality Gates intégrés

- Product gate
- Design gate
- Figma gate
- Frontend gate
- Visual QA gate
- Test gate
- Deployment gate

## Langues

Voir [README.md](README.md).

## Roadmap

- AstraFlow CLI
- Codex skill/plugin package
- Figma generation helpers
- Visual QA automation templates
- Example projects
- Multi-agent workflow templates

## License

Apache-2.0

