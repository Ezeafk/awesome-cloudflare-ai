# Awesome Cloudflare AI

> Curated open-source AI, Agent, MCP, Workers AI, D1, R2, Vectorize, and Durable Objects projects deployable on Cloudflare.

Languages: [English](README.md) | [简体中文](i18n/README.zh-CN.md) | [Português do Brasil](i18n/README.pt-BR.md) | [日本語](i18n/README.ja.md) | [Deutsch](i18n/README.de.md) | [Русский](i18n/README.ru.md)

A strictly curated directory of Cloudflare AI / Agent / MCP open-source projects. This is not a general AI tools list. It only includes projects with a clear connection to Cloudflare deployment, runtime, or data infrastructure.

Last reviewed: 2026-06-30

## Why This List

Cloudflare Workers, Pages, D1, KV, R2, Vectorize, Durable Objects, Workers AI, AI Gateway, and Queues are becoming important building blocks for low-cost AI apps and agents. This project focuses on three things:

- Deployable: the project can run on Cloudflare, or its core architecture clearly depends on Cloudflare.
- Verifiable: README files, config files, examples, or docs make the purpose and deployment path clear.
- Maintained: projects with recent signs of maintenance are preferred.

## Legend

| Field | Values |
|---|---|
| Deploy | Easy = one-click deploy or clear commands; Medium = multiple services/API keys; Hard = architecture knowledge or code changes required |
| Status | Active = clear maintenance in the last 6 months; Stable = less recent activity but still useful; Use with care = security, compliance, privacy, or abuse risk |
| Risk | Low = ordinary app/template; Medium = user data, API keys, files, accounts, or automation; High = proxy, anonymous, restriction-bypass, crawling, or similarly sensitive use |

## Evaluation Method

Projects are scored before inclusion. Stars are a weak signal only; a new project can be included when it is clearly relevant, deployable, documented, and safe enough to recommend.

| Area | Points | What reviewers check |
|---|---:|---|
| Cloudflare relevance | 0-3 | Direct use of Workers, Pages, Workers AI, AI Gateway, D1, KV, R2, Vectorize, Durable Objects, Queues, Email Routing, Turnstile, or Cloudflare APIs. |
| Deployability | 0-2 | Clear deploy path, wrangler config, template, demo, or setup instructions. |
| Maintenance | 0-2 | Recent commits, releases, issue replies, or active community use. |
| Documentation and license | 0-2 | Clear README, environment variables, architecture notes, and auditable license. |
| Safety | 0-1 | Reasonable boundaries for auth, user data, uploads, automation, proxies, email, or privileged APIs. |

Inclusion guide: 8-10 = recommended, 6-7 = acceptable with caveats, 4-5 = use with care or re-review, below 4 = remove or do not include. High-risk projects need a stronger score and explicit safety notes.

## Contents

- [Official and Core](#official-and-core)
- [AI Apps on Cloudflare](#ai-apps-on-cloudflare)
- [Agents on Workers](#agents-on-workers)
- [MCP on Cloudflare](#mcp-on-cloudflare)
- [Storage and Memory](#storage-and-memory)
- [Templates and Starters](#templates-and-starters)
- [Observability and Ops](#observability-and-ops)
- [Use With Care](#use-with-care)
- [Evaluation Method](#evaluation-method)
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
| [arusso-aboutcloud/aboutcloud-search](https://github.com/arusso-aboutcloud/aboutcloud-search) | Auditable RAG chatbot with explicit safety guardrails. | Workers AI, Vectorize, D1, Workers | Medium | Active | Medium |

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
| [acoyfellow/my-ax](https://github.com/acoyfellow/my-ax) | Personal AI agent operating environment self-hosted on Cloudflare. | Workers, Durable Objects, D1, MCP | Hard | Active | Medium |
| [yukthapriya/web-research-agent](https://github.com/yukthapriya/web-research-agent) | Web research agent that plans, searches, and writes cited reports. | Workers AI, Workflows, Durable Objects | Medium | Active | Medium |

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
| [miantiao-me/github-stars](https://github.com/miantiao-me/github-stars) | Natural-language search over GitHub starred repositories via MCP. | Workers, MCP, R2, AutoRAG | Medium | Active | Medium |

## Storage and Memory

| Project | What | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [TimeSurgeLabs/athenadb](https://github.com/TimeSurgeLabs/athenadb) | Serverless vector database API. | Workers, D1, Vectorize, Workers AI | Medium | Stable | Medium |
| [elizabethsiegle/art-vector-search-cloudflare](https://github.com/elizabethsiegle/art-vector-search-cloudflare) | Art search using Vectorize and Workers AI. | Vectorize, Workers AI, AI Gateway | Medium | Stable | Medium |
| [synapse-ai-labs/synapse-api](https://github.com/synapse-ai-labs/synapse-api) | Serverless embeddings API using Vectorize and OpenAI. | Workers, D1, Vectorize | Medium | Stable | Medium |
| [adam0white/MessageAI](https://github.com/adam0white/MessageAI) | Real-time messaging app with RAG and agents. | Workers, Durable Objects, Vectorize, Workers AI | Hard | Active | Medium |
| [realchendahuang/FlareMo](https://github.com/realchendahuang/FlareMo) | Cloudflare-native personal knowledge system with Memos API and MCP subset. | Workers, D1, R2, Access, MCP | Easy | Active | Medium |

## Templates and Starters

| Project | What | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [louisbrulenaudet/genai-api](https://github.com/louisbrulenaudet/genai-api) | Workers + Gemini API template. | Workers, AI Gateway, Hono | Easy | Active | Medium |
| [nuxt-hub/core](https://github.com/nuxt-hub/core) | Nuxt module adding database, KV, blob storage, cache, and AI integrations. | D1, KV, R2, Workers AI | Medium | Active | Low |
| [JSONbored/opennextjs-cli](https://github.com/JSONbored/opennextjs-cli) | CLI/TUI for OpenNext.js on Workers with MCP features. | Workers, OpenNext, MCP | Medium | Active | Low |
| [acoyfellow/svelte-edge](https://github.com/acoyfellow/svelte-edge) | Agent-generated Svelte UI compiled on Workers. | Workers, Hono, Workers AI | Medium | Active | Medium |
| [Geekgineer/needle-rs](https://github.com/Geekgineer/needle-rs) | Small WASM tool-calling transformer runtime for browser, Workers, and Node. | Workers, WASM | Hard | Active | Low |

## Observability and Ops

| Project | What | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [PoemMisty/CF-Request-Analytics-Panel](https://github.com/PoemMisty/CF-Request-Analytics-Panel) | Multi-account Cloudflare request analytics panel. | Workers, analytics APIs | Medium | Active | Medium |
| [bgdnvk/clanker](https://github.com/bgdnvk/clanker) | Autonomous systems engineering CLI agent for cloud environments. | Cloudflare support, Workers topics | Hard | Active | Medium |

## Use With Care

These projects may be useful for learning or self-hosting, but they involve sensitive patterns such as anonymous messaging, public search, email, provider policy boundaries, or privileged account access. Review code, permissions, logging, abuse controls, and upstream terms before deploying.

| Project | What | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [Vauth/duckgpt](https://github.com/Vauth/duckgpt) | Chat app using Workers AI-style model access. | Workers AI, Workers | Medium | Use with care | High |

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
