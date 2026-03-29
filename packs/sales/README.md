# Sales

> Prospect, craft outreach, and build deal strategy faster. Prep for calls, manage your pipeline, and write personalized messaging that moves deals forward.

## What It Does

- Research prospects and accounts with web search and data enrichment
- Draft personalized outreach (email + LinkedIn) backed by prospect research
- Process call notes/transcripts into structured summaries with action items and follow-up drafts
- Generate weighted sales forecasts with best/likely/worst scenarios
- Analyze pipeline health, flag risks, and build weekly action plans
- Prepare for calls with account context, attendee research, and discovery questions
- Research competitors with differentiation matrices and talk tracks
- Create custom sales assets (decks, one-pagers, landing pages) tailored to prospects

## Quick Start

### Deploy to ClawPod
[![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/deploy?template=sales)

### Self-host
```bash
cp -r ./* ~/.openclaw/workspace/
openclaw restart
```

## Skills Included

| Skill | Type | Description |
|-------|------|-------------|
| `account-research` | Auto | Research a company or person -- company intel, key contacts, recent news, hiring signals |
| `call-prep` | Auto | Prepare for sales calls -- account context, attendee research, agenda, discovery questions |
| `daily-briefing` | Auto | Prioritized daily briefing -- meetings, pipeline alerts, email priorities, actions |
| `draft-outreach` | Auto | Research-first outreach -- personalized email and LinkedIn messages |
| `competitive-intelligence` | Auto | Competitor research -- product comparison, pricing intel, differentiation matrix |
| `create-an-asset` | Auto | Custom sales assets -- landing pages, decks, one-pagers for prospects |
| `call-summary` | Command | Process call notes/transcript -- action items, follow-up draft, internal summary |
| `forecast` | Command | Weighted sales forecast -- CSV or manual input, quota projections, gap analysis |
| `pipeline-review` | Command | Pipeline health analysis -- deal prioritization, risk flags, action plan |

## Example Conversation

```
User: Research Acme Corp before my call tomorrow

Agent: Researching Acme Corp...

## Acme Corp -- Pre-Call Brief

**Company**: Acme Corp | Series C | $45M ARR | 320 employees
**Industry**: Supply chain SaaS
**Recent News**: Raised $60M Series C (Jan 2026), expanding into EU market
**Key Contacts**:
  - Jane Smith, VP Engineering (your meeting) -- 3 years at Acme, prev. at Stripe
  - Tom Chen, CTO -- co-founder, active on LinkedIn about AI/ML

**Recommended Approach**: Lead with supply chain automation angle.
Their engineering team is growing 40% YoY -- likely feeling infrastructure pain.

**Discovery Questions**:
1. How are you handling the scaling challenges with the EU expansion?
2. What does your current vendor evaluation process look like?
3. Who else is involved in tooling decisions for the engineering team?
```

## Origin

Adapted from Anthropic's Knowledge Work Plugins (`knowledge-work-plugins/sales`).
