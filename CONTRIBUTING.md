# Contributing

Thanks for helping improve Awesome Cloudflare AI.

This list values judgment over volume. Please do not submit a large batch of links without checking whether each project is actually useful, deployable, and relevant to Cloudflare.

## Before Submitting

Make sure the project:

- Is open source, or has auditable core code.
- Has a clear Cloudflare connection.
- Has setup, deployment, or runtime documentation.
- Is not a pure marketing page.
- Is not obviously abandoned, archived, or broken.

## Entry Format

Use the existing table format:

```md
| [Project](https://github.com/owner/repo) | Short description. | Workers, D1 | Medium | Active | Medium |
```

Keep descriptions factual and compact.

## Evaluation Score

Every new project should be scored before it is added. Stars are only a weak signal; reviewers should prioritize usefulness, deployability, documentation, and safety.

| Area | Points | Review focus |
|---|---:|---|
| Cloudflare relevance | 0-3 | Direct use of Workers, Pages, Workers AI, AI Gateway, D1, KV, R2, Vectorize, Durable Objects, Queues, Email Routing, Turnstile, or Cloudflare APIs. |
| Deployability | 0-2 | Clear deploy path, wrangler config, template, demo, or setup instructions. |
| Maintenance | 0-2 | Recent commits, releases, issue replies, or active community use. |
| Documentation and license | 0-2 | Clear README, environment variables, architecture notes, and auditable license. |
| Safety | 0-1 | Reasonable boundaries for auth, user data, uploads, automation, proxies, email, or privileged APIs. |

Inclusion guide:

- 8-10: recommended.
- 6-7: acceptable with caveats.
- 4-5: use with care or re-review.
- Below 4: remove or do not include.

## Status Guide

- Active: recent commit, release, issue reply, or PR activity within roughly 6 months.
- Stable: less recent activity, but still useful and not archived.
- Use with care: sensitive data, privileged APIs, anonymous workflows, public upload/search, email, proxy-like behavior, or policy-sensitive use.

## Deploy Guide

- Easy: one-click deploy, template, or short documented command path.
- Medium: requires multiple services, API keys, OAuth setup, or Cloudflare resources.
- Hard: requires architecture understanding, code changes, migrations, or production security review.

## Risk Guide

- Low: ordinary app, template, SDK, demo, or framework.
- Medium: handles user data, API keys, files, account permissions, workflow automation, or agent actions.
- High: anonymous messaging, email access, scraping, proxy behavior, authless demos, privileged integrations, or any pattern that needs explicit abuse controls.

## PR Checklist

- [ ] Link points to the canonical project repository.
- [ ] Project is open source or core code is auditable.
- [ ] Cloudflare stack is listed accurately.
- [ ] Evaluation score is at least 6, or the PR explains why a lower-scoring project is still worth tracking.
- [ ] Deploy, status, and risk fields are filled.
- [ ] Safety caveats are included for sensitive projects.
- [ ] Link check passes.
