# AstraFlow

[메인 README로 돌아가기](../README.md)

**막연한 아이디어를 설계되고 테스트되며 배포 가능한 소프트웨어로 바꾸는 AI 네이티브 프로젝트 워크플로우 블루프린트입니다.**

`idea -> PRD -> design direction -> design system -> AI visuals -> Figma handoff -> frontend -> visual QA -> tests -> fixes -> deployment`

## Quickstart

프로젝트에 AstraFlow를 적용하세요:
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

[Core Prompt](#core-prompt)로 시작하면 AstraFlow가 아이디어를 PRD, 디자인 시스템, Figma 핸드오프, 프론트엔드 구현, 시각 QA, 테스트, 수정, 배포 준비로 연결합니다.

![AstraFlow and Superpowers full-loop workflow](../assets/diagrams/astraflow-superpowers-loop.svg)

대부분의 AI 코딩 프로젝트는 안정적인 제품 맥락, 디자인 규칙, 수용 기준, 품질 게이트 없이 모호한 프롬프트로 시작하기 때문에 실패합니다. AstraFlow는 AI 에이전트를 위한 구조화된 프로젝트 운영 체계를 제공합니다.

## 왜 AstraFlow인가

AI 도구는 강력하지만 많은 팀은 여전히 채팅처럼 사용합니다. “페이지를 개선해줘”, “앱을 만들어줘”, “디자인을 생성해줘”, “UI를 고쳐줘”, “배포해줘”. 데모에는 충분하지만 실제 제품에서는 깨집니다.

AstraFlow는 AI에 제품 목적, 사용자, 워크플로우, 디자인 규칙, 중요한 파일, 시각 품질, 테스트, 배포 기대치를 제공합니다.

## 해결하는 문제

### 1. 모호한 프롬프트는 모호한 제품을 만듭니다

AstraFlow는 일회성 프롬프트를 `AGENTS.md`, `docs/02-prd.md`, `docs/03-design-system.md`, `docs/05-quality-gates.md`, 재사용 가능한 prompts로 대체합니다.

### 2. AI 생성 UI는 데모처럼 보이기 쉽습니다

실제 워크플로우, 현실적인 데이터, 완전한 상태, 반응형 레이아웃, 잘리지 않는 텍스트, 겹침 없는 UI를 요구합니다.

### 3. 디자인과 엔지니어링이 어긋납니다

Product Brief, PRD, 디자인 시스템, 이미지 생성, Figma 핸드오프, 프론트엔드 구현, 시각 회귀 검사를 연결합니다.

### 4. AI 에이전트는 맥락을 잃습니다

변경 전 읽어야 할 순서와 source of truth를 제공합니다.

### 5. 출시에는 코드 이상이 필요합니다

테스트, 시각 QA, 자산 관리, 배포 체크리스트, 자기 진화를 처음부터 포함합니다.

## AstraFlow vs Superpowers

[obra/superpowers](https://github.com/obra/superpowers)는 coding agent를 위한 강력한 소프트웨어 개발 방법론입니다. AstraFlow는 AI 네이티브 제품 전달 시스템입니다.

Superpowers는 AI coding agent의 작업 방식을 개선합니다. AstraFlow는 제품 프로젝트가 아이디어에서 디자인, Figma, 프론트엔드, QA, 배포까지 구조화되도록 합니다.

비교: [../docs/06-positioning-vs-superpowers.md](../docs/06-positioning-vs-superpowers.md)  
통합 루프: [../docs/08-full-loop-with-superpowers.md](../docs/08-full-loop-with-superpowers.md)

## 자기 진화

반복되는 실패는 더 강한 프롬프트, 명확한 요구사항, 엄격한 디자인 규칙, QA 체크, Figma 규칙, 자산 제약, 테스트, 배포 체크리스트로 남겨야 합니다.

문서: [../docs/07-self-evolution.md](../docs/07-self-evolution.md), [../docs/evolution/ledger.md](../docs/evolution/ledger.md)

## 핵심 장점

- AI-first 프로젝트 구조
- 완벽한 프롬프트 대신 선택형 워크플로우
- 상용 수준 UI 품질 기준
- Figma-ready 핸드오프
- 이미지 생성 및 자산 파이프라인
- 내장 품질 게이트
- 스택 독립적
- AI가 읽을 수 있는 source of truth
- 문서 템플릿, bootstrap, CLI 기반, Codex skill/plugin 기반으로 사용 가능

## 대상 사용자

인디 해커, 창업자, 디자인 엔지니어, 제품팀, 에이전시, 개발자, Figma/스크린샷/아이디어를 실제 소프트웨어로 만들고 싶은 팀.

## 작동 방식

```text
1. 제품 맥락 기록
2. PRD 생성 또는 개선
3. AI가 3가지 디자인 방향 제안
4. 방향 선택
5. 디자인 시스템 생성
6. 시각 레퍼런스 또는 제품 이미지 생성
7. Figma 핸드오프 준비
8. 실제 프론트엔드 화면 구현
9. 데스크톱, 태블릿, 모바일 시각 QA
10. 테스트, 수정, 배포
```

## 저장소 구조

[../README.md#repository-structure](../README.md#repository-structure)를 참고하세요.

## 빠른 시작

1. 이 저장소를 clone 또는 copy합니다.
2. `docs/00-project-context.md`를 작성합니다.
3. `docs/01-product-brief.md`를 작성합니다.
4. AI coding agent에게 요청합니다:

```text
Read AGENTS.md and the docs folder.
Use AstraFlow's workflow to turn this product idea into a PRD, 3 design directions, a design system, implementation plan, visual QA plan, and deployment checklist.
If anything is unclear, give me 3 options instead of asking me to write a perfect prompt.
```

5. 디자인 방향을 선택합니다.
6. 구현과 QA를 진행합니다.

### Codex App

Codex App에서 저장소를 열고 `AGENTS.md`를 읽어 AstraFlow를 사용하도록 요청합니다.

### Codex CLI

저장소 루트에서 Codex를 실행하고 core prompt로 시작합니다.

### Claude Code

Claude Code에서 저장소를 열고 `AGENTS.md`를 따르게 합니다.

### Cursor

Cursor Agent에서 `AGENTS.md`와 `docs/`를 먼저 읽게 합니다.

### Gemini CLI

저장소 루트에서 Gemini CLI를 실행하고 AstraFlow 워크플로우를 따르게 합니다.

### GitHub Copilot CLI

저장소 파일을 source of truth로 사용하여 계획이나 구현 변경을 생성합니다.

### Kimi Code

Kimi Code에서 AstraFlow read order를 따릅니다.

### OpenCode

저장소 루트에서 OpenCode를 실행하고 core prompt로 시작합니다.

### Figma

`figma/figma-handoff.md`와 `prompts/figma-generation.md`를 사용합니다.

### Superpowers Integration

AstraFlow로 좋은 결과의 기준을 정의하고 Superpowers를 engineering execution engine으로 사용합니다.

## Core Prompt

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

## 내장 품질 게이트

- Product gate
- Design gate
- Figma gate
- Frontend gate
- Visual QA gate
- Test gate
- Deployment gate

## 언어

[README.md](README.md)를 참고하세요.

## 로드맵

- AstraFlow CLI
- Codex skill/plugin package
- Figma generation helpers
- Visual QA automation templates
- Example projects
- Multi-agent workflow templates

## License

Apache-2.0

