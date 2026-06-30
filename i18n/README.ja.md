# Awesome Cloudflare AI

> Cloudflare にデプロイ可能な AI、Agent、MCP、Workers AI、D1、R2、Vectorize、Durable Objects の厳選オープンソースプロジェクト集。

言語: [English](../README.md) | [简体中文](README.zh-CN.md) | [Português do Brasil](README.pt-BR.md) | [日本語](README.ja.md) | [Deutsch](README.de.md) | [Русский](README.ru.md)

Cloudflare AI / Agent / MCP に関する厳選オープンソースディレクトリです。汎用 AI ツール一覧ではなく、Cloudflare でのデプロイ、ランタイム、データ基盤と明確な関係があるプロジェクトだけを掲載します。

最終確認日: 2026-06-30

## このリストについて

Cloudflare Workers、Pages、D1、KV、R2、Vectorize、Durable Objects、Workers AI、AI Gateway、Queues は、低コストな AI アプリや Agent の重要な構成要素になりつつあります。このリストは次の 3 点を重視します。

- デプロイ可能: Cloudflare 上で動作する、または中核アーキテクチャが Cloudflare に明確に依存している。
- 検証可能: README、設定ファイル、サンプル、ドキュメントから用途とデプロイ方法を判断できる。
- メンテナンス中: 最近のメンテナンスが確認できるプロジェクトを優先する。

## 凡例

| 項目 | 値 |
|---|---|
| Deploy | Easy = ワンクリックデプロイまたは明確なコマンド；Medium = 複数サービス/API key が必要；Hard = アーキテクチャ理解やコード変更が必要 |
| Status | Active = 直近 6 か月に明確なメンテナンスあり；Stable = 更新は少ないが有用；Use with care = セキュリティ、コンプライアンス、プライバシー、悪用リスクあり |
| Risk | Low = 一般的なアプリ/テンプレート；Medium = ユーザーデータ、API key、ファイル、アカウント、自動化を扱う；High = proxy、匿名性、制限回避、クローリングなど |

## 評価方法

掲載前にプロジェクトをスコアリングします。Stars は弱いシグナルにすぎません。新しいプロジェクトでも、Cloudflare との関連性、デプロイ可能性、ドキュメント、安全性が十分なら掲載できます。

| 領域 | 点数 | 確認内容 |
|---|---:|---|
| Cloudflare 関連性 | 0-3 | Workers、Pages、Workers AI、AI Gateway、D1、KV、R2、Vectorize、Durable Objects、Queues、Email Routing、Turnstile、Cloudflare APIs の直接利用。 |
| デプロイ可能性 | 0-2 | 明確な deploy path、wrangler config、template、demo、setup instructions。 |
| メンテナンス | 0-2 | 最近の commits、releases、issue replies、または community use。 |
| ドキュメントとライセンス | 0-2 | 明確な README、environment variables、architecture notes、監査可能な license。 |
| 安全性 | 0-1 | auth、user data、uploads、automation、proxies、email、privileged APIs に対する妥当な境界。 |

掲載目安: 8-10 = 推奨、6-7 = 注意付きで可、4-5 = Use with care または再審査、4 未満 = 削除または掲載しない。高リスクプロジェクトにはより高いスコアと明確な安全メモが必要です。

## 目次

- [公式・コア](#公式コア)
- [Cloudflare 上の AI アプリ](#cloudflare-上の-ai-アプリ)
- [Workers 上の Agent](#workers-上の-agent)
- [Cloudflare 上の MCP](#cloudflare-上の-mcp)
- [ストレージとメモリ](#ストレージとメモリ)
- [テンプレートとスターター](#テンプレートとスターター)
- [可観測性と運用](#可観測性と運用)
- [注意して使うもの](#注意して使うもの)
- [評価方法](#評価方法)
- [選定基準](#選定基準)
- [コントリビューション](#コントリビューション)

## 公式・コア

| プロジェクト | 内容 | Cloudflare スタック | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [cloudflare/agents](https://github.com/cloudflare/agents) | AI Agent の構築とデプロイのための公式 SDK。 | Workers, Durable Objects, Workflows | Medium | Active | Low |
| [cloudflare/ai](https://github.com/cloudflare/ai) | 公式 Workers AI サンプル、デモ、パッケージ。 | Workers AI, Workers | Easy | Active | Low |
| [cloudflare/mcp-server-cloudflare](https://github.com/cloudflare/mcp-server-cloudflare) | Cloudflare アカウントリソース向け公式 MCP サーバー。 | MCP, Workers/KV/R2/DNS APIs | Medium | Active | Medium |
| [cloudflare/templates](https://github.com/cloudflare/templates) | Workers 向け公式テンプレート、アプリ/API スターター。 | Workers, Pages, D1, KV, R2 | Easy | Active | Low |
| [cloudflare/workers-chat-demo](https://github.com/cloudflare/workers-chat-demo) | Edge ネイティブなリアルタイムチャット公式デモ。 | Workers, Durable Objects | Medium | Active | Medium |
| [cloudflare/workers-sdk](https://github.com/cloudflare/workers-sdk) | Wrangler と Workers 開発ツールチェーン。 | Workers, Wrangler | Medium | Active | Low |

## Cloudflare 上の AI アプリ

| プロジェクト | 内容 | Cloudflare スタック | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [cloudflare/vibesdk](https://github.com/cloudflare/vibesdk) | Cloudflare スタックで構築されたオープンソース vibe coding プラットフォーム。 | Workers, Durable Objects | Medium | Active | Medium |
| [Jazee6/cloudflare-ai-web](https://github.com/Jazee6/cloudflare-ai-web) | ワンクリックデプロイ可能な Cloudflare AI Web プラットフォーム。 | Workers AI, Pages/Workers | Easy | Active | Medium |
| [miantiao-me/hacker-podcast](https://github.com/miantiao-me/hacker-podcast) | Hacker News から AI で中国語ポッドキャストを生成。 | Workers, Workflows | Medium | Active | Medium |
| [nicholasgriffintn/ai-platform](https://github.com/nicholasgriffintn/ai-platform) | マルチモデルの個人 AI アシスタントプラットフォーム。 | Workers, AI Gateway, Hono | Medium | Active | Medium |
| [unicornB/Supportly-Ai](https://github.com/unicornB/Supportly-Ai) | Cloudflare ネイティブな AI カスタマーサポート基盤。 | Workers, Workers AI, knowledge base | Medium | Active | Medium |
| [G4brym/workers-research](https://github.com/G4brym/workers-research) | Serverless な深掘り調査 Agent。 | Workers, Durable Objects | Medium | Active | Medium |
| [atinux/flux-ai-image-generator](https://github.com/atinux/flux-ai-image-generator) | Cloudflare 上の Flux を使う画像生成アプリ。 | Workers AI, R2, NuxtHub | Easy | Active | Medium |
| [chipmates/agoracosmica](https://github.com/chipmates/agoracosmica) | 教育向け AI 会話プラットフォーム。 | Workers, self-hosted app | Medium | Active | Medium |
| [devarshishimpi/codra](https://github.com/devarshishimpi/codra) | GitHub PR 向け self-hosted AI コードレビュー。 | Workers, KV, Queues, Hyperdrive, Workers AI | Medium | Active | Medium |
| [bestian/askit-hono](https://github.com/bestian/askit-hono) | Audrey Tang の文字起こしアーカイブを使う引用付き RAG QA。 | Workers, Hono, Vectorize, Workers AI | Medium | Active | Medium |
| [Teycir/ArxivExplorer](https://github.com/Teycir/ArxivExplorer) | arXiv 論文向け AI セマンティック検索。 | Workers, semantic search | Medium | Active | Medium |
| [IchimaruGin728/Gins-Blog](https://github.com/IchimaruGin728/Gins-Blog) | AI 検索と OAuth を備えた Edge ブログ。 | Workers, D1, R2, KV, Hono | Medium | Active | Medium |
| [arusso-aboutcloud/aboutcloud-search](https://github.com/arusso-aboutcloud/aboutcloud-search) | 明示的な安全ガードレールを備えた監査可能な RAG チャットボット。 | Workers AI, Vectorize, D1, Workers | Medium | Active | Medium |

## Workers 上の Agent

| プロジェクト | 内容 | Cloudflare スタック | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [openma-ai/open-managed-agents](https://github.com/openma-ai/open-managed-agents) | Claude Managed Agents API の self-hosted 実装。 | Workers, Durable Objects | Medium | Active | Medium |
| [Logos-Flux/cloudflare-multiagent](https://github.com/Logos-Flux/cloudflare-multiagent) | Workers 上のマルチ Agent AI プラットフォーム。 | Workers, AI generation | Medium | Active | Medium |
| [acoyfellow/flue-snippets](https://github.com/acoyfellow/flue-snippets) | デプロイテスト付きの実行可能な Flue Agent サンプル。 | Workers, Durable Objects, Workers AI | Easy | Active | Low |
| [stukennedy/honi](https://github.com/stukennedy/honi) | Cloudflare ネイティブな agentic AI フレームワーク。 | Durable Objects, Workers | Medium | Active | Medium |
| [acoyfellow/fleet-pattern](https://github.com/acoyfellow/fleet-pattern) | 階層型 Durable Object Agent パターン。 | Workers, Durable Objects | Medium | Stable | Low |
| [serpin-taxt/openchief](https://github.com/serpin-taxt/openchief) | 業務ツールを監視しレポートを生成する Agent。 | Workers, serverless runtime | Medium | Active | Medium |
| [huseynsnmz/postr](https://github.com/huseynsnmz/postr) | AI Agent 付き keyboard-first メール TUI。 | Workers, Durable Objects, Email Routing, Workers AI | Hard | Active | Medium |
| [Ahmad-A0/iris-voice-agent](https://github.com/Ahmad-A0/iris-voice-agent) | Edge 上のリアルタイム音声 Agent。 | Workers, Durable Objects | Hard | Active | Medium |
| [sinameraji/kimiflare](https://github.com/sinameraji/kimiflare) | Cloudflare アカウント上で動くターミナル型コーディング Agent。 | Workers AI, AI Gateway | Medium | Active | Medium |
| [marceloeatworld/clopinette-ai](https://github.com/marceloeatworld/clopinette-ai) | メモリと bot 連携を持つマルチモーダル AI Agent。 | Workers, Durable Objects, Workers AI, AutoRAG | Hard | Active | Medium |
| [acoyfellow/my-ax](https://github.com/acoyfellow/my-ax) | Cloudflare にセルフホストする個人向け AI agent 運用環境。 | Workers, Durable Objects, D1, MCP | Hard | Active | Medium |
| [yukthapriya/web-research-agent](https://github.com/yukthapriya/web-research-agent) | 計画、検索、引用付きレポート作成を行う Web research agent。 | Workers AI, Workflows, Durable Objects | Medium | Active | Medium |

## Cloudflare 上の MCP

| プロジェクト | 内容 | Cloudflare スタック | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [rahilp/second-brain-cloudflare](https://github.com/rahilp/second-brain-cloudflare) | MCP クライアント向け self-hosted AI メモリ層。 | Workers, D1, Vectorize | Medium | Active | Medium |
| [cyanheads/mcp-ts-core](https://github.com/cyanheads/mcp-ts-core) | Workers 対応の TypeScript MCP サーバーフレームワーク。 | Cloudflare Workers runtime | Medium | Active | Low |
| [Puliczek/mcp-memory](https://github.com/Puliczek/mcp-memory) | ユーザー設定と記憶を扱う MCP メモリサーバー。 | Workers, D1, Vectorize | Medium | Active | Medium |
| [Yrobot/cloudflare-search](https://github.com/Yrobot/cloudflare-search) | MCP で AI ツールを強化できる検索サーバー。 | Workers, MCP | Medium | Active | Medium |
| [stytchauth/mcp-stytch-consumer-todo-list](https://github.com/stytchauth/mcp-stytch-consumer-todo-list) | 認証例付き TODO アプリ MCP サーバー。 | Workers, MCP, Stytch | Medium | Active | Medium |
| [dinasaur404/BestReads-MCP-Server](https://github.com/dinasaur404/BestReads-MCP-Server) | Workers で構築されたリモート MCP サーバー。 | Workers, MCP | Medium | Active | Medium |
| [omarshahine/fastmail-mcp-remote](https://github.com/omarshahine/fastmail-mcp-remote) | Cloudflare Access OAuth を使う Fastmail リモート MCP。 | Workers, Access OAuth, MCP | Medium | Active | Medium |
| [miantiao-me/github-stars](https://github.com/miantiao-me/github-stars) | MCP 経由で GitHub starred repositories を自然言語検索。 | Workers, MCP, R2, AutoRAG | Medium | Active | Medium |

## ストレージとメモリ

| プロジェクト | 内容 | Cloudflare スタック | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [TimeSurgeLabs/athenadb](https://github.com/TimeSurgeLabs/athenadb) | Serverless なベクトルデータベース API。 | Workers, D1, Vectorize, Workers AI | Medium | Stable | Medium |
| [elizabethsiegle/art-vector-search-cloudflare](https://github.com/elizabethsiegle/art-vector-search-cloudflare) | Vectorize と Workers AI を使うアート検索。 | Vectorize, Workers AI, AI Gateway | Medium | Stable | Medium |
| [synapse-ai-labs/synapse-api](https://github.com/synapse-ai-labs/synapse-api) | Vectorize と OpenAI を使う Serverless embeddings API。 | Workers, D1, Vectorize | Medium | Stable | Medium |
| [adam0white/MessageAI](https://github.com/adam0white/MessageAI) | RAG と Agent を備えたリアルタイムメッセージアプリ。 | Workers, Durable Objects, Vectorize, Workers AI | Hard | Active | Medium |
| [realchendahuang/FlareMo](https://github.com/realchendahuang/FlareMo) | Memos API と MCP subset を備えた Cloudflare-native 個人知識システム。 | Workers, D1, R2, Access, MCP | Easy | Active | Medium |

## テンプレートとスターター

| プロジェクト | 内容 | Cloudflare スタック | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [louisbrulenaudet/genai-api](https://github.com/louisbrulenaudet/genai-api) | Workers + Gemini API テンプレート。 | Workers, AI Gateway, Hono | Easy | Active | Medium |
| [nuxt-hub/core](https://github.com/nuxt-hub/core) | Nuxt に DB、KV、blob storage、cache、AI 連携を追加。 | D1, KV, R2, Workers AI | Medium | Active | Low |
| [JSONbored/opennextjs-cli](https://github.com/JSONbored/opennextjs-cli) | Workers 上の OpenNext.js 向け CLI/TUI と MCP 機能。 | Workers, OpenNext, MCP | Medium | Active | Low |
| [acoyfellow/svelte-edge](https://github.com/acoyfellow/svelte-edge) | Agent 生成 Svelte UI を Workers でコンパイル。 | Workers, Hono, Workers AI | Medium | Active | Medium |
| [Geekgineer/needle-rs](https://github.com/Geekgineer/needle-rs) | tool-calling transformer 用の小型 WASM ランタイム。 | Workers, WASM | Hard | Active | Low |

## 可観測性と運用

| プロジェクト | 内容 | Cloudflare スタック | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [PoemMisty/CF-Request-Analytics-Panel](https://github.com/PoemMisty/CF-Request-Analytics-Panel) | 複数 Cloudflare アカウントのリクエスト分析パネル。 | Workers, analytics APIs | Medium | Active | Medium |
| [bgdnvk/clanker](https://github.com/bgdnvk/clanker) | クラウド環境向け自律システムエンジニアリング CLI Agent。 | Cloudflare support, Workers topics | Hard | Active | Medium |

## 注意して使うもの

これらは学習や self-hosting に役立つ可能性がありますが、匿名メッセージ、公開検索、メール、プロバイダー規約境界、特権アカウントアクセスなどの慎重な扱いが必要なパターンを含みます。デプロイ前にコード、権限、ログ、悪用対策、上流規約を確認してください。

| プロジェクト | 内容 | Cloudflare スタック | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [Vauth/duckgpt](https://github.com/Vauth/duckgpt) | Workers AI 風のモデルアクセスを使うチャットアプリ。 | Workers AI, Workers | Medium | Use with care | High |

## 選定基準

### 必須

- オープンソース、または中核コードを監査できる。
- Workers、Pages、Workers AI、AI Gateway、D1、KV、R2、Vectorize、Durable Objects、Queues、Email Routing、Turnstile、Cloudflare アカウント API と明確な関係がある。
- README または docs が用途と基本セットアップを説明している。
- 単なるマーケティングページではない。

### 優先

- 最近の commit、release、issue 返信、PR 活動がある。
- `wrangler` 設定、ワンクリックデプロイ、または Cloudflare への手順付きデプロイ docs がある。
- Demo、スクリーンショット、アーキテクチャメモ、テストがある。
- 環境変数、権限、コスト、セキュリティ注意点が明確。

### 掲載しないもの

- アイデアだけで実行可能コードがないリポジトリ。
- クローズドソースサービス。
- Cloudflare が単に言及されているだけのリポジトリ。
- 明確な悪用、bypass、認証情報窃取、ポリシー回避プロジェクト。
- 参考価値が明確でない archived または未メンテナンスのプロジェクト。

## コントリビューション

Pull request を歓迎します。プロジェクトを提案する前に [CONTRIBUTING.md](../CONTRIBUTING.md) を読んでください。

プロジェクト追加時は以下を含めてください。

- 何をするプロジェクトか。
- 使用する Cloudflare コンポーネント。
- デプロイ難易度。
- メンテナンス状況。
- リスクまたは安全上の注意。

## ライセンス

MIT。詳細は [LICENSE](../LICENSE) を参照してください。
