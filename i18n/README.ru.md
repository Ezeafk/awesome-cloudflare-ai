# Awesome Cloudflare AI

> Подборка open-source проектов AI, Agent, MCP, Workers AI, D1, R2, Vectorize и Durable Objects, которые можно развернуть на Cloudflare.

Языки: [English](../README.md) | [简体中文](README.zh-CN.md) | [Português do Brasil](README.pt-BR.md) | [日本語](README.ja.md) | [Deutsch](README.de.md) | [Русский](README.ru.md)

Строго отобранный каталог open-source проектов Cloudflare AI / Agent / MCP. Это не общий список AI-инструментов: сюда входят только проекты с явной связью с деплоем, runtime или data-инфраструктурой Cloudflare.

Последняя проверка: 2026-06-26

## Зачем нужен этот список

Cloudflare Workers, Pages, D1, KV, R2, Vectorize, Durable Objects, Workers AI, AI Gateway и Queues становятся важными строительными блоками для недорогих AI-приложений и агентов. Этот проект фокусируется на трех вещах:

- Развертываемость: проект работает на Cloudflare или его ключевая архитектура явно зависит от Cloudflare.
- Проверяемость: README, конфиги, примеры или документация позволяют понять назначение и путь деплоя.
- Поддержка: приоритет у проектов с недавними признаками сопровождения.

## Обозначения

| Поле | Значения |
|---|---|
| Deploy | Easy = one-click deploy или понятные команды; Medium = несколько сервисов/API keys; Hard = требуется понимание архитектуры или изменение кода |
| Status | Active = заметная поддержка за последние 6 месяцев; Stable = обновлений меньше, но проект полезен; Use with care = риски безопасности, комплаенса, приватности или злоупотреблений |
| Risk | Low = обычное приложение/шаблон; Medium = пользовательские данные, API keys, файлы, аккаунты или автоматизация; High = proxy, анонимность, обход ограничений, crawling или похожие чувствительные сценарии |

## Метод Оценки

Перед включением проекты получают оценку. Stars — только слабый сигнал; новый проект можно включить, если он явно связан с Cloudflare, разворачивается, хорошо документирован и достаточно безопасен для рекомендации.

| Область | Баллы | Что проверяется |
|---|---:|---|
| Связь с Cloudflare | 0-3 | Прямое использование Workers, Pages, Workers AI, AI Gateway, D1, KV, R2, Vectorize, Durable Objects, Queues, Email Routing, Turnstile или Cloudflare APIs. |
| Развертываемость | 0-2 | Понятный путь deploy, wrangler config, template, demo или setup instructions. |
| Поддержка | 0-2 | Недавние commits, releases, issue replies или активное community use. |
| Документация и лицензия | 0-2 | Понятный README, environment variables, architecture notes и проверяемая license. |
| Безопасность | 0-1 | Разумные границы для auth, user data, uploads, automation, proxies, email или privileged APIs. |

Ориентир включения: 8-10 = рекомендуется, 6-7 = допустимо с оговорками, 4-5 = use with care или повторная проверка, ниже 4 = удалить или не включать. High-risk проекты требуют более высокого балла и явных заметок по безопасности.

## Содержание

- [Официальные и базовые проекты](#официальные-и-базовые-проекты)
- [AI-приложения на Cloudflare](#ai-приложения-на-cloudflare)
- [Agents на Workers](#agents-на-workers)
- [MCP на Cloudflare](#mcp-на-cloudflare)
- [Хранилище и память](#хранилище-и-память)
- [Шаблоны и стартеры](#шаблоны-и-стартеры)
- [Observability и Ops](#observability-и-ops)
- [Использовать с осторожностью](#использовать-с-осторожностью)
- [Метод Оценки](#метод-оценки)
- [Критерии отбора](#критерии-отбора)
- [Участие](#участие)

## Официальные и базовые проекты

| Проект | Что делает | Cloudflare stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [cloudflare/agents](https://github.com/cloudflare/agents) | Официальный SDK для создания и деплоя AI agents. | Workers, Durable Objects, Workflows | Medium | Active | Low |
| [cloudflare/ai](https://github.com/cloudflare/ai) | Официальные примеры, демо и пакеты Workers AI. | Workers AI, Workers | Easy | Active | Low |
| [cloudflare/mcp-server-cloudflare](https://github.com/cloudflare/mcp-server-cloudflare) | Официальный MCP server для ресурсов аккаунта Cloudflare. | MCP, Workers/KV/R2/DNS APIs | Medium | Active | Medium |
| [cloudflare/templates](https://github.com/cloudflare/templates) | Официальные Workers templates для приложений и API. | Workers, Pages, D1, KV, R2 | Easy | Active | Low |
| [cloudflare/workers-chat-demo](https://github.com/cloudflare/workers-chat-demo) | Официальное realtime chat demo для edge-приложений. | Workers, Durable Objects | Medium | Active | Medium |
| [cloudflare/workers-sdk](https://github.com/cloudflare/workers-sdk) | Wrangler и toolchain для разработки Workers. | Workers, Wrangler | Medium | Active | Low |

## AI-приложения на Cloudflare

| Проект | Что делает | Cloudflare stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [cloudflare/vibesdk](https://github.com/cloudflare/vibesdk) | Open-source платформа vibe coding на стеке Cloudflare. | Workers, Durable Objects | Medium | Active | Medium |
| [Jazee6/cloudflare-ai-web](https://github.com/Jazee6/cloudflare-ai-web) | Cloudflare AI web platform с one-click deploy. | Workers AI, Pages/Workers | Easy | Active | Medium |
| [miantiao-me/hacker-podcast](https://github.com/miantiao-me/hacker-podcast) | AI-подкаст на китайском из материалов Hacker News. | Workers, Workflows | Medium | Active | Medium |
| [nicholasgriffintn/ai-platform](https://github.com/nicholasgriffintn/ai-platform) | Multi-model платформа персонального AI assistant. | Workers, AI Gateway, Hono | Medium | Active | Medium |
| [unicornB/Supportly-Ai](https://github.com/unicornB/Supportly-Ai) | Cloudflare-native платформа AI customer support. | Workers, Workers AI, knowledge base | Medium | Active | Medium |
| [G4brym/workers-research](https://github.com/G4brym/workers-research) | Serverless агент для глубокого исследования. | Workers, Durable Objects | Medium | Active | Medium |
| [atinux/flux-ai-image-generator](https://github.com/atinux/flux-ai-image-generator) | Генерация изображений с Flux на Cloudflare. | Workers AI, R2, NuxtHub | Easy | Active | Medium |
| [chipmates/agoracosmica](https://github.com/chipmates/agoracosmica) | Образовательная платформа для AI-разговоров. | Workers, self-hosted app | Medium | Active | Medium |
| [devarshishimpi/codra](https://github.com/devarshishimpi/codra) | Self-hosted AI code review для GitHub PR. | Workers, KV, Queues, Hyperdrive, Workers AI | Medium | Active | Medium |
| [bestian/askit-hono](https://github.com/bestian/askit-hono) | RAG-ответы с цитатами из архива расшифровок Audrey Tang. | Workers, Hono, Vectorize, Workers AI | Medium | Active | Medium |
| [Teycir/ArxivExplorer](https://github.com/Teycir/ArxivExplorer) | AI-enhanced semantic search для arXiv papers. | Workers, semantic search | Medium | Active | Medium |
| [IchimaruGin728/Gins-Blog](https://github.com/IchimaruGin728/Gins-Blog) | Edge blog с AI search и OAuth. | Workers, D1, R2, KV, Hono | Medium | Active | Medium |

## Agents на Workers

| Проект | Что делает | Cloudflare stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [openma-ai/open-managed-agents](https://github.com/openma-ai/open-managed-agents) | Self-hosted реализация Claude Managed Agents API. | Workers, Durable Objects | Medium | Active | Medium |
| [Logos-Flux/cloudflare-multiagent](https://github.com/Logos-Flux/cloudflare-multiagent) | Multi-agent AI platform на Workers. | Workers, AI generation | Medium | Active | Medium |
| [acoyfellow/flue-snippets](https://github.com/acoyfellow/flue-snippets) | Запускаемые примеры Flue agents с deploy tests. | Workers, Durable Objects, Workers AI | Easy | Active | Low |
| [stukennedy/honi](https://github.com/stukennedy/honi) | Cloudflare-native фреймворк для agentic AI. | Durable Objects, Workers | Medium | Active | Medium |
| [acoyfellow/fleet-pattern](https://github.com/acoyfellow/fleet-pattern) | Иерархический паттерн Durable Object agents. | Workers, Durable Objects | Medium | Stable | Low |
| [serpin-taxt/openchief](https://github.com/serpin-taxt/openchief) | Agents, которые наблюдают за business tools и делают отчеты. | Workers, serverless runtime | Medium | Active | Medium |
| [huseynsnmz/postr](https://github.com/huseynsnmz/postr) | Keyboard-first email TUI с AI agent. | Workers, Durable Objects, Email Routing, Workers AI | Hard | Active | Medium |
| [Ahmad-A0/iris-voice-agent](https://github.com/Ahmad-A0/iris-voice-agent) | Realtime voice agent на edge. | Workers, Durable Objects | Hard | Active | Medium |
| [sinameraji/kimiflare](https://github.com/sinameraji/kimiflare) | Terminal coding agent, работающий в аккаунте Cloudflare. | Workers AI, AI Gateway | Medium | Active | Medium |
| [marceloeatworld/clopinette-ai](https://github.com/marceloeatworld/clopinette-ai) | Мультимодальный AI agent с memory и bot integrations. | Workers, Durable Objects, Workers AI, AutoRAG | Hard | Active | Medium |

## MCP на Cloudflare

| Проект | Что делает | Cloudflare stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [rahilp/second-brain-cloudflare](https://github.com/rahilp/second-brain-cloudflare) | Self-hosted AI memory layer для MCP clients. | Workers, D1, Vectorize | Medium | Active | Medium |
| [cyanheads/mcp-ts-core](https://github.com/cyanheads/mcp-ts-core) | TypeScript framework для MCP servers с поддержкой Workers. | Cloudflare Workers runtime | Medium | Active | Low |
| [Puliczek/mcp-memory](https://github.com/Puliczek/mcp-memory) | MCP memory server для preferences и recall. | Workers, D1, Vectorize | Medium | Active | Medium |
| [Yrobot/cloudflare-search](https://github.com/Yrobot/cloudflare-search) | Search server, который расширяет AI tools через MCP. | Workers, MCP | Medium | Active | Medium |
| [stytchauth/mcp-stytch-consumer-todo-list](https://github.com/stytchauth/mcp-stytch-consumer-todo-list) | TODO app MCP server с примером auth. | Workers, MCP, Stytch | Medium | Active | Medium |
| [dinasaur404/BestReads-MCP-Server](https://github.com/dinasaur404/BestReads-MCP-Server) | Remote MCP server на Workers. | Workers, MCP | Medium | Active | Medium |
| [omarshahine/fastmail-mcp-remote](https://github.com/omarshahine/fastmail-mcp-remote) | Fastmail remote MCP с Cloudflare Access OAuth. | Workers, Access OAuth, MCP | Medium | Active | Medium |

## Хранилище и память

| Проект | Что делает | Cloudflare stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [TimeSurgeLabs/athenadb](https://github.com/TimeSurgeLabs/athenadb) | Serverless API для векторной базы данных. | Workers, D1, Vectorize, Workers AI | Medium | Stable | Medium |
| [elizabethsiegle/art-vector-search-cloudflare](https://github.com/elizabethsiegle/art-vector-search-cloudflare) | Поиск искусства с Vectorize и Workers AI. | Vectorize, Workers AI, AI Gateway | Medium | Stable | Medium |
| [synapse-ai-labs/synapse-api](https://github.com/synapse-ai-labs/synapse-api) | Serverless embeddings API с Vectorize и OpenAI. | Workers, D1, Vectorize | Medium | Stable | Medium |
| [adam0white/MessageAI](https://github.com/adam0white/MessageAI) | Realtime messaging app с RAG и agents. | Workers, Durable Objects, Vectorize, Workers AI | Hard | Active | Medium |

## Шаблоны и стартеры

| Проект | Что делает | Cloudflare stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [louisbrulenaudet/genai-api](https://github.com/louisbrulenaudet/genai-api) | Шаблон Workers + Gemini API. | Workers, AI Gateway, Hono | Easy | Active | Medium |
| [nuxt-hub/core](https://github.com/nuxt-hub/core) | Nuxt module для database, KV, blob storage, cache и AI integrations. | D1, KV, R2, Workers AI | Medium | Active | Low |
| [JSONbored/opennextjs-cli](https://github.com/JSONbored/opennextjs-cli) | CLI/TUI для OpenNext.js на Workers с MCP features. | Workers, OpenNext, MCP | Medium | Active | Low |
| [acoyfellow/svelte-edge](https://github.com/acoyfellow/svelte-edge) | Agent-generated Svelte UI, компилируемый на Workers. | Workers, Hono, Workers AI | Medium | Active | Medium |
| [Geekgineer/needle-rs](https://github.com/Geekgineer/needle-rs) | Маленький WASM runtime для tool-calling transformer. | Workers, WASM | Hard | Active | Low |

## Observability и Ops

| Проект | Что делает | Cloudflare stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [PoemMisty/CF-Request-Analytics-Panel](https://github.com/PoemMisty/CF-Request-Analytics-Panel) | Request analytics panel для нескольких Cloudflare accounts. | Workers, analytics APIs | Medium | Active | Medium |
| [bgdnvk/clanker](https://github.com/bgdnvk/clanker) | Autonomous systems engineering CLI agent для cloud environments. | Cloudflare support, Workers topics | Hard | Active | Medium |

## Использовать с осторожностью

Эти проекты могут быть полезны для обучения или self-hosting, но содержат чувствительные паттерны: анонимные сообщения, публичный поиск, email, границы правил провайдеров или привилегированный доступ к аккаунтам. Перед деплоем проверьте код, разрешения, логи, защиту от злоупотреблений и условия upstream-сервисов.

| Проект | Что делает | Cloudflare stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [Vauth/duckgpt](https://github.com/Vauth/duckgpt) | Chat app с доступом к моделям в стиле Workers AI. | Workers AI, Workers | Medium | Use with care | High |

## Критерии отбора

### Обязательно

- Open-source код или как минимум проверяемое ядро.
- Явная связь с Workers, Pages, Workers AI, AI Gateway, D1, KV, R2, Vectorize, Durable Objects, Queues, Email Routing, Turnstile или Cloudflare account APIs.
- README или docs объясняют назначение и базовую настройку.
- Это не чисто маркетинговая страница.

### Предпочтительно

- Недавние commits, releases, ответы в issues или PR activity.
- `wrangler` config, one-click deploy или пошаговая документация по деплою на Cloudflare.
- Demo, screenshots, architecture notes или tests.
- Понятные environment variables, permissions, cost и security notes.

### Не включается

- Репозитории только с идеей и без запускаемого кода.
- Closed-source сервисы.
- Репозитории, где Cloudflare упоминается лишь вскользь.
- Очевидный abuse, bypass, credential harvesting или policy-evasion.
- Архивные или неподдерживаемые проекты, если у них нет явной справочной ценности.

## Участие

Pull requests приветствуются. Перед предложением проекта прочитайте [CONTRIBUTING.md](../CONTRIBUTING.md).

При добавлении проекта укажите:

- Что он делает.
- Какие компоненты Cloudflare использует.
- Сложность деплоя.
- Статус поддержки.
- Риски или заметки по безопасности.

## Лицензия

MIT. См. [LICENSE](../LICENSE).
