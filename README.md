[English](./README.md) | [中文](./README.zh-CN.md) | [日本語](./README.ja.md) | [Español](./README.es.md) | [Deutsch](./README.de.md)

# Awesome OpenClaw Agent Packs

**Pre-configured AI agent packs for OpenClaw. Pick a role, deploy to Telegram, start working.**

[![Deploy to ClawPod](https://img.shields.io/badge/Deploy%20to-ClawPod-FF6B35?style=for-the-badge)](https://clawpod.app/templates)
![Packs](https://img.shields.io/badge/Packs-11-blue?style=for-the-badge)
![Skills](https://img.shields.io/badge/Skills-92-purple?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

---

## What Is This?

Each pack turns a generic OpenClaw agent into a specialized team member. A **Sales Co-Pilot** that preps for calls, researches prospects, and drafts outreach. An **Engineering Co-Pilot** that does standups, code reviews, and incident response. A **Legal Analyst** that reviews contracts and checks compliance.

Every pack includes 6 definition files + a full `skills/` directory:

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

## Available Packs

| Pack | Skills | Domain | Deploy |
|------|--------|--------|--------|
| [Sales Co-Pilot](./packs/sales/) | 9 | Sales & Revenue | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/sales) |
| [Engineering Co-Pilot](./packs/engineering/) | 10 | Software Engineering | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/engineering) |
| [Data Analyst](./packs/data/) | 10 | Data & Analytics | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/data) |
| [Marketing Strategist](./packs/marketing/) | 8 | Marketing & Content | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/marketing) |
| [Legal Analyst](./packs/legal/) | 9 | Legal & Compliance | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/legal) |
| [Finance Analyst](./packs/finance/) | 8 | Finance & Accounting | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/finance) |
| [Product Manager](./packs/product-management/) | 8 | Product Management | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/product-management) |
| [HR Partner](./packs/human-resources/) | 9 | HR & People Ops | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/human-resources) |
| [Customer Support](./packs/customer-support/) | 5 | Customer Support | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/customer-support) |
| [Design Partner](./packs/design/) | 7 | UX & Design | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/design) |
| [Operations Manager](./packs/operations/) | 9 | Business Operations | [![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/templates/operations) |

---

## Quick Start

### Option A: One-Click Deploy (recommended)

1. Pick a pack above and click **Deploy to ClawPod**
2. Enter your Telegram bot token
3. Your agent is live in 30 seconds at [clawpod.app](https://clawpod.app)

No Docker, no VPS, no configuration files.

### Option B: Self-Host with OpenClaw

```bash
git clone https://github.com/clawpod-app/awesome-openclaw-agent-packs.git
cp -r awesome-openclaw-agent-packs/packs/sales/* ~/.openclaw/workspace/
openclaw gateway restart
```

Your agent reads `SOUL.md` on startup, loads the skills from `skills/`, and starts working.

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

---

## Contributing

We welcome new packs! Requirements:

1. All 6 core files: `SOUL.md`, `AGENTS.md`, `HEARTBEAT.md`, `TOOLS.md`, `MEMORY.md`, `README.md`
2. At least one skill with a complete `SKILL.md` workflow
3. Tested on a real OpenClaw or ClawPod instance
4. README includes setup steps and example conversations

See any existing pack for the expected format.

---

## Attribution

Adapted from [Anthropic's Knowledge Work Plugins](https://github.com/anthropics/knowledge-work-plugins) (Apache-2.0). See [NOTICE](./NOTICE) for details.

## License

MIT. Knowledge Work skills are derived from Anthropic's Apache-2.0 licensed work. See [LICENSE](./LICENSE).

---

*Maintained by [ClawPod](https://clawpod.app) — Deploy your AI Telegram bot in 30 seconds.*
