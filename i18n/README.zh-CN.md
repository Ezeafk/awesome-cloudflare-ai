# Awesome Cloudflare AI

> 精选可部署在 Cloudflare 上的开源 AI、Agent、MCP、Workers AI、D1、R2、Vectorize 和 Durable Objects 项目。

语言：[English](../README.md) | [简体中文](README.zh-CN.md) | [Português do Brasil](README.pt-BR.md) | [日本語](README.ja.md) | [Deutsch](README.de.md) | [Русский](README.ru.md)

一个严格筛选的 Cloudflare AI / Agent / MCP 开源项目导航。这里不是泛 AI 工具大全，只收录与 Cloudflare 部署、运行时或数据基础设施有明确关系的项目。

最后审核：2026-06-26

## 为什么做这个列表

Cloudflare Workers、Pages、D1、KV、R2、Vectorize、Durable Objects、Workers AI、AI Gateway 和 Queues 正在成为低成本 AI 应用与 Agent 的重要基础设施。本项目关注三点：

- 可部署：项目能运行在 Cloudflare 上，或核心架构明显依赖 Cloudflare。
- 可验证：README、配置文件、示例或文档足以判断用途和部署方式。
- 有维护：优先收录近期仍有维护迹象的项目。

## 标记说明

| 字段 | 含义 |
|---|---|
| 部署 | Easy = 一键部署或清晰命令；Medium = 需要多个服务/API key；Hard = 需要理解架构或修改代码 |
| 状态 | Active = 最近 6 个月有明显维护；Stable = 更新较少但仍有参考价值；Use with care = 存在安全、合规、隐私或滥用风险 |
| 风险 | Low = 普通应用/模板；Medium = 涉及用户数据、API key、文件、账号或自动化；High = 代理、匿名、绕限制、爬虫等敏感用途 |

## 目录

- [官方与核心项目](#官方与核心项目)
- [Cloudflare 上的 AI 应用](#cloudflare-上的-ai-应用)
- [Workers 上的 Agent](#workers-上的-agent)
- [Cloudflare 上的 MCP](#cloudflare-上的-mcp)
- [存储与记忆](#存储与记忆)
- [模板与脚手架](#模板与脚手架)
- [可观测性与运维](#可观测性与运维)
- [谨慎使用](#谨慎使用)
- [收录标准](#收录标准)
- [贡献](#贡献)

## 官方与核心项目

| 项目 | 用途 | Cloudflare 技术栈 | 部署 | 状态 | 风险 |
|---|---|---|---|---|---|
| [cloudflare/agents](https://github.com/cloudflare/agents) | 用于构建和部署 AI Agent 的官方 SDK。 | Workers, Durable Objects, Workflows | Medium | Active | Low |
| [cloudflare/ai](https://github.com/cloudflare/ai) | 官方 Workers AI 示例、演示和包。 | Workers AI, Workers | Easy | Active | Low |
| [cloudflare/mcp-server-cloudflare](https://github.com/cloudflare/mcp-server-cloudflare) | 面向 Cloudflare 账号资源的官方 MCP 服务器。 | MCP, Workers/KV/R2/DNS APIs | Medium | Active | Medium |
| [cloudflare/templates](https://github.com/cloudflare/templates) | 官方 Workers 模板，包含应用和 API starter。 | Workers, Pages, D1, KV, R2 | Easy | Active | Low |
| [cloudflare/workers-chat-demo](https://github.com/cloudflare/workers-chat-demo) | 官方边缘实时聊天演示。 | Workers, Durable Objects | Medium | Active | Medium |
| [cloudflare/workers-sdk](https://github.com/cloudflare/workers-sdk) | Wrangler 和 Workers 开发工具链。 | Workers, Wrangler | Medium | Active | Low |

## Cloudflare 上的 AI 应用

| 项目 | 用途 | Cloudflare 技术栈 | 部署 | 状态 | 风险 |
|---|---|---|---|---|---|
| [cloudflare/vibesdk](https://github.com/cloudflare/vibesdk) | 基于 Cloudflare 构建的开源 vibe coding 平台。 | Workers, Durable Objects | Medium | Active | Medium |
| [Jazee6/cloudflare-ai-web](https://github.com/Jazee6/cloudflare-ai-web) | 可一键部署的 Cloudflare AI Web 平台。 | Workers AI, Pages/Workers | Easy | Active | Medium |
| [miantiao-me/hacker-podcast](https://github.com/miantiao-me/hacker-podcast) | 从 Hacker News 自动生成中文 AI 播客。 | Workers, Workflows | Medium | Active | Medium |
| [nicholasgriffintn/ai-platform](https://github.com/nicholasgriffintn/ai-platform) | 多模型个人 AI 助手平台。 | Workers, AI Gateway, Hono | Medium | Active | Medium |
| [unicornB/Supportly-Ai](https://github.com/unicornB/Supportly-Ai) | Cloudflare 原生 AI 客服平台。 | Workers, Workers AI, knowledge base | Medium | Active | Medium |
| [G4brym/workers-research](https://github.com/G4brym/workers-research) | Serverless 深度研究 Agent。 | Workers, Durable Objects | Medium | Active | Medium |
| [atinux/flux-ai-image-generator](https://github.com/atinux/flux-ai-image-generator) | 使用 Cloudflare 上的 Flux 生成图片。 | Workers AI, R2, NuxtHub | Easy | Active | Medium |
| [chipmates/agoracosmica](https://github.com/chipmates/agoracosmica) | 教育类 AI 对话平台。 | Workers, self-hosted app | Medium | Active | Medium |
| [devarshishimpi/codra](https://github.com/devarshishimpi/codra) | 自托管 GitHub PR AI 代码评审。 | Workers, KV, Queues, Hyperdrive, Workers AI | Medium | Active | Medium |
| [bestian/askit-hono](https://github.com/bestian/askit-hono) | 基于唐凤逐字稿档案的带引用 RAG 问答。 | Workers, Hono, Vectorize, Workers AI | Medium | Active | Medium |
| [Teycir/ArxivExplorer](https://github.com/Teycir/ArxivExplorer) | 面向 arXiv 论文的 AI 语义搜索。 | Workers, semantic search | Medium | Active | Medium |
| [IchimaruGin728/Gins-Blog](https://github.com/IchimaruGin728/Gins-Blog) | 带 AI 搜索和 OAuth 的边缘博客。 | Workers, D1, R2, KV, Hono | Medium | Active | Medium |

## Workers 上的 Agent

| 项目 | 用途 | Cloudflare 技术栈 | 部署 | 状态 | 风险 |
|---|---|---|---|---|---|
| [openma-ai/open-managed-agents](https://github.com/openma-ai/open-managed-agents) | Claude Managed Agents API 的自托管实现。 | Workers, Durable Objects | Medium | Active | Medium |
| [Logos-Flux/cloudflare-multiagent](https://github.com/Logos-Flux/cloudflare-multiagent) | Workers 上的多 Agent AI 平台。 | Workers, AI generation | Medium | Active | Medium |
| [acoyfellow/flue-snippets](https://github.com/acoyfellow/flue-snippets) | 可运行的 Flue Agent 示例，并带部署测试。 | Workers, Durable Objects, Workers AI | Easy | Active | Low |
| [stukennedy/honi](https://github.com/stukennedy/honi) | Cloudflare 原生 Agentic AI 框架。 | Durable Objects, Workers | Medium | Active | Medium |
| [acoyfellow/fleet-pattern](https://github.com/acoyfellow/fleet-pattern) | 分层 Durable Object Agent 模式演示。 | Workers, Durable Objects | Medium | Stable | Low |
| [serpin-taxt/openchief](https://github.com/serpin-taxt/openchief) | 观察业务工具并生成报告的 Agent。 | Workers, serverless runtime | Medium | Active | Medium |
| [huseynsnmz/postr](https://github.com/huseynsnmz/postr) | 带 AI Agent 的键盘优先邮件 TUI。 | Workers, Durable Objects, Email Routing, Workers AI | Hard | Active | Medium |
| [Ahmad-A0/iris-voice-agent](https://github.com/Ahmad-A0/iris-voice-agent) | 边缘实时语音 Agent。 | Workers, Durable Objects | Hard | Active | Medium |
| [sinameraji/kimiflare](https://github.com/sinameraji/kimiflare) | 运行在 Cloudflare 上的终端编码 Agent。 | Workers AI, AI Gateway | Medium | Active | Medium |
| [marceloeatworld/clopinette-ai](https://github.com/marceloeatworld/clopinette-ai) | 带记忆和机器人集成的多模态 AI Agent。 | Workers, Durable Objects, Workers AI, AutoRAG | Hard | Active | Medium |

## Cloudflare 上的 MCP

| 项目 | 用途 | Cloudflare 技术栈 | 部署 | 状态 | 风险 |
|---|---|---|---|---|---|
| [rahilp/second-brain-cloudflare](https://github.com/rahilp/second-brain-cloudflare) | 面向 MCP 客户端的自托管 AI 记忆层。 | Workers, D1, Vectorize | Medium | Active | Medium |
| [cyanheads/mcp-ts-core](https://github.com/cyanheads/mcp-ts-core) | 支持 Workers 的 TypeScript MCP 服务器框架。 | Cloudflare Workers runtime | Medium | Active | Low |
| [Puliczek/mcp-memory](https://github.com/Puliczek/mcp-memory) | 用于用户偏好和记忆召回的 MCP 记忆服务器。 | Workers, D1, Vectorize | Medium | Active | Medium |
| [Yrobot/cloudflare-search](https://github.com/Yrobot/cloudflare-search) | 可通过 MCP 增强 AI 工具的搜索服务器。 | Workers, MCP | Medium | Active | Medium |
| [stytchauth/mcp-stytch-consumer-todo-list](https://github.com/stytchauth/mcp-stytch-consumer-todo-list) | 带认证示例的 TODO App MCP 服务器。 | Workers, MCP, Stytch | Medium | Active | Medium |
| [dinasaur404/BestReads-MCP-Server](https://github.com/dinasaur404/BestReads-MCP-Server) | 基于 Workers 的远程 MCP 服务器。 | Workers, MCP | Medium | Active | Medium |
| [omarshahine/fastmail-mcp-remote](https://github.com/omarshahine/fastmail-mcp-remote) | 使用 Cloudflare Access OAuth 的 Fastmail 远程 MCP 服务器。 | Workers, Access OAuth, MCP | Medium | Active | Medium |
| [ofershap/mcp-server-cloudflare](https://github.com/ofershap/mcp-server-cloudflare) | 用于管理 Workers、KV、R2、DNS 和缓存的 MCP 服务器。 | Workers, KV, R2, DNS APIs | Medium | Active | Medium |
| [Jignesh-Ponamwar/skills-mcp](https://github.com/Jignesh-Ponamwar/skills-mcp) | 通过 MCP 提供的可自托管语义搜索 Agent Skills 注册表。 | Workers, MCP, vector search | Medium | Active | Medium |
| [Mihai-Codes/cf_ai_canvas](https://github.com/Mihai-Codes/cf_ai_canvas) | 协作画布与远程 MCP 服务器。 | Workers, Durable Objects, MCP, Workers AI | Medium | Active | Medium |

## 存储与记忆

| 项目 | 用途 | Cloudflare 技术栈 | 部署 | 状态 | 风险 |
|---|---|---|---|---|---|
| [TimeSurgeLabs/athenadb](https://github.com/TimeSurgeLabs/athenadb) | Serverless 向量数据库 API。 | Workers, D1, Vectorize, Workers AI | Medium | Stable | Medium |
| [elizabethsiegle/art-vector-search-cloudflare](https://github.com/elizabethsiegle/art-vector-search-cloudflare) | 使用 Vectorize 和 Workers AI 的艺术品搜索。 | Vectorize, Workers AI, AI Gateway | Medium | Stable | Medium |
| [synapse-ai-labs/synapse-api](https://github.com/synapse-ai-labs/synapse-api) | 使用 Vectorize 和 OpenAI 的 Serverless Embeddings API。 | Workers, D1, Vectorize | Medium | Stable | Medium |
| [zdmc23/cf-service-vector](https://github.com/zdmc23/cf-service-vector) | 面向 Pages Functions Service Binding 的 Vectorize API 包装器。 | Workers, Pages Functions, Vectorize | Medium | Stable | Low |
| [adam0white/MessageAI](https://github.com/adam0white/MessageAI) | 带 RAG 和 Agent 的实时消息应用。 | Workers, Durable Objects, Vectorize, Workers AI | Hard | Active | Medium |
| [vishal-codes/course-hero-rag-bot](https://github.com/vishal-codes/course-hero-rag-bot) | 面向选课聊天机器人的紧凑 RAG API。 | Workers, Vectorize | Medium | Active | Medium |

## 模板与脚手架

| 项目 | 用途 | Cloudflare 技术栈 | 部署 | 状态 | 风险 |
|---|---|---|---|---|---|
| [louisbrulenaudet/genai-api](https://github.com/louisbrulenaudet/genai-api) | Workers + Gemini API 模板。 | Workers, AI Gateway, Hono | Easy | Active | Medium |
| [nuxt-hub/core](https://github.com/nuxt-hub/core) | 为 Nuxt 增加数据库、KV、对象存储、缓存和 AI 集成的模块。 | D1, KV, R2, Workers AI | Medium | Active | Low |
| [JSONbored/opennextjs-cli](https://github.com/JSONbored/opennextjs-cli) | 面向 Workers 上 OpenNext.js 的 CLI/TUI，并带 MCP 能力。 | Workers, OpenNext, MCP | Medium | Active | Low |
| [jamescary/quickstart-template](https://github.com/jamescary/quickstart-template) | Cloudflare 原生全栈 starter。 | D1, KV, Durable Objects | Easy | Active | Low |
| [acoyfellow/svelte-edge](https://github.com/acoyfellow/svelte-edge) | 在 Workers 上编译 Agent 生成的 Svelte UI。 | Workers, Hono, Workers AI | Medium | Active | Medium |
| [Geekgineer/needle-rs](https://github.com/Geekgineer/needle-rs) | 适用于浏览器、Workers 和 Node 的小型 WASM 工具调用 Transformer 运行时。 | Workers, WASM | Hard | Active | Low |

## 可观测性与运维

| 项目 | 用途 | Cloudflare 技术栈 | 部署 | 状态 | 风险 |
|---|---|---|---|---|---|
| [PoemMisty/CF-Request-Analytics-Panel](https://github.com/PoemMisty/CF-Request-Analytics-Panel) | Cloudflare 多账号请求分析面板。 | Workers, analytics APIs | Medium | Active | Medium |
| [bgdnvk/clanker](https://github.com/bgdnvk/clanker) | 面向云环境的自治系统工程 CLI Agent。 | Cloudflare support, Workers topics | Hard | Active | Medium |
| [avansaber/seo-monster](https://github.com/avansaber/seo-monster) | 包含 Cloudflare 数据的只读 SEO 工作流 MCP 服务器。 | MCP, Cloudflare integrations | Medium | Active | Medium |
| [sebastienrousseau/cloudcdn.pro](https://github.com/sebastienrousseau/cloudcdn.pro) | 带 MCP 控制和边缘能力的 AI 原生 CDN。 | Workers, Pages, Durable Objects, Vectorize, Workers AI | Hard | Active | Medium |

## 谨慎使用

这些项目可用于学习或自托管，但涉及匿名消息、公共搜索、邮箱、服务条款边界或高权限账号访问等敏感模式。部署前请审查代码、权限、日志、滥用防护和上游条款。

| 项目 | 用途 | Cloudflare 技术栈 | 部署 | 状态 | 风险 |
|---|---|---|---|---|---|
| [Vauth/duckgpt](https://github.com/Vauth/duckgpt) | 使用 Workers AI 风格模型访问的聊天应用。 | Workers AI, Workers | Medium | Use with care | High |
| [mohetios/Nekonymous](https://github.com/mohetios/Nekonymous) | 带加密中继的匿名 Telegram Bot。 | Workers, D1, KV, Queues, Vectorize | Medium | Use with care | High |
| [elizabethsiegle/remote-mcp-server-authless-chat-with-cal](https://github.com/elizabethsiegle/remote-mcp-server-authless-chat-with-cal) | 无认证日历 MCP 演示。 | Workers, Workers AI, MCP | Medium | Use with care | High |
| [nikolanovoselec/m365-mcp-server-production](https://github.com/nikolanovoselec/m365-mcp-server-production) | Microsoft 365 远程 MCP 服务器示例。 | Workers, MCP, AI Gateway | Hard | Use with care | High |

## 收录标准

### 必须满足

- 开源代码，或至少核心代码可审计。
- 与 Cloudflare Workers、Pages、Workers AI、AI Gateway、D1、KV、R2、Vectorize、Durable Objects、Queues、Email Routing、Turnstile 或 Cloudflare 账号 API 有明确关系。
- README 或文档说明项目用途和基本设置。
- 不是纯营销页面。

### 优先收录

- 近期有 commit、release、issue 回复或 PR 活动。
- 有 `wrangler` 配置、一键部署或逐步 Cloudflare 部署文档。
- 有 demo、截图、架构说明或测试。
- 清楚说明环境变量、权限、成本和安全注意事项。

### 暂不收录

- 只有想法、没有可运行代码的仓库。
- 闭源服务。
- 只是顺带提到 Cloudflare 的仓库。
- 明显用于滥用、绕过限制、窃取凭据或规避平台政策的项目。
- 已归档或长期无人维护的项目，除非仍有明确参考价值。

## 贡献

欢迎提交 PR。提交项目之前请阅读 [CONTRIBUTING.md](../CONTRIBUTING.md)。

新增项目时请包含：

- 项目用途。
- 使用了哪些 Cloudflare 组件。
- 部署难度。
- 维护状态。
- 风险或安全说明。

## 许可证

MIT。见 [LICENSE](../LICENSE)。
