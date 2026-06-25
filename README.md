# Awesome Cloudflare AI

> Curated open-source AI, Agent, MCP, Workers AI, D1, R2, Vectorize, and Durable Objects projects deployable on Cloudflare.

一个严格筛选的 Cloudflare AI / Agent / MCP 开源项目导航。这里不收泛 AI 工具大全，只收录与 Cloudflare 部署、运行时或数据组件有明确关系的开源项目。

Last reviewed: 2026-06-26

## Why This List

Cloudflare 的 Workers、Pages、D1、KV、R2、Vectorize、Durable Objects、Workers AI、AI Gateway 和 Queues 正在成为低成本部署 AI 应用与 Agent 的重要基础设施。本项目关注三件事：

- Deployable: 项目能在 Cloudflare 上部署，或核心架构明显依赖 Cloudflare。
- Verifiable: README、配置文件、示例或文档足以判断用途和部署方式。
- Maintained: 优先收录近期仍有维护迹象的项目。

## Legend

| Field | Values |
|---|---|
| Deploy | Easy = 一键部署或清晰命令；Medium = 需要多个服务/API key；Hard = 需要理解架构或改代码 |
| Status | Active = 最近 6 个月有明显维护；Stable = 更新较少但仍有参考价值；Use with care = 有安全、合规、隐私或滥用风险 |
| Risk | Low = 普通应用/模板；Medium = 涉及用户数据、API key、文件、账号或自动化；High = 代理、匿名、绕限制、爬虫等敏感用途 |

## Contents

- [Official and Core](#official-and-core)
- [AI Apps on Cloudflare](#ai-apps-on-cloudflare)
- [Agents on Workers](#agents-on-workers)
- [MCP on Cloudflare](#mcp-on-cloudflare)
- [Storage and Memory](#storage-and-memory)
- [Templates and Starters](#templates-and-starters)
- [Observability and Ops](#observability-and-ops)
- [Use With Care](#use-with-care)
- [Selection Criteria](#selection-criteria)
- [Contributing](#contributing)

## Official and Core

| Project | What | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [cloudflare/agents](https://github.com/cloudflare/agents) | Official SDK for building and deploying AI agents. | Workers, Durable Objects, Workflows | Medium | Active | Low |
| [cloudflare/ai](https://github.com/cloudflare/ai) | Official Workers AI examples, demos, and packages. | Workers AI, Workers | Easy | Active | Low |
| [cloudflare/mcp-server-cloudflare](https://github.com/cloudflare/mcp-server-cloudflare) | Official MCP server for Cloudflare account resources. | MCP, Workers/KV/R2/DNS APIs | Medium | Active | Medium |
| [cloudflare/templates](https://github.com/cloudflare/templates) | Official Workers templates, including app and API starters. | Workers, Pages, D1, KV, R2 | Easy | Active | Low |
| [cloudflare/workers-chat-demo](https://github.com/cloudflare/workers-chat-demo) | Official real-time chat demo for edge-native apps. | Workers, Durable Objects | Medium | Active | Medium |
| [cloudflare/workers-sdk](https://github.com/cloudflare/workers-sdk) | Wrangler and Workers development toolchain. | Workers, Wrangler | Medium | Active | Low |

## AI Apps on Cloudflare

| Project | What | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [cloudflare/vibesdk](https://github.com/cloudflare/vibesdk) | Open-source vibe-coding platform built on Cloudflare. | Workers, Durable Objects | Medium | Active | Medium |
| [Jazee6/cloudflare-ai-web](https://github.com/Jazee6/cloudflare-ai-web) | One-click Cloudflare AI web platform. | Workers AI, Pages/Workers | Easy | Active | Medium |
| [miantiao-me/hacker-podcast](https://github.com/miantiao-me/hacker-podcast) | AI-generated Chinese podcast from Hacker News. | Workers, Workflows | Medium | Active | Medium |
| [nicholasgriffintn/ai-platform](https://github.com/nicholasgriffintn/ai-platform) | Multi-model personal AI assistant platform. | Workers, AI Gateway, Hono | Medium | Active | Medium |
| [unicornB/Supportly-Ai](https://github.com/unicornB/Supportly-Ai) | Cloudflare-native AI customer support platform. | Workers, Workers AI, knowledge base | Medium | Active | Medium |
| [G4brym/workers-research](https://github.com/G4brym/workers-research) | Serverless deep research agent. | Workers, Durable Objects | Medium | Active | Medium |
| [atinux/flux-ai-image-generator](https://github.com/atinux/flux-ai-image-generator) | Image generation app using Flux on Cloudflare. | Workers AI, R2, NuxtHub | Easy | Active | Medium |
| [chipmates/agoracosmica](https://github.com/chipmates/agoracosmica) | Educational AI conversation platform. | Workers, self-hosted app | Medium | Active | Medium |
| [devarshishimpi/codra](https://github.com/devarshishimpi/codra) | Self-hosted AI code review for GitHub PRs. | Workers, KV, Queues, Hyperdrive, Workers AI | Medium | Active | Medium |
| [bestian/askit-hono](https://github.com/bestian/askit-hono) | Cited RAG answers from Audrey Tang transcript archive. | Workers, Hono, Vectorize, Workers AI | Medium | Active | Medium |
| [Teycir/ArxivExplorer](https://github.com/Teycir/ArxivExplorer) | AI-enhanced semantic search for arXiv papers. | Workers, semantic search | Medium | Active | Medium |
| [IchimaruGin728/Gins-Blog](https://github.com/IchimaruGin728/Gins-Blog) | Edge blog with AI search and OAuth. | Workers, D1, R2, KV, Hono | Medium | Active | Medium |

## Agents on Workers

| Project | What | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [openma-ai/open-managed-agents](https://github.com/openma-ai/open-managed-agents) | Self-hosted implementation of Claude Managed Agents API. | Workers, Durable Objects | Medium | Active | Medium |
| [Logos-Flux/cloudflare-multiagent](https://github.com/Logos-Flux/cloudflare-multiagent) | Multi-agent AI platform on Workers. | Workers, AI generation | Medium | Active | Medium |
| [acoyfellow/flue-snippets](https://github.com/acoyfellow/flue-snippets) | Runnable Flue agent examples with deploy tests. | Workers, Durable Objects, Workers AI | Easy | Active | Low |
| [stukennedy/honi](https://github.com/stukennedy/honi) | Cloudflare-native agentic AI framework. | Durable Objects, Workers | Medium | Active | Medium |
| [acoyfellow/fleet-pattern](https://github.com/acoyfellow/fleet-pattern) | Hierarchical Durable Object agent pattern. | Workers, Durable Objects | Medium | Stable | Low |
| [serpin-taxt/openchief](https://github.com/serpin-taxt/openchief) | Agents that watch business tools and produce reports. | Workers, serverless runtime | Medium | Active | Medium |
| [huseynsnmz/postr](https://github.com/huseynsnmz/postr) | Keyboard-first email TUI with AI agent. | Workers, Durable Objects, Email Routing, Workers AI | Hard | Active | Medium |
| [Ahmad-A0/iris-voice-agent](https://github.com/Ahmad-A0/iris-voice-agent) | Real-time voice agent on the edge. | Workers, Durable Objects | Hard | Active | Medium |
| [sinameraji/kimiflare](https://github.com/sinameraji/kimiflare) | Terminal coding agent running on Cloudflare. | Workers AI, AI Gateway | Medium | Active | Medium |
| [marceloeatworld/clopinette-ai](https://github.com/marceloeatworld/clopinette-ai) | Multimodal AI agent with memory and bot integrations. | Workers, Durable Objects, Workers AI, AutoRAG | Hard | Active | Medium |

## MCP on Cloudflare

| Project | What | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [rahilp/second-brain-cloudflare](https://github.com/rahilp/second-brain-cloudflare) | Self-hosted AI memory layer for MCP clients. | Workers, D1, Vectorize | Medium | Active | Medium |
| [cyanheads/mcp-ts-core](https://github.com/cyanheads/mcp-ts-core) | TypeScript framework for MCP servers with Workers support. | Cloudflare Workers runtime | Medium | Active | Low |
| [Puliczek/mcp-memory](https://github.com/Puliczek/mcp-memory) | MCP memory server for user preferences and recall. | Workers, D1, Vectorize | Medium | Active | Medium |
| [Yrobot/cloudflare-search](https://github.com/Yrobot/cloudflare-search) | Search server that can enhance AI tools with MCP. | Workers, MCP | Medium | Active | Medium |
| [stytchauth/mcp-stytch-consumer-todo-list](https://github.com/stytchauth/mcp-stytch-consumer-todo-list) | TODO app MCP server with auth example. | Workers, MCP, Stytch | Medium | Active | Medium |
| [dinasaur404/BestReads-MCP-Server](https://github.com/dinasaur404/BestReads-MCP-Server) | Remote MCP server built on Workers. | Workers, MCP | Medium | Active | Medium |
| [omarshahine/fastmail-mcp-remote](https://github.com/omarshahine/fastmail-mcp-remote) | Fastmail remote MCP server with Cloudflare Access OAuth. | Workers, Access OAuth, MCP | Medium | Active | Medium |
| [ofershap/mcp-server-cloudflare](https://github.com/ofershap/mcp-server-cloudflare) | MCP server to manage Workers, KV, R2, DNS, and cache. | Workers, KV, R2, DNS APIs | Medium | Active | Medium |
| [Jignesh-Ponamwar/skills-mcp](https://github.com/Jignesh-Ponamwar/skills-mcp) | Self-hostable searchable Agent Skills registry over MCP. | Workers, MCP, vector search | Medium | Active | Medium |
| [Mihai-Codes/cf_ai_canvas](https://github.com/Mihai-Codes/cf_ai_canvas) | Collaborative canvas and remote MCP server. | Workers, Durable Objects, MCP, Workers AI | Medium | Active | Medium |

## Storage and Memory

| Project | What | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [TimeSurgeLabs/athenadb](https://github.com/TimeSurgeLabs/athenadb) | Serverless vector database API. | Workers, D1, Vectorize, Workers AI | Medium | Stable | Medium |
| [elizabethsiegle/art-vector-search-cloudflare](https://github.com/elizabethsiegle/art-vector-search-cloudflare) | Art search using Vectorize and Workers AI. | Vectorize, Workers AI, AI Gateway | Medium | Stable | Medium |
| [synapse-ai-labs/synapse-api](https://github.com/synapse-ai-labs/synapse-api) | Serverless embeddings API using Vectorize and OpenAI. | Workers, D1, Vectorize | Medium | Stable | Medium |
| [zdmc23/cf-service-vector](https://github.com/zdmc23/cf-service-vector) | Vectorize API wrapper for Pages Functions service binding use. | Workers, Pages Functions, Vectorize | Medium | Stable | Low |
| [adam0white/MessageAI](https://github.com/adam0white/MessageAI) | Real-time messaging app with RAG and agents. | Workers, Durable Objects, Vectorize, Workers AI | Hard | Active | Medium |
| [vishal-codes/course-hero-rag-bot](https://github.com/vishal-codes/course-hero-rag-bot) | Compact RAG API for course-selection chatbot. | Workers, Vectorize | Medium | Active | Medium |

## Templates and Starters

| Project | What | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [louisbrulenaudet/genai-api](https://github.com/louisbrulenaudet/genai-api) | Workers + Gemini API template. | Workers, AI Gateway, Hono | Easy | Active | Medium |
| [nuxt-hub/core](https://github.com/nuxt-hub/core) | Nuxt module adding database, KV, blob storage, cache, and AI integrations. | D1, KV, R2, Workers AI | Medium | Active | Low |
| [JSONbored/opennextjs-cli](https://github.com/JSONbored/opennextjs-cli) | CLI/TUI for OpenNext.js on Workers with MCP features. | Workers, OpenNext, MCP | Medium | Active | Low |
| [jamescary/quickstart-template](https://github.com/jamescary/quickstart-template) | Cloudflare-native full-stack starter. | D1, KV, Durable Objects | Easy | Active | Low |
| [acoyfellow/svelte-edge](https://github.com/acoyfellow/svelte-edge) | Agent-generated Svelte UI compiled on Workers. | Workers, Hono, Workers AI | Medium | Active | Medium |
| [Geekgineer/needle-rs](https://github.com/Geekgineer/needle-rs) | Small WASM tool-calling transformer runtime for browser, Workers, and Node. | Workers, WASM | Hard | Active | Low |

## Observability and Ops

| Project | What | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [PoemMisty/CF-Request-Analytics-Panel](https://github.com/PoemMisty/CF-Request-Analytics-Panel) | Multi-account Cloudflare request analytics panel. | Workers, analytics APIs | Medium | Active | Medium |
| [bgdnvk/clanker](https://github.com/bgdnvk/clanker) | Autonomous systems engineering CLI agent for cloud environments. | Cloudflare support, Workers topics | Hard | Active | Medium |
| [avansaber/seo-monster](https://github.com/avansaber/seo-monster) | Read-first MCP server for SEO workflows including Cloudflare data. | MCP, Cloudflare integrations | Medium | Active | Medium |
| [sebastienrousseau/cloudcdn.pro](https://github.com/sebastienrousseau/cloudcdn.pro) | AI-native CDN with MCP controls and edge features. | Workers, Pages, Durable Objects, Vectorize, Workers AI | Hard | Active | Medium |

## Use With Care

These projects may be useful for learning or self-hosting, but they involve sensitive patterns such as anonymous messaging, public search, email, provider policy boundaries, or privileged account access. Review code, permissions, logging, abuse controls, and upstream terms before deploying.

| Project | What | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [Vauth/duckgpt](https://github.com/Vauth/duckgpt) | Chat app using Workers AI-style model access. | Workers AI, Workers | Medium | Use with care | High |
| [mohetios/Nekonymous](https://github.com/mohetios/Nekonymous) | Anonymous Telegram bot with encrypted relay. | Workers, D1, KV, Queues, Vectorize | Medium | Use with care | High |
| [elizabethsiegle/remote-mcp-server-authless-chat-with-cal](https://github.com/elizabethsiegle/remote-mcp-server-authless-chat-with-cal) | Authless calendar MCP demo. | Workers, Workers AI, MCP | Medium | Use with care | High |
| [nikolanovoselec/m365-mcp-server-production](https://github.com/nikolanovoselec/m365-mcp-server-production) | Microsoft 365 remote MCP server example. | Workers, MCP, AI Gateway | Hard | Use with care | High |

## Selection Criteria

### Must Have

- Open-source code, or at least auditable core code.
- Clear relationship to Cloudflare Workers, Pages, Workers AI, AI Gateway, D1, KV, R2, Vectorize, Durable Objects, Queues, Email Routing, Turnstile, or Cloudflare account APIs.
- README or docs that explain the project purpose and basic setup.
- Not a pure marketing site.

### Preferred

- Recent commit, release, issue reply, or PR activity.
- `wrangler` config, one-click deploy, or step-by-step Cloudflare deployment docs.
- Demo, screenshots, architecture notes, or tests.
- Clear environment variables, permissions, cost, and security notes.

### Not Included

- Idea-only repos with no runnable code.
- Closed-source services.
- Repos where Cloudflare is only mentioned in passing.
- Obvious abuse, bypass, credential harvesting, or policy-evasion projects.
- Archived or unmaintained projects unless they are still valuable references.

## Contributing

Pull requests are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a project.

When adding a project, include:

- What it does.
- Which Cloudflare components it uses.
- Deployment difficulty.
- Maintenance status.
- Any risk or safety notes.

## License

MIT. See [LICENSE](LICENSE).
