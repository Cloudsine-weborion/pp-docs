# GenAI Protector Plus — Documentation

[![Built with Mintlify](https://img.shields.io/badge/Built%20with-Mintlify-0E9F6E)](https://mintlify.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

Public documentation site for **CloudsineAI's GenAI Protector Plus** — a runtime AI security platform that sits inline between GenAI applications and their LLM endpoints, providing defence-in-depth detection for prompt injection, PII leakage, unsafe content, and agentic threats.

Built with [Mintlify](https://mintlify.com).

## Local preview

Requires Node.js 18+.

```bash
npm i -g mintlify
mintlify dev
```

The site is served at <http://localhost:3000>. MDX edits hot-reload; changes to `docs.json` require restarting the server.

## Structure

| Path | Contents |
| --- | --- |
| `docs.json` | Mintlify config — theme, navigation, navbar, footer. |
| `introduction/` | Overview, key concepts, quickstart. |
| `architecture/` | System overview, deployment modes, detection layers, ShieldPrompt, TVDB. |
| `deployment/` | AWS Marketplace, Kubernetes/Helm, on-premises, network prerequisites. |
| `user-guide/` | Setup, security profiles, guardrails, protection levels, threat management, SIEM. |
| `benchmarks/` | Accuracy and performance results. |
| `api-reference/` | REST API endpoints, authentication, integration patterns. |
| `logo/`, `images/` | Brand assets and screenshots. |
| `snippets/` | Reusable MDX fragments. |

## Editing

- Pages are MDX. Mintlify components (`<Card>`, `<CardGroup>`, `<Steps>`, `<Accordion>`, `<Frame>`, `<Tabs>`) are available out of the box — see [Mintlify docs](https://mintlify.com/docs).
- Diagrams use Mermaid via fenced code blocks (` ```mermaid `).
- Navigation order is defined in `docs.json` under `navigation.tabs[].groups[].pages` — add a new MDX file *and* register it here.

## Branding

| Token | Value |
| --- | --- |
| Primary | `#1F3864` (Cloudsine navy) |
| Light | `#00B5E2` (Cloudsine cyan) |
| Dark | `#0F1E3A` |
| Font | Inter |
| Primary CTA | "Get an API Key" → <https://www.cloudsine.tech/contact> |

## Deployment

Mintlify auto-deploys on push to the default branch once the repo is connected at <https://dashboard.mintlify.com>.

1. Push this repo to GitHub.
2. Sign in to the Mintlify dashboard and connect the repo.
3. Configure a custom domain (e.g. `docs.cloudsine.tech`) once DNS is ready.

## Contributing

- All API examples must use `<YOUR_API_KEY>` and `<your-protector-plus-host>` placeholders.
- Never commit live API keys, bearer tokens, or backend URLs. Sandbox keys are issued via the contact form.
- Run `mintlify dev` locally before opening a PR; surface any broken-link or nav warnings in the description.

## License

Released under the [MIT License](./LICENSE). © 2026 Cloudsine Pte Ltd.

The "CloudsineAI" and "GenAI Protector Plus" names and logos are trademarks of Cloudsine Pte Ltd and are not licensed for reuse.
