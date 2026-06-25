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
- [ ] Deploy, status, and risk fields are filled.
- [ ] Safety caveats are included for sensitive projects.
- [ ] Link check passes.
