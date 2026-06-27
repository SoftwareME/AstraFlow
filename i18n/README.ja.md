# AstraFlow

[メイン README に戻る](../README.md)

**粗いアイデアを、設計済み・テスト済み・デプロイ可能なソフトウェアへ変換する AI ネイティブなプロジェクトワークフローブループリント。**

`idea -> PRD -> design direction -> design system -> AI visuals -> Figma handoff -> frontend -> visual QA -> tests -> fixes -> deployment`

## Quickstart

プロジェクトに AstraFlow を与える:
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

[コアプロンプト](#コアプロンプト)から始めると、AstraFlow がアイデアを PRD、デザインシステム、Figma ハンドオフ、フロントエンド実装、ビジュアル QA、テスト、修正、デプロイ準備へ導きます。

![AstraFlow and Superpowers full-loop workflow](../assets/diagrams/astraflow-superpowers-loop.svg)

多くの AI コーディングプロジェクトは、安定したプロダクト文脈、デザインルール、受け入れ基準、品質ゲートがないまま曖昧なプロンプトから始まるため失敗します。AstraFlow は AI エージェントのための構造化されたプロジェクト OS を提供します。

## なぜ AstraFlow を使うのか

AI ツールは強力ですが、多くのチームはまだチャットボックスのように使っています。「ページを良くして」「アプリを作って」「デザインを生成して」「UI を直して」「デプロイして」。これは demo には有効ですが、実プロダクトでは壊れます。

AstraFlow は AI に、プロダクト目的、ユーザー、ワークフロー、デザインルール、重要ファイル、視覚品質、テスト、デプロイ期待値を与えます。

## 解決する課題

### 1. 曖昧なプロンプトは曖昧なプロダクトを生む

AstraFlow は一回限りのプロンプトを `AGENTS.md`、`docs/02-prd.md`、`docs/03-design-system.md`、`docs/05-quality-gates.md`、再利用可能な prompts に置き換えます。

### 2. AI 生成 UI は demo っぽくなりがち

実ワークフロー、現実的なデータ、完全な状態、レスポンシブレイアウト、文字切れなし、重なりなし、placeholder 過多なしを重視します。

### 3. デザインとエンジニアリングがずれる

Product Brief、PRD、デザインシステム、画像生成、Figma ハンドオフ、フロントエンド実装、ビジュアル回帰を接続します。

### 4. AI エージェントが文脈を失う

変更前に読む順序と信頼できる情報源を明確にします。

### 5. 出荷にはコード以上が必要

テスト、ビジュアル QA、アセット管理、デプロイチェックリスト、自己進化を最初から含みます。

## AstraFlow vs Superpowers

[obra/superpowers](https://github.com/obra/superpowers) は coding agent のための強力なソフトウェア開発方法論です。AstraFlow は異なり、AI ネイティブなプロダクトデリバリーシステムです。

Superpowers は AI coding agent の働き方を改善します。AstraFlow は AI ネイティブなプロダクトプロジェクトを、アイデアからデザイン、Figma、フロントエンド、QA、デプロイまで構造化します。

比較: [../docs/06-positioning-vs-superpowers.md](../docs/06-positioning-vs-superpowers.md)  
統合ループ: [../docs/08-full-loop-with-superpowers.md](../docs/08-full-loop-with-superpowers.md)

## 自己進化

AstraFlow は時間とともに改善されます。反復する失敗は、より強いプロンプト、明確な要件、厳密なデザインルール、QA チェック、Figma ルール、アセット制約、テスト、デプロイ項目として残すべきです。

詳細: [../docs/07-self-evolution.md](../docs/07-self-evolution.md)、[../docs/evolution/ledger.md](../docs/evolution/ledger.md)

## 主な利点

- AI-first なプロジェクト構造
- 完璧なプロンプト不要の選択式ワークフロー
- 商用品質の UI 基準
- Figma-ready ハンドオフ
- 画像生成とアセットパイプライン
- 組み込み品質ゲート
- スタック非依存
- AI が読める信頼できる情報源
- ドキュメントテンプレート、bootstrap、CLI 基盤、Codex skill/plugin 基盤として利用可能

## 対象ユーザー

個人開発者、創業者、デザインエンジニア、プロダクトチーム、代理店、開発者、Figma・スクリーンショット・プロダクトアイデアを実ソフトウェアにしたいチーム。

## 仕組み

```text
1. プロダクト文脈を記録
2. PRD を生成または改善
3. AI に 3 つのデザイン方向を提案させる
4. 方向を選ぶ
5. デザインシステムを作成
6. ビジュアル参照や製品画像を生成
7. Figma ハンドオフを準備
8. 実際のフロントエンド画面を実装
9. デスクトップ・タブレット・モバイルでビジュアル QA
10. テスト、修正、デプロイ
```

## リポジトリ構造

[../README.md#repository-structure](../README.md#repository-structure) を参照してください。

## クイックスタート

1. このリポジトリを clone または copy。
2. `docs/00-project-context.md` を記入。
3. `docs/01-product-brief.md` を記入。
4. AI coding agent に依頼:

```text
Read AGENTS.md and the docs folder.
Use AstraFlow's workflow to turn this product idea into a PRD, 3 design directions, a design system, implementation plan, visual QA plan, and deployment checklist.
If anything is unclear, give me 3 options instead of asking me to write a perfect prompt.
```

5. デザイン方向を選択。
6. 実装と QA へ進める。

### Codex App

Codex App で開き、`AGENTS.md` を読んで AstraFlow を使うよう依頼します。

### Codex CLI

リポジトリルートで Codex を実行し、コアプロンプトから始めます。

### Claude Code

Claude Code で開き、`AGENTS.md` に従わせます。

### Cursor

Cursor Agent で `AGENTS.md` と `docs/` を先に読ませます。

### Gemini CLI

リポジトリルートで Gemini CLI を実行し、AstraFlow ワークフローに従わせます。

### GitHub Copilot CLI

リポジトリファイルを情報源として計画や実装変更を生成します。

### Kimi Code

Kimi Code で AstraFlow の read order に従います。

### OpenCode

リポジトリルートで OpenCode を実行し、コアプロンプトから開始します。

### Figma

`figma/figma-handoff.md` と `prompts/figma-generation.md` を使います。

### Superpowers Integration

AstraFlow で「何が良いか」を定義し、Superpowers を engineering execution engine として使います。

## コアプロンプト

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

## 組み込み品質ゲート

- Product gate
- Design gate
- Figma gate
- Frontend gate
- Visual QA gate
- Test gate
- Deployment gate

## 言語

[README.md](README.md) を参照してください。

## ロードマップ

- AstraFlow CLI
- Codex skill/plugin package
- Figma generation helpers
- Visual QA automation templates
- Example projects
- Multi-agent workflow templates

## License

Apache-2.0

