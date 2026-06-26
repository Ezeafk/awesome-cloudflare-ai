# Awesome Cloudflare AI

> Kuratierte Open-Source-Projekte für AI, Agent, MCP, Workers AI, D1, R2, Vectorize und Durable Objects, die auf Cloudflare deploybar sind.

Sprachen: [English](../README.md) | [简体中文](README.zh-CN.md) | [Português do Brasil](README.pt-BR.md) | [日本語](README.ja.md) | [Deutsch](README.de.md) | [Русский](README.ru.md)

Ein streng kuratiertes Verzeichnis für Cloudflare AI / Agent / MCP Open-Source-Projekte. Dies ist keine allgemeine KI-Toolliste, sondern enthält nur Projekte mit klarem Bezug zu Cloudflare-Deployment, Runtime oder Dateninfrastruktur.

Zuletzt geprüft: 2026-06-26

## Warum diese Liste

Cloudflare Workers, Pages, D1, KV, R2, Vectorize, Durable Objects, Workers AI, AI Gateway und Queues werden zu wichtigen Bausteinen für kostengünstige KI-Apps und Agents. Diese Liste fokussiert sich auf drei Punkte:

- Deploybar: Das Projekt läuft auf Cloudflare oder seine Kernarchitektur hängt klar von Cloudflare ab.
- Überprüfbar: README, Konfigurationen, Beispiele oder Dokumentation machen Zweck und Deployment-Pfad nachvollziehbar.
- Gepflegt: Projekte mit aktuellen Wartungssignalen werden bevorzugt.

## Legende

| Feld | Werte |
|---|---|
| Deploy | Easy = One-Click-Deploy oder klare Befehle; Medium = mehrere Services/API keys; Hard = Architekturverständnis oder Codeänderungen nötig |
| Status | Active = klare Wartung in den letzten 6 Monaten; Stable = weniger aktuell, aber weiterhin nützlich; Use with care = Risiko für Sicherheit, Compliance, Datenschutz oder Missbrauch |
| Risk | Low = normale App/Vorlage; Medium = Nutzerdaten, API keys, Dateien, Accounts oder Automatisierung; High = Proxy, Anonymität, Umgehung, Crawling oder ähnlich sensible Nutzung |

## Bewertungsmethode

Projekte werden vor der Aufnahme bewertet. Stars sind nur ein schwaches Signal; ein neues Projekt kann aufgenommen werden, wenn es klar Cloudflare-relevant, deploybar, dokumentiert und sicher genug ist.

| Bereich | Punkte | Prüfung |
|---|---:|---|
| Cloudflare-Relevanz | 0-3 | Direkte Nutzung von Workers, Pages, Workers AI, AI Gateway, D1, KV, R2, Vectorize, Durable Objects, Queues, Email Routing, Turnstile oder Cloudflare APIs. |
| Deployability | 0-2 | Klarer Deploy-Pfad, wrangler config, template, demo oder setup instructions. |
| Wartung | 0-2 | Aktuelle commits, releases, issue replies oder aktive community use. |
| Dokumentation und Lizenz | 0-2 | Klares README, environment variables, architecture notes und auditierbare license. |
| Sicherheit | 0-1 | Sinnvolle Grenzen für auth, user data, uploads, automation, proxies, email oder privileged APIs. |

Aufnahmeleitlinie: 8-10 = empfohlen, 6-7 = akzeptabel mit Hinweisen, 4-5 = use with care oder erneut prüfen, unter 4 = entfernen oder nicht aufnehmen. High-risk Projekte brauchen einen stärkeren Score und klare Sicherheitshinweise.

## Inhalt

- [Offiziell und Kernprojekte](#offiziell-und-kernprojekte)
- [KI-Apps auf Cloudflare](#ki-apps-auf-cloudflare)
- [Agents auf Workers](#agents-auf-workers)
- [MCP auf Cloudflare](#mcp-auf-cloudflare)
- [Storage und Memory](#storage-und-memory)
- [Templates und Starter](#templates-und-starter)
- [Observability und Ops](#observability-und-ops)
- [Mit Vorsicht nutzen](#mit-vorsicht-nutzen)
- [Bewertungsmethode](#bewertungsmethode)
- [Auswahlkriterien](#auswahlkriterien)
- [Mitwirken](#mitwirken)

## Offiziell und Kernprojekte

| Projekt | Zweck | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [cloudflare/agents](https://github.com/cloudflare/agents) | Offizielles SDK zum Erstellen und Deployen von AI Agents. | Workers, Durable Objects, Workflows | Medium | Active | Low |
| [cloudflare/ai](https://github.com/cloudflare/ai) | Offizielle Workers-AI-Beispiele, Demos und Pakete. | Workers AI, Workers | Easy | Active | Low |
| [cloudflare/mcp-server-cloudflare](https://github.com/cloudflare/mcp-server-cloudflare) | Offizieller MCP-Server für Cloudflare-Account-Ressourcen. | MCP, Workers/KV/R2/DNS APIs | Medium | Active | Medium |
| [cloudflare/templates](https://github.com/cloudflare/templates) | Offizielle Workers-Templates für Apps und APIs. | Workers, Pages, D1, KV, R2 | Easy | Active | Low |
| [cloudflare/workers-chat-demo](https://github.com/cloudflare/workers-chat-demo) | Offizielle Realtime-Chat-Demo für Edge-Apps. | Workers, Durable Objects | Medium | Active | Medium |
| [cloudflare/workers-sdk](https://github.com/cloudflare/workers-sdk) | Wrangler und Toolchain für Workers-Entwicklung. | Workers, Wrangler | Medium | Active | Low |

## KI-Apps auf Cloudflare

| Projekt | Zweck | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [cloudflare/vibesdk](https://github.com/cloudflare/vibesdk) | Open-Source-Vibe-Coding-Plattform auf Cloudflare. | Workers, Durable Objects | Medium | Active | Medium |
| [Jazee6/cloudflare-ai-web](https://github.com/Jazee6/cloudflare-ai-web) | Cloudflare-AI-Webplattform mit One-Click-Deploy. | Workers AI, Pages/Workers | Easy | Active | Medium |
| [miantiao-me/hacker-podcast](https://github.com/miantiao-me/hacker-podcast) | KI-generierter chinesischer Podcast aus Hacker News. | Workers, Workflows | Medium | Active | Medium |
| [nicholasgriffintn/ai-platform](https://github.com/nicholasgriffintn/ai-platform) | Multi-Model-Plattform für persönliche KI-Assistenten. | Workers, AI Gateway, Hono | Medium | Active | Medium |
| [unicornB/Supportly-Ai](https://github.com/unicornB/Supportly-Ai) | Cloudflare-native KI-Plattform für Kundensupport. | Workers, Workers AI, knowledge base | Medium | Active | Medium |
| [G4brym/workers-research](https://github.com/G4brym/workers-research) | Serverless Deep-Research-Agent. | Workers, Durable Objects | Medium | Active | Medium |
| [atinux/flux-ai-image-generator](https://github.com/atinux/flux-ai-image-generator) | Bildgenerierungs-App mit Flux auf Cloudflare. | Workers AI, R2, NuxtHub | Easy | Active | Medium |
| [chipmates/agoracosmica](https://github.com/chipmates/agoracosmica) | Bildungsplattform für KI-Gespräche. | Workers, self-hosted app | Medium | Active | Medium |
| [devarshishimpi/codra](https://github.com/devarshishimpi/codra) | Self-hosted KI-Code-Review für GitHub PRs. | Workers, KV, Queues, Hyperdrive, Workers AI | Medium | Active | Medium |
| [bestian/askit-hono](https://github.com/bestian/askit-hono) | Zitierte RAG-Antworten aus dem Audrey-Tang-Transkriptarchiv. | Workers, Hono, Vectorize, Workers AI | Medium | Active | Medium |
| [Teycir/ArxivExplorer](https://github.com/Teycir/ArxivExplorer) | KI-gestützte semantische Suche für arXiv-Paper. | Workers, semantic search | Medium | Active | Medium |
| [IchimaruGin728/Gins-Blog](https://github.com/IchimaruGin728/Gins-Blog) | Edge-Blog mit KI-Suche und OAuth. | Workers, D1, R2, KV, Hono | Medium | Active | Medium |

## Agents auf Workers

| Projekt | Zweck | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [openma-ai/open-managed-agents](https://github.com/openma-ai/open-managed-agents) | Self-hosted Implementierung der Claude Managed Agents API. | Workers, Durable Objects | Medium | Active | Medium |
| [Logos-Flux/cloudflare-multiagent](https://github.com/Logos-Flux/cloudflare-multiagent) | Multi-Agent-KI-Plattform auf Workers. | Workers, AI generation | Medium | Active | Medium |
| [acoyfellow/flue-snippets](https://github.com/acoyfellow/flue-snippets) | Ausführbare Flue-Agent-Beispiele mit Deploy-Tests. | Workers, Durable Objects, Workers AI | Easy | Active | Low |
| [stukennedy/honi](https://github.com/stukennedy/honi) | Cloudflare-natives agentic-AI-Framework. | Durable Objects, Workers | Medium | Active | Medium |
| [acoyfellow/fleet-pattern](https://github.com/acoyfellow/fleet-pattern) | Hierarchisches Durable-Object-Agent-Pattern. | Workers, Durable Objects | Medium | Stable | Low |
| [serpin-taxt/openchief](https://github.com/serpin-taxt/openchief) | Agents, die Business-Tools beobachten und Reports erstellen. | Workers, serverless runtime | Medium | Active | Medium |
| [huseynsnmz/postr](https://github.com/huseynsnmz/postr) | Keyboard-first E-Mail-TUI mit KI-Agent. | Workers, Durable Objects, Email Routing, Workers AI | Hard | Active | Medium |
| [Ahmad-A0/iris-voice-agent](https://github.com/Ahmad-A0/iris-voice-agent) | Realtime-Voice-Agent an der Edge. | Workers, Durable Objects | Hard | Active | Medium |
| [sinameraji/kimiflare](https://github.com/sinameraji/kimiflare) | Terminal-Coding-Agent auf dem eigenen Cloudflare-Account. | Workers AI, AI Gateway | Medium | Active | Medium |
| [marceloeatworld/clopinette-ai](https://github.com/marceloeatworld/clopinette-ai) | Multimodaler Agent mit Memory und Bot-Integrationen. | Workers, Durable Objects, Workers AI, AutoRAG | Hard | Active | Medium |

## MCP auf Cloudflare

| Projekt | Zweck | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [rahilp/second-brain-cloudflare](https://github.com/rahilp/second-brain-cloudflare) | Self-hosted KI-Memory-Layer für MCP-Clients. | Workers, D1, Vectorize | Medium | Active | Medium |
| [cyanheads/mcp-ts-core](https://github.com/cyanheads/mcp-ts-core) | TypeScript-Framework für MCP-Server mit Workers-Support. | Cloudflare Workers runtime | Medium | Active | Low |
| [Puliczek/mcp-memory](https://github.com/Puliczek/mcp-memory) | MCP-Memory-Server für Nutzerpräferenzen und Recall. | Workers, D1, Vectorize | Medium | Active | Medium |
| [Yrobot/cloudflare-search](https://github.com/Yrobot/cloudflare-search) | Suchserver, der KI-Tools per MCP erweitern kann. | Workers, MCP | Medium | Active | Medium |
| [stytchauth/mcp-stytch-consumer-todo-list](https://github.com/stytchauth/mcp-stytch-consumer-todo-list) | TODO-App-MCP-Server mit Auth-Beispiel. | Workers, MCP, Stytch | Medium | Active | Medium |
| [dinasaur404/BestReads-MCP-Server](https://github.com/dinasaur404/BestReads-MCP-Server) | Remote-MCP-Server auf Workers. | Workers, MCP | Medium | Active | Medium |
| [omarshahine/fastmail-mcp-remote](https://github.com/omarshahine/fastmail-mcp-remote) | Fastmail-Remote-MCP mit Cloudflare Access OAuth. | Workers, Access OAuth, MCP | Medium | Active | Medium |

## Storage und Memory

| Projekt | Zweck | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [TimeSurgeLabs/athenadb](https://github.com/TimeSurgeLabs/athenadb) | Serverless Vektordatenbank-API. | Workers, D1, Vectorize, Workers AI | Medium | Stable | Medium |
| [elizabethsiegle/art-vector-search-cloudflare](https://github.com/elizabethsiegle/art-vector-search-cloudflare) | Kunstsuche mit Vectorize und Workers AI. | Vectorize, Workers AI, AI Gateway | Medium | Stable | Medium |
| [synapse-ai-labs/synapse-api](https://github.com/synapse-ai-labs/synapse-api) | Serverless Embeddings API mit Vectorize und OpenAI. | Workers, D1, Vectorize | Medium | Stable | Medium |
| [adam0white/MessageAI](https://github.com/adam0white/MessageAI) | Realtime-Messaging-App mit RAG und Agents. | Workers, Durable Objects, Vectorize, Workers AI | Hard | Active | Medium |

## Templates und Starter

| Projekt | Zweck | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [louisbrulenaudet/genai-api](https://github.com/louisbrulenaudet/genai-api) | Workers + Gemini API Template. | Workers, AI Gateway, Hono | Easy | Active | Medium |
| [nuxt-hub/core](https://github.com/nuxt-hub/core) | Nuxt-Modul für DB, KV, Blob Storage, Cache und KI-Integrationen. | D1, KV, R2, Workers AI | Medium | Active | Low |
| [JSONbored/opennextjs-cli](https://github.com/JSONbored/opennextjs-cli) | CLI/TUI für OpenNext.js auf Workers mit MCP-Funktionen. | Workers, OpenNext, MCP | Medium | Active | Low |
| [acoyfellow/svelte-edge](https://github.com/acoyfellow/svelte-edge) | Agent-generierte Svelte-UI, auf Workers kompiliert. | Workers, Hono, Workers AI | Medium | Active | Medium |
| [Geekgineer/needle-rs](https://github.com/Geekgineer/needle-rs) | Kleine WASM-Runtime für tool-calling Transformer. | Workers, WASM | Hard | Active | Low |

## Observability und Ops

| Projekt | Zweck | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [PoemMisty/CF-Request-Analytics-Panel](https://github.com/PoemMisty/CF-Request-Analytics-Panel) | Request-Analytics-Panel für mehrere Cloudflare-Accounts. | Workers, analytics APIs | Medium | Active | Medium |
| [bgdnvk/clanker](https://github.com/bgdnvk/clanker) | Autonomer Systems-Engineering-CLI-Agent für Cloud-Umgebungen. | Cloudflare support, Workers topics | Hard | Active | Medium |

## Mit Vorsicht nutzen

Diese Projekte können zum Lernen oder Self-Hosting nützlich sein, enthalten aber sensible Muster wie anonyme Nachrichten, öffentliche Suche, E-Mail, Provider-Policy-Grenzen oder privilegierten Accountzugriff. Prüfe Code, Berechtigungen, Logging, Missbrauchsschutz und Upstream-Bedingungen vor dem Deployment.

| Projekt | Zweck | Cloudflare Stack | Deploy | Status | Risk |
|---|---|---|---|---|---|
| [Vauth/duckgpt](https://github.com/Vauth/duckgpt) | Chat-App mit Workers-AI-artigem Modellzugriff. | Workers AI, Workers | Medium | Use with care | High |

## Auswahlkriterien

### Muss erfüllt sein

- Open-Source-Code oder mindestens auditierbarer Kerncode.
- Klarer Bezug zu Workers, Pages, Workers AI, AI Gateway, D1, KV, R2, Vectorize, Durable Objects, Queues, Email Routing, Turnstile oder Cloudflare-Account-APIs.
- README oder Dokumentation erklärt Zweck und Basiseinrichtung.
- Keine reine Marketingseite.

### Bevorzugt

- Aktuelle Commits, Releases, Issue-Antworten oder PR-Aktivität.
- `wrangler`-Konfiguration, One-Click-Deploy oder Schritt-für-Schritt-Cloudflare-Deployment.
- Demo, Screenshots, Architekturnotizen oder Tests.
- Klare Angaben zu Umgebungsvariablen, Berechtigungen, Kosten und Sicherheit.

### Nicht aufgenommen

- Reine Ideen-Repos ohne lauffähigen Code.
- Closed-Source-Dienste.
- Repos, die Cloudflare nur beiläufig erwähnen.
- Offensichtlicher Missbrauch, Bypass, Credential Theft oder Policy-Evasion.
- Archivierte oder ungepflegte Projekte, außer sie haben klaren Referenzwert.

## Mitwirken

Pull Requests sind willkommen. Bitte lies [CONTRIBUTING.md](../CONTRIBUTING.md), bevor du ein Projekt vorschlägst.

Beim Hinzufügen eines Projekts bitte angeben:

- Was es macht.
- Welche Cloudflare-Komponenten es nutzt.
- Deployment-Schwierigkeit.
- Wartungsstatus.
- Risiken oder Sicherheitshinweise.

## Lizenz

MIT. Siehe [LICENSE](../LICENSE).
