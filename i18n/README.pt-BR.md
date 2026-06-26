# Awesome Cloudflare AI

> Projetos open source selecionados de AI, Agent, MCP, Workers AI, D1, R2, Vectorize e Durable Objects implantáveis na Cloudflare.

Idiomas: [English](../README.md) | [简体中文](README.zh-CN.md) | [Português do Brasil](README.pt-BR.md) | [日本語](README.ja.md) | [Deutsch](README.de.md) | [Русский](README.ru.md)

Um diretório rigorosamente selecionado de projetos open source de Cloudflare AI / Agent / MCP. Esta não é uma lista genérica de ferramentas de IA; ela inclui apenas projetos com relação clara com implantação, runtime ou infraestrutura de dados da Cloudflare.

Última revisão: 2026-06-26

## Por que esta lista

Cloudflare Workers, Pages, D1, KV, R2, Vectorize, Durable Objects, Workers AI, AI Gateway e Queues estão se tornando blocos importantes para apps de IA e agentes de baixo custo. Este projeto foca em três pontos:

- Implantável: o projeto roda na Cloudflare, ou sua arquitetura principal depende claramente da Cloudflare.
- Verificável: README, configs, exemplos ou docs deixam claros o propósito e o caminho de implantação.
- Mantido: projetos com sinais recentes de manutenção têm prioridade.

## Legenda

| Campo | Valores |
|---|---|
| Deploy | Easy = deploy em um clique ou comandos claros; Medium = vários serviços/API keys; Hard = exige entender arquitetura ou alterar código |
| Status | Active = manutenção clara nos últimos 6 meses; Stable = menos recente, mas ainda útil; Use with care = risco de segurança, compliance, privacidade ou abuso |
| Risk | Low = app/template comum; Medium = dados de usuário, API keys, arquivos, contas ou automação; High = proxy, anonimato, contorno de restrições, crawling ou uso sensível |

## Método de Avaliação

Os projetos são pontuados antes da inclusão. Stars são apenas um sinal fraco; um projeto novo pode entrar quando é claramente relevante para Cloudflare, implantável, documentado e seguro o bastante para recomendar.

| Área | Pontos | O que revisar |
|---|---:|---|
| Relevância para Cloudflare | 0-3 | Uso direto de Workers, Pages, Workers AI, AI Gateway, D1, KV, R2, Vectorize, Durable Objects, Queues, Email Routing, Turnstile ou APIs da Cloudflare. |
| Deployability | 0-2 | Caminho de deploy claro, config wrangler, template, demo ou instruções de setup. |
| Manutenção | 0-2 | Commits, releases, respostas em issues ou uso comunitário recente. |
| Documentação e licença | 0-2 | README claro, variáveis de ambiente, notas de arquitetura e licença auditável. |
| Segurança | 0-1 | Limites razoáveis para auth, dados de usuários, uploads, automação, proxies, email ou APIs privilegiadas. |

Guia de inclusão: 8-10 = recomendado, 6-7 = aceitável com ressalvas, 4-5 = use com cuidado ou revise novamente, abaixo de 4 = remover ou não incluir. Projetos de alto risco precisam de pontuação mais forte e notas explícitas de segurança.

## Conteúdo

- [Oficiais e essenciais](#oficiais-e-essenciais)
- [Apps de IA na Cloudflare](#apps-de-ia-na-cloudflare)
- [Agents em Workers](#agents-em-workers)
- [MCP na Cloudflare](#mcp-na-cloudflare)
- [Armazenamento e memória](#armazenamento-e-memória)
- [Templates e starters](#templates-e-starters)
- [Observabilidade e ops](#observabilidade-e-ops)
- [Use com cuidado](#use-com-cuidado)
- [Método de Avaliação](#método-de-avaliação)
- [Critérios de seleção](#critérios-de-seleção)
- [Contribuição](#contribuição)

## Oficiais e essenciais

| Projeto | O que faz | Stack Cloudflare | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [cloudflare/agents](https://github.com/cloudflare/agents) | SDK oficial para criar e implantar agentes de IA. | Workers, Durable Objects, Workflows | Medium | Active | Low |
| [cloudflare/ai](https://github.com/cloudflare/ai) | Exemplos, demos e pacotes oficiais de Workers AI. | Workers AI, Workers | Easy | Active | Low |
| [cloudflare/mcp-server-cloudflare](https://github.com/cloudflare/mcp-server-cloudflare) | Servidor MCP oficial para recursos de contas Cloudflare. | MCP, Workers/KV/R2/DNS APIs | Medium | Active | Medium |
| [cloudflare/templates](https://github.com/cloudflare/templates) | Templates oficiais para Workers, apps e APIs. | Workers, Pages, D1, KV, R2 | Easy | Active | Low |
| [cloudflare/workers-chat-demo](https://github.com/cloudflare/workers-chat-demo) | Demo oficial de chat em tempo real na edge. | Workers, Durable Objects | Medium | Active | Medium |
| [cloudflare/workers-sdk](https://github.com/cloudflare/workers-sdk) | Wrangler e toolchain de desenvolvimento para Workers. | Workers, Wrangler | Medium | Active | Low |

## Apps de IA na Cloudflare

| Projeto | O que faz | Stack Cloudflare | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [cloudflare/vibesdk](https://github.com/cloudflare/vibesdk) | Plataforma open source de vibe coding construída na Cloudflare. | Workers, Durable Objects | Medium | Active | Medium |
| [Jazee6/cloudflare-ai-web](https://github.com/Jazee6/cloudflare-ai-web) | Plataforma web de IA da Cloudflare com deploy em um clique. | Workers AI, Pages/Workers | Easy | Active | Medium |
| [miantiao-me/hacker-podcast](https://github.com/miantiao-me/hacker-podcast) | Podcast chinês gerado por IA a partir do Hacker News. | Workers, Workflows | Medium | Active | Medium |
| [nicholasgriffintn/ai-platform](https://github.com/nicholasgriffintn/ai-platform) | Plataforma de assistente pessoal de IA multi-modelo. | Workers, AI Gateway, Hono | Medium | Active | Medium |
| [unicornB/Supportly-Ai](https://github.com/unicornB/Supportly-Ai) | Plataforma de suporte ao cliente com IA nativa da Cloudflare. | Workers, Workers AI, knowledge base | Medium | Active | Medium |
| [G4brym/workers-research](https://github.com/G4brym/workers-research) | Agente serverless de pesquisa profunda. | Workers, Durable Objects | Medium | Active | Medium |
| [atinux/flux-ai-image-generator](https://github.com/atinux/flux-ai-image-generator) | App de geração de imagens com Flux na Cloudflare. | Workers AI, R2, NuxtHub | Easy | Active | Medium |
| [chipmates/agoracosmica](https://github.com/chipmates/agoracosmica) | Plataforma educacional de conversas com IA. | Workers, self-hosted app | Medium | Active | Medium |
| [devarshishimpi/codra](https://github.com/devarshishimpi/codra) | Revisão de código com IA para PRs do GitHub, self-hosted. | Workers, KV, Queues, Hyperdrive, Workers AI | Medium | Active | Medium |
| [bestian/askit-hono](https://github.com/bestian/askit-hono) | Respostas RAG citadas a partir do arquivo de transcrições de Audrey Tang. | Workers, Hono, Vectorize, Workers AI | Medium | Active | Medium |
| [Teycir/ArxivExplorer](https://github.com/Teycir/ArxivExplorer) | Busca semântica com IA para artigos do arXiv. | Workers, semantic search | Medium | Active | Medium |
| [IchimaruGin728/Gins-Blog](https://github.com/IchimaruGin728/Gins-Blog) | Blog na edge com busca por IA e OAuth. | Workers, D1, R2, KV, Hono | Medium | Active | Medium |

## Agents em Workers

| Projeto | O que faz | Stack Cloudflare | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [openma-ai/open-managed-agents](https://github.com/openma-ai/open-managed-agents) | Implementação self-hosted da API Claude Managed Agents. | Workers, Durable Objects | Medium | Active | Medium |
| [Logos-Flux/cloudflare-multiagent](https://github.com/Logos-Flux/cloudflare-multiagent) | Plataforma multiagente de IA em Workers. | Workers, AI generation | Medium | Active | Medium |
| [acoyfellow/flue-snippets](https://github.com/acoyfellow/flue-snippets) | Exemplos executáveis de agentes Flue com testes de deploy. | Workers, Durable Objects, Workers AI | Easy | Active | Low |
| [stukennedy/honi](https://github.com/stukennedy/honi) | Framework de IA agentic nativo da Cloudflare. | Durable Objects, Workers | Medium | Active | Medium |
| [acoyfellow/fleet-pattern](https://github.com/acoyfellow/fleet-pattern) | Padrão de agentes hierárquicos com Durable Objects. | Workers, Durable Objects | Medium | Stable | Low |
| [serpin-taxt/openchief](https://github.com/serpin-taxt/openchief) | Agentes que observam ferramentas de negócio e geram relatórios. | Workers, serverless runtime | Medium | Active | Medium |
| [huseynsnmz/postr](https://github.com/huseynsnmz/postr) | TUI de email keyboard-first com agente de IA. | Workers, Durable Objects, Email Routing, Workers AI | Hard | Active | Medium |
| [Ahmad-A0/iris-voice-agent](https://github.com/Ahmad-A0/iris-voice-agent) | Agente de voz em tempo real na edge. | Workers, Durable Objects | Hard | Active | Medium |
| [sinameraji/kimiflare](https://github.com/sinameraji/kimiflare) | Agente de programação no terminal rodando na Cloudflare. | Workers AI, AI Gateway | Medium | Active | Medium |
| [marceloeatworld/clopinette-ai](https://github.com/marceloeatworld/clopinette-ai) | Agente multimodal com memória e integrações de bots. | Workers, Durable Objects, Workers AI, AutoRAG | Hard | Active | Medium |

## MCP na Cloudflare

| Projeto | O que faz | Stack Cloudflare | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [rahilp/second-brain-cloudflare](https://github.com/rahilp/second-brain-cloudflare) | Camada de memória de IA self-hosted para clientes MCP. | Workers, D1, Vectorize | Medium | Active | Medium |
| [cyanheads/mcp-ts-core](https://github.com/cyanheads/mcp-ts-core) | Framework TypeScript para servidores MCP com suporte a Workers. | Cloudflare Workers runtime | Medium | Active | Low |
| [Puliczek/mcp-memory](https://github.com/Puliczek/mcp-memory) | Servidor MCP de memória para preferências e recall. | Workers, D1, Vectorize | Medium | Active | Medium |
| [Yrobot/cloudflare-search](https://github.com/Yrobot/cloudflare-search) | Servidor de busca que pode ampliar ferramentas de IA via MCP. | Workers, MCP | Medium | Active | Medium |
| [stytchauth/mcp-stytch-consumer-todo-list](https://github.com/stytchauth/mcp-stytch-consumer-todo-list) | Servidor MCP de TODO app com exemplo de autenticação. | Workers, MCP, Stytch | Medium | Active | Medium |
| [dinasaur404/BestReads-MCP-Server](https://github.com/dinasaur404/BestReads-MCP-Server) | Servidor MCP remoto construído com Workers. | Workers, MCP | Medium | Active | Medium |
| [omarshahine/fastmail-mcp-remote](https://github.com/omarshahine/fastmail-mcp-remote) | MCP remoto para Fastmail com Cloudflare Access OAuth. | Workers, Access OAuth, MCP | Medium | Active | Medium |

## Armazenamento e memória

| Projeto | O que faz | Stack Cloudflare | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [TimeSurgeLabs/athenadb](https://github.com/TimeSurgeLabs/athenadb) | API serverless de banco vetorial. | Workers, D1, Vectorize, Workers AI | Medium | Stable | Medium |
| [elizabethsiegle/art-vector-search-cloudflare](https://github.com/elizabethsiegle/art-vector-search-cloudflare) | Busca de arte usando Vectorize e Workers AI. | Vectorize, Workers AI, AI Gateway | Medium | Stable | Medium |
| [synapse-ai-labs/synapse-api](https://github.com/synapse-ai-labs/synapse-api) | API serverless de embeddings com Vectorize e OpenAI. | Workers, D1, Vectorize | Medium | Stable | Medium |
| [adam0white/MessageAI](https://github.com/adam0white/MessageAI) | App de mensagens em tempo real com RAG e agentes. | Workers, Durable Objects, Vectorize, Workers AI | Hard | Active | Medium |

## Templates e starters

| Projeto | O que faz | Stack Cloudflare | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [louisbrulenaudet/genai-api](https://github.com/louisbrulenaudet/genai-api) | Template Workers + Gemini API. | Workers, AI Gateway, Hono | Easy | Active | Medium |
| [nuxt-hub/core](https://github.com/nuxt-hub/core) | Módulo Nuxt com banco, KV, blob storage, cache e IA. | D1, KV, R2, Workers AI | Medium | Active | Low |
| [JSONbored/opennextjs-cli](https://github.com/JSONbored/opennextjs-cli) | CLI/TUI para OpenNext.js em Workers com recursos MCP. | Workers, OpenNext, MCP | Medium | Active | Low |
| [acoyfellow/svelte-edge](https://github.com/acoyfellow/svelte-edge) | UI Svelte gerada por agente e compilada em Workers. | Workers, Hono, Workers AI | Medium | Active | Medium |
| [Geekgineer/needle-rs](https://github.com/Geekgineer/needle-rs) | Runtime WASM pequeno para transformer com tool-calling. | Workers, WASM | Hard | Active | Low |

## Observabilidade e ops

| Projeto | O que faz | Stack Cloudflare | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [PoemMisty/CF-Request-Analytics-Panel](https://github.com/PoemMisty/CF-Request-Analytics-Panel) | Painel de analytics de requisições para múltiplas contas Cloudflare. | Workers, analytics APIs | Medium | Active | Medium |
| [bgdnvk/clanker](https://github.com/bgdnvk/clanker) | Agente CLI autônomo de engenharia de sistemas para nuvem. | Cloudflare support, Workers topics | Hard | Active | Medium |

## Use com cuidado

Estes projetos podem ser úteis para aprendizado ou self-hosting, mas envolvem padrões sensíveis como mensagens anônimas, busca pública, email, limites de políticas de provedores ou acesso privilegiado a contas. Revise código, permissões, logs, controles de abuso e termos dos provedores antes de implantar.

| Projeto | O que faz | Stack Cloudflare | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [Vauth/duckgpt](https://github.com/Vauth/duckgpt) | App de chat com acesso a modelos no estilo Workers AI. | Workers AI, Workers | Medium | Use with care | High |

## Critérios de seleção

### Obrigatório

- Código open source, ou ao menos núcleo auditável.
- Relação clara com Workers, Pages, Workers AI, AI Gateway, D1, KV, R2, Vectorize, Durable Objects, Queues, Email Routing, Turnstile ou APIs da conta Cloudflare.
- README ou docs explicando propósito e setup básico.
- Não ser apenas uma página de marketing.

### Preferido

- Commits, releases, respostas em issues ou atividade de PR recente.
- Configuração `wrangler`, deploy em um clique ou documentação passo a passo para Cloudflare.
- Demo, screenshots, notas de arquitetura ou testes.
- Variáveis de ambiente, permissões, custos e notas de segurança claros.

### Fora da lista

- Repositórios só com ideias e sem código executável.
- Serviços fechados.
- Repositórios que só mencionam Cloudflare de passagem.
- Projetos de abuso, bypass, roubo de credenciais ou evasão de políticas.
- Projetos arquivados ou sem manutenção, salvo quando ainda forem referências úteis.

## Contribuição

Pull requests são bem-vindos. Leia [CONTRIBUTING.md](../CONTRIBUTING.md) antes de sugerir um projeto.

Ao adicionar um projeto, inclua:

- O que ele faz.
- Quais componentes Cloudflare usa.
- Dificuldade de deploy.
- Status de manutenção.
- Riscos ou notas de segurança.

## Licença

MIT. Veja [LICENSE](../LICENSE).
