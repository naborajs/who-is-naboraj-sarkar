# Naboraj Sarkar — Developer Portfolio

<p align="center">
  <strong>Naboraj Sarkar</strong> (Nishant) — Developer, AI practitioner, and automation engineer.
  <br>
  Location: Siliguri, West Bengal, India 🇮🇳 • Online: @naborajs
</p>

I build audit-friendly automations, Telegram/WhatsApp bots with GitHub logging, and AI agents used in real-world deployments. This repository is a public, searchable record of those projects, technical notes, and learning resources (NSCodex).

---

## Table of contents

- About — who I am and what I build
- Featured projects — technical summaries and stacks
- Architecture highlights — diagrams and example flows
- Deployments & operations — hosting, monitoring, and reliability
- Skills & tech stack — concrete technologies I use
- How to collaborate — contact, demos, and contribution
- SEO keywords & meta suggestions (for web landing pages)
- License

---

## About

I’m a pragmatic builder who prefers reproducible work and measurable outcomes. I publish my experiments publicly so others can learn from the design, failure modes, and operational details. I focus on:

- AI agents and retrieval-based memory systems
- Automation with n8n and custom runners
- Integrations: Telegram, WhatsApp, GitHub-based logging
- Education through NSCodex: project-first, hands-on learning

Quote: “Build in public, document the failures, and make tools that others can reuse.”

---

## Recent highlights (quick)

- Life Logger — Telegram bot → captures structured activity, creates commits in a GitHub repo for every entry (audit-ready personal logs).
- AI Pro Sales Assistant — memory-enabled agent for sales/support with admin dashboard and multi-channel integration.
- CODE — experimental AI-powered IDE for rapid scaffolding using multiple LLM providers.
- NS Fin — crypto & market intelligence dashboard (educational, not financial advice).

---

## Featured projects — technical summaries

### Life Logger — Telegram bot with GitHub integration

- Type: Bot / Integration
- Stack: Python/Node.js, Telegram Bot API, GitHub REST API, webhooks
- Architecture (summary): Telegram webhook → capture service → normalization → GitHub commit API (JSON/MD) → optional static UI on Vercel
- Value: auditable personal logs, versioned notes for habits and compliance

### AI Pro Sales Assistant

- Type: AI agent / Automation
- Stack: LLMs (OpenAI/Gemini/Anthropic), retrieval (vector DB), webhook connectors (Telegram/WhatsApp), admin UI (React)
- Features: memory layers, human-in-the-loop overrides, analytics, continuous updates from new conversations

### CODE — AI-assisted online IDE (prototype)

- Type: Web app / Productivity tool
- Stack: React frontend, Node/Flask backend, configurable LLM providers
- Notes: supports user-supplied API keys, multi-model prompt orchestration, scaffold generation

### NS Fin — Finance & Crypto Intelligence (educational)

- Type: Data aggregation & dashboard
- Stack: Market APIs, data pipelines, visualization, sentiment analysis
- Focus: research and education — not investment advice

---

## Architecture highlights — examples

Life Logger flow (example):

1. Telegram bot receives message → webhook posts to capture endpoint
2. Capture service normalizes message to JSON and validates schema
3. Commit generator prepares a content file and calls GitHub REST API to create a commit in a dedicated logging repo
4. Optional: static UI renders logs from the repo via Vercel for quick browsing

Design principles: idempotence for webhooks, small single-purpose services, clear auditability (git commits), and defensive retries.

---

## Deployments & operations

- Hosting: Vercel / Netlify for static sites and lightweight front-ends
- Automations: n8n hosted or self-hosted runners for scheduled workflows
- Monitoring: structured logs, Git-backed changes, and simple alerting (email/Telegram)
- Reliability: exponential backoff on external APIs, circuit-breakers for LLM calls, minimal privileged credentials

---

## Skills & tech stack

- Languages: Python (primary), JavaScript/Node.js, basic C++
- Web: HTML/CSS, React for small admin UIs
- APIs: REST, webhooks, GitHub API, Telegram Bot API
- Automation: n8n, cron, webhook orchestration
- AI: prompt engineering, retrieval systems, multi-model orchestration
- Deployment: Vercel, Netlify, simple CI patterns

---

## How to collaborate

- Quick demo / bot walkthrough: Telegram — @Nishantsarkar10k
- Business/proposal: nishant.ns.business@gmail.com
- Code, issues, PRs: https://github.com/naborajs

If you want a technical walkthrough (architecture diagram, deployment notes, or code pointers), open an issue in the relevant repository and tag me.

---

## SEO keywords & meta suggestions (for publishing this page on a website)

- Meta title suggestion: "Naboraj Sarkar — Developer Portfolio · AI Agents · Automation · NSCodex"
- Meta description suggestion: "Naboraj Sarkar (Nishant) — Developer focused on AI agents, Telegram bots with GitHub logging, and automation. Projects: Life Logger, AI Pro Sales Assistant, NSCodex."
- Primary keywords: Naboraj Sarkar, Life Logger Telegram bot, AI agent development, n8n automation, NSCodex, Telegram GitHub integration
- Structured data suggestion (JSON-LD): add Organization/Person schema on your website landing page to improve search visibility

---

## Getting started (for contributors)

1. Browse `PROJECTS.md` to find a project you want to work on.
2. Open an issue describing the improvement or feature.
3. Fork, implement, and open a pull request with a clear description and a short deployment checklist.

Contribution preferences: small, focused PRs, clear tests or manual verification steps, and documentation updates.

---

## License

This repository content is provided under the MIT License.

© 2026 Naboraj Sarkar
