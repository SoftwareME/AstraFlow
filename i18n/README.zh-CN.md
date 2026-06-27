# AstraFlow

[返回主 README](../README.md)

**AI 原生项目工作流蓝图：把粗略想法转化为完成设计、测试并可部署的软件。**

`想法 -> PRD -> 设计方向 -> 设计系统 -> AI 视觉 -> Figma 交付 -> 前端 -> 视觉 QA -> 测试 -> 修复 -> 部署`

## 快速开始

把 AstraFlow 交给你的项目：
[Codex App](#codex-app),
[Codex CLI](#codex-cli),
[Claude Code](#claude-code),
[Cursor](#cursor),
[Gemini CLI](#gemini-cli),
[GitHub Copilot CLI](#github-copilot-cli),
[Kimi Code](#kimi-code),
[OpenCode](#opencode),
[Figma](#figma),
[Superpowers](#superpowers-integration)。

从[核心提示词](#核心提示词)开始，让 AstraFlow 把你的想法转成 PRD、设计系统、Figma 交付、前端实现、视觉 QA、测试、修复和部署准备。

![AstraFlow 与 Superpowers 全流程闭环](../assets/diagrams/astraflow-superpowers-loop.svg)

多数 AI 编程项目失败，是因为 AI 只拿到一个模糊提示词，却没有稳定的产品上下文、设计规则、验收标准和质量门禁。AstraFlow 给项目提供一套 AI 可读的操作系统。

## 为什么使用 AstraFlow

AI 工具很强，但很多团队仍然像聊天框一样使用它们：“让页面更好看”“做一个 App”“生成设计”“修 UI”“部署一下”。这适合 demo，不适合真实产品。

AstraFlow 给 AI 补上项目记忆：产品目标、用户、工作流、设计规则、关键文件、视觉质量、测试和部署要求。

## 解决什么痛点

### 1. 模糊提示词产生模糊产品

AstraFlow 用 `AGENTS.md`、`docs/02-prd.md`、`docs/03-design-system.md`、`docs/05-quality-gates.md` 和可复用 prompts 替代一次性提示词。

### 2. AI 生成的 UI 经常像 demo

AstraFlow 要求真实工作流、真实数据、完整状态、响应式布局、无裁切、无混乱重叠、少占位符。

### 3. 设计和工程容易脱节

AstraFlow 连接 Product Brief、PRD、设计系统、图片生成、Figma 交付、前端实现和视觉回归检查。

### 4. AI 代理容易丢上下文

AstraFlow 给每个 AI 代理明确的读取顺序和事实来源。

### 5. 交付不只是写代码

AstraFlow 从一开始就包含测试、视觉 QA、资产管理、部署清单和自我进化机制。

## AstraFlow vs Superpowers

[obra/superpowers](https://github.com/obra/superpowers) 是很强的 coding agent 软件工程方法论。AstraFlow 不同：它是 AI 原生产品交付系统。

Superpowers 改善 AI coding agent 如何工作。AstraFlow 改善 AI 原生产品项目如何从想法走到设计、Figma、前端、QA 和部署。

两者可以一起用：Superpowers 负责工程纪律，AstraFlow 负责产品、设计、视觉 QA、资产、Figma 交付和部署结构。

完整对比：[../docs/06-positioning-vs-superpowers.md](../docs/06-positioning-vs-superpowers.md)  
集成闭环：[../docs/08-full-loop-with-superpowers.md](../docs/08-full-loop-with-superpowers.md)

## 自我进化

AstraFlow 会随着项目失败、反馈和复盘持续进化。重复问题应该沉淀成更强提示词、更清晰需求、更严格设计规则、更好的视觉 QA、Figma 规则、资产约束、测试或部署清单。

查看：[../docs/07-self-evolution.md](../docs/07-self-evolution.md) 和 [../docs/evolution/ledger.md](../docs/evolution/ledger.md)。

## 核心优势

- AI 优先的项目结构
- 用户选方案，不必写完美提示词
- 商业级 UI 质量标准
- Figma-ready 交付
- 图片生成与资产管线
- 内置质量门禁
- 技术栈无关
- AI 可读的项目事实来源
- 可作为文档模板、项目骨架、CLI 基础或 Codex skill/plugin 基础

## 适合谁

独立开发者、创业者、设计工程师、产品团队、外包/咨询团队、开发者，以及希望把 Figma、截图、产品想法变成真实软件的团队。

## 工作方式

```text
1. 捕获产品上下文
2. 生成或完善 PRD
3. 让 AI 提供 3 个设计方向
4. 选择一个方向
5. 创建设计系统
6. 生成视觉参考或产品图
7. 准备 Figma 交付
8. 实现真实前端页面
9. 在桌面、平板、移动端做视觉 QA
10. 运行测试、修复问题并部署
```

## 仓库结构

查看主 README 的结构说明：[../README.md#repository-structure](../README.md#repository-structure)。

## 开始使用

1. 克隆或复制本仓库。
2. 填写 `docs/00-project-context.md`。
3. 填写 `docs/01-product-brief.md`。
4. 让 AI 代理执行：

```text
Read AGENTS.md and the docs folder.
Use AstraFlow's workflow to turn this product idea into a PRD, 3 design directions, a design system, implementation plan, visual QA plan, and deployment checklist.
If anything is unclear, give me 3 options instead of asking me to write a perfect prompt.
```

5. 选择一个设计方向。
6. 让 AI 继续完成实现和 QA。

### Codex App

在 Codex App 中打开仓库，让它读取 `AGENTS.md` 并使用 AstraFlow。

### Codex CLI

在仓库根目录运行 Codex，并从下方核心提示词开始。

### Claude Code

在 Claude Code 中打开仓库，并要求它遵循 `AGENTS.md`。

### Cursor

在 Cursor Agent 中打开仓库，要求它先读 `AGENTS.md` 和 `docs/`。

### Gemini CLI

在仓库根目录运行 Gemini CLI，并要求它遵循 AstraFlow 工作流。

### GitHub Copilot CLI

把仓库文件作为事实来源，让 Copilot CLI 基于 PRD 和设计系统生成计划或代码修改。

### Kimi Code

在 Kimi Code 中打开项目，并遵循 AstraFlow 读取顺序。

### OpenCode

在仓库根目录运行 OpenCode，并使用核心提示词开始。

### Figma

使用 `figma/figma-handoff.md` 和 `prompts/figma-generation.md`。

### Superpowers Integration

用 AstraFlow 定义什么是好，再用 Superpowers 作为工程执行引擎。

## 核心提示词

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

## 内置质量门禁

- 产品门禁
- 设计门禁
- Figma 门禁
- 前端门禁
- 视觉 QA 门禁
- 测试门禁
- 部署门禁

## 语言

查看 [README.md](README.md)。

## 路线图

- AstraFlow CLI
- Codex skill/plugin 包
- Figma 生成辅助工具
- 视觉 QA 自动化模板
- 示例项目
- 多代理工作流模板

## License

Apache-2.0

