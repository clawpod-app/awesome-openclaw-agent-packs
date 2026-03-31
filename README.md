[English](./README.md) | [中文](./README.zh-CN.md) | [日本語](./README.ja.md) | [Español](./README.es.md) | [Deutsch](./README.de.md)

# Awesome OpenClaw Agent Packs

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![GitHub stars](https://img.shields.io/github/stars/clawpod-app/awesome-openclaw-agent-packs?style=social)](https://github.com/clawpod-app/awesome-openclaw-agent-packs)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/clawpod-app/awesome-openclaw-agent-packs/pulls)
[![Packs](https://img.shields.io/badge/Packs-30-blue)](./packs/)
[![Skills](https://img.shields.io/badge/Skills-131-purple)](./packs/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](./LICENSE)

**Pre-configured AI agent packs for OpenClaw. Pick a role, deploy in 30 seconds.**

> :rocket: [Browse all packs](https://clawpod.app/templates?utm_source=github&utm_medium=readme&utm_campaign=browse) | :zap: [Deploy in 30 seconds](https://clawpod.app?utm_source=github&utm_medium=readme&utm_campaign=deploy) | :book: [What is OpenClaw?](https://clawpod.app/blog/what-is-openclaw?utm_source=github&utm_medium=readme&utm_campaign=learn)

---

## Contents

- [Available Packs](#available-packs)
- [Why OpenClaw?](#why-openclaw)
- [Quick Start](#quick-start)
- [How Skills Work](#how-skills-work)
- [Tutorials & Guides](#tutorials--guides)
- [Contributing](#contributing)
- [Attribution](#attribution)
- [License](#license)

---

## Available Packs

Each pack turns a generic OpenClaw agent into a specialized team member. Every pack includes 6 definition files (`SOUL.md`, `AGENTS.md`, `HEARTBEAT.md`, `TOOLS.md`, `MEMORY.md`, `README.md`) plus a full `skills/` directory.

| Pack | Skills | When to Use | Deploy |
|------|:------:|-------------|--------|
| :briefcase: [Sales Co-Pilot](./packs/sales/) | 9 | Prospect research, call prep, outreach drafting, pipeline reviews | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/sales?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :wrench: [Engineering Co-Pilot](./packs/engineering/) | 10 | Standups, code reviews, incident response, architecture decisions | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/engineering?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :bar_chart: [Data Analyst](./packs/data/) | 10 | SQL queries, dashboards, data quality checks, ad-hoc analysis | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/data?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :mega: [Marketing Strategist](./packs/marketing/) | 8 | Campaign planning, content calendars, SEO briefs, competitor analysis | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/marketing?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :scales: [Legal Analyst](./packs/legal/) | 9 | Contract review, compliance checks, risk assessments, policy drafting | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/legal?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :moneybag: [Finance Analyst](./packs/finance/) | 8 | Financial modeling, expense tracking, budget forecasts, audit prep | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/finance?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :clipboard: [Product Manager](./packs/product-management/) | 8 | PRDs, sprint planning, user story writing, feature prioritization | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/product-management?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :people_holding_hands: [HR Partner](./packs/human-resources/) | 9 | Hiring workflows, onboarding checklists, policy Q&A, performance reviews | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/human-resources?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :headphones: [Customer Support](./packs/customer-support/) | 5 | Ticket triage, FAQ answers, escalation handling, satisfaction tracking | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/customer-support?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :art: [Design Partner](./packs/design/) | 7 | Design critiques, UX audits, style guide enforcement, wireframe feedback | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/design?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :gear: [Operations Manager](./packs/operations/) | 9 | Process optimization, vendor management, SOP drafting, KPI tracking | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/operations?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |

#### Community-Sourced Packs

The following packs are curated from high-quality MIT-licensed community repos, with full attribution.

| Pack | Skills | When to Use | Source | Deploy |
|------|:------:|-------------|--------|--------|
| :rocket: [DevOps Guardian](./packs/devops/) | 3 | CI/CD monitoring, deploy rollbacks, incident response, infrastructure audits | [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/devops?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :pencil2: [Copywriter](./packs/copywriting/) | 3 | Ad copy, landing pages, email campaigns, brand voice consistency | [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/copywriting?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :mortar_board: [Education Tutor](./packs/education/) | 2 | Personalized tutoring, quiz generation, learning plans, study guides | [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/education?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :house: [Personal Assistant](./packs/personal-assistant/) | 2 | Daily planning, reminders, travel research, life admin tasks | [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/personal-assistant?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :shopping_cart: [E-Commerce Manager](./packs/ecommerce/) | 3 | Pricing optimization, inventory tracking, review management | [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/ecommerce?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :shield: [Security Analyst](./packs/security/) | 3 | Threat monitoring, vulnerability scanning, compliance audits | [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/security?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :mag: [Recruiter](./packs/recruiting/) | 2 | Candidate sourcing, resume screening, interview scheduling | [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/recruiting?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :chart_with_upwards_trend: [SEO Specialist](./packs/seo/) | 3 | Keyword research, content optimization, technical SEO audits, rank tracking | [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/seo?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :speech_balloon: [Social Media Manager](./packs/social-media/) | 3 | Content scheduling, engagement tracking, trend monitoring, community replies | [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/social-media?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :bulb: [Startup Advisor](./packs/startup-advisor/) | 2 | Market validation, pitch deck feedback, fundraising strategy, competitive analysis | [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/startup-advisor?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :microscope: [Researcher](./packs/research/) | 2 | Deep research, source verification, literature review, competitive intelligence | [openclaw-multi-agent-kit](https://github.com/raulvidis/openclaw-multi-agent-kit) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/research?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :seedling: [Growth Hacker](./packs/growth/) | 2 | Growth experiments, funnel optimization, A/B test analysis, viral loops | [openclaw-multi-agent-kit](https://github.com/raulvidis/openclaw-multi-agent-kit) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/growth?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :wave: [Community Manager](./packs/community/) | 2 | Discord/forum moderation, community engagement, user feedback synthesis | [openclaw-multi-agent-kit](https://github.com/raulvidis/openclaw-multi-agent-kit) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/community?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :movie_camera: [Content Creator](./packs/content-creation/) | 2 | Blog posts, newsletters, social threads, content repurposing | [openclaw-multi-agent-kit](https://github.com/raulvidis/openclaw-multi-agent-kit) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/content-creation?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :white_check_mark: [QA Engineer](./packs/qa/) | 2 | Test planning, bug triage, regression testing, quality gates | [openclaw-multi-agent-kit](https://github.com/raulvidis/openclaw-multi-agent-kit) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/qa?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :fountain_pen: [Writing Assistant](./packs/writing/) | 2 | Long-form writing, editing, style consistency, tone adaptation | [openclaw-agents](https://github.com/shenhao-stu/openclaw-agents) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/writing?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :mag_right: [Code Reviewer](./packs/code-review/) | 2 | PR reviews, code quality checks, security scanning, style enforcement | [openclaw-agents](https://github.com/shenhao-stu/openclaw-agents) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/code-review?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :zap: [Idea Generator](./packs/ideation/) | 2 | Brainstorming, concept validation, lateral thinking, innovation workshops | [openclaw-agents](https://github.com/shenhao-stu/openclaw-agents) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/ideation?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |
| :calendar: [Project Planner](./packs/project-planning/) | 2 | Project timelines, task breakdown, milestone tracking, dependency mapping | [openclaw-agents](https://github.com/shenhao-stu/openclaw-agents) | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/project-planning?utm_source=github&utm_medium=readme&utm_campaign=pack-deploy) |

Don't see your role? [Request a pack :arrow_right:](https://github.com/clawpod-app/awesome-openclaw-agent-packs/issues/new?labels=pack-request&title=Pack+request:+)

---

## Why OpenClaw?

| Feature | ChatGPT | Copilot | OpenClaw + ClawPod |
|---------|:-------:|:-------:|:------------------:|
| Self-hosted | :x: | :x: | :white_check_mark: |
| Custom skills | :x: | Limited | :white_check_mark: Unlimited |
| Messaging platforms | Web only | IDE | Telegram, Discord, WhatsApp, Slack |
| Monthly cost | $20/user | $10/user | $29.9 flat |
| Your data stays yours | :x: | :x: | :white_check_mark: |

OpenClaw is an open-source AI agent framework. [ClawPod](https://clawpod.app?utm_source=github&utm_medium=readme&utm_campaign=why-openclaw) handles hosting, so you get a production agent without managing infrastructure.

---

## Quick Start

### Option A: One-Click Deploy (recommended)

1. Pick a pack from the table above and click **Deploy**
2. Enter your bot token (Telegram, Discord, or other platform)
3. Your agent is live in 30 seconds at [clawpod.app](https://clawpod.app?utm_source=github&utm_medium=readme&utm_campaign=quickstart)

No Docker, no VPS, no configuration files.

### Option B: Self-Host with OpenClaw

```bash
git clone https://github.com/clawpod-app/awesome-openclaw-agent-packs.git
cp -r awesome-openclaw-agent-packs/packs/sales/* ~/.openclaw/workspace/
openclaw gateway restart
```

Your agent reads `SOUL.md` on startup, loads skills from `skills/`, and starts working.

### Option C: Manual Setup

1. Copy any pack to your OpenClaw workspace directory
2. Configure API keys and MCP tools per `TOOLS.md`
3. Restart your agent

---

## How Skills Work

Skills are text-based workflow guides, not executable scripts. When a user asks "research Acme Corp", the agent:

1. Reads `skills/account-research/SKILL.md`
2. Follows the step-by-step workflow defined inside
3. Uses available tools (web search, MCP connectors) to execute
4. Returns structured output

Skills work standalone with web search. They get better when you connect MCP tools (CRM, email, calendar), but they're fully functional without them.

```
packs/sales/
├── SOUL.md          # Who the agent is (personality, values, communication style)
├── AGENTS.md        # What it does on startup, available skills, workflows
├── HEARTBEAT.md     # Scheduled tasks (daily briefings, weekly pipeline reviews)
├── TOOLS.md         # Connected tools and MCP configuration
├── MEMORY.md        # How the agent remembers context across sessions
├── README.md        # Setup guide
└── skills/          # 9 skill workflows
    ├── account-research/    → Research any company or prospect
    ├── call-prep/           → Prepare for sales calls with context
    ├── draft-outreach/      → Personalized email & LinkedIn messages
    ├── pipeline-review/     → Analyze deal health and flag risks
    ├── forecast/            → Weighted revenue projections
    └── ...                  → + 4 more
```

---

## Tutorials & Guides

- [What is OpenClaw?](https://clawpod.app/blog/what-is-openclaw?utm_source=github&utm_medium=readme&utm_campaign=tutorial) — Overview of the OpenClaw framework and how it works
- [How to Install OpenClaw](https://clawpod.app/blog/how-to-install-openclaw?utm_source=github&utm_medium=readme&utm_campaign=tutorial) — Step-by-step installation guide
- [OpenClaw VPS Hosting Compared](https://clawpod.app/blog/openclaw-vps-hosting-compared?utm_source=github&utm_medium=readme&utm_campaign=tutorial) — Self-host vs managed hosting options
- [Cut OpenClaw Token Costs](https://clawpod.app/blog/cut-openclaw-token-costs?utm_source=github&utm_medium=readme&utm_campaign=tutorial) — Reduce LLM spend without sacrificing quality
- [OpenClaw Browser Automation Guide](https://clawpod.app/blog/openclaw-browser-automation-guide?utm_source=github&utm_medium=readme&utm_campaign=tutorial) — Automate web tasks with your agent
- [OpenClaw Security Guide](https://clawpod.app/blog/openclaw-security-guide-2026?utm_source=github&utm_medium=readme&utm_campaign=tutorial) — Hardening and best practices
- [Discord Bot Setup Guide](https://clawpod.app/blog/clawpod-discord-bot-setup-guide?utm_source=github&utm_medium=readme&utm_campaign=tutorial) — Deploy your agent to Discord
- [OpenClaw Multi-Agent Teams](https://clawpod.app/blog/openclaw-multi-agent-team-setup?utm_source=github&utm_medium=readme&utm_campaign=tutorial) — Coordinate multiple agents together
- [OpenClaw Real-World Use Cases](https://clawpod.app/blog/openclaw-real-world-use-cases?utm_source=github&utm_medium=readme&utm_campaign=tutorial) — How teams are using OpenClaw in production
- [OpenClaw vs n8n vs Make](https://clawpod.app/blog/openclaw-vs-n8n-vs-make-comparison?utm_source=github&utm_medium=readme&utm_campaign=tutorial) — Feature comparison with automation platforms

---

## Contributing

We welcome new packs and improvements to existing ones. See [CONTRIBUTING.md](./CONTRIBUTING.md) for the full guide.

**Quick version:**

1. All 6 core files required: `SOUL.md`, `AGENTS.md`, `HEARTBEAT.md`, `TOOLS.md`, `MEMORY.md`, `README.md`
2. At least one skill with a complete `SKILL.md` workflow
3. Tested on a real OpenClaw or ClawPod instance
4. README includes setup steps and example conversations

- [Submit a new pack](https://github.com/clawpod-app/awesome-openclaw-agent-packs/pulls) — Open a PR with your pack
- [Request a pack](https://github.com/clawpod-app/awesome-openclaw-agent-packs/issues/new?labels=pack-request&title=Pack+request:+) — Describe the role you need
- [Report an issue](https://github.com/clawpod-app/awesome-openclaw-agent-packs/issues/new) — Found a bug or have feedback

---

## Attribution

Core packs (11) adapted from [Anthropic's Knowledge Work Plugins](https://github.com/anthropics/knowledge-work-plugins) (Apache-2.0). See [NOTICE](./NOTICE) for details.

Community-sourced packs adapted from:
- [mergisi/awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) (MIT) — 10 packs
- [raulvidis/openclaw-multi-agent-kit](https://github.com/raulvidis/openclaw-multi-agent-kit) (MIT) — 5 packs
- [shenhao-stu/openclaw-agents](https://github.com/shenhao-stu/openclaw-agents) (MIT) — 4 packs

## License

MIT. Knowledge Work skills are derived from Anthropic's Apache-2.0 licensed work. See [LICENSE](./LICENSE).

---

Built by [ClawPod](https://clawpod.app?utm_source=github&utm_medium=readme&utm_campaign=footer) — Deploy your AI agent on Telegram or Discord in 30 seconds. $29.9/mo, everything included.
