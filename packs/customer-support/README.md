# Customer Support

> Triage tickets, draft responses, escalate issues, and build your knowledge base. Research customer context and turn resolved issues into self-service content.

## What It Does

- Triage incoming tickets with structured categorization, priority assessment (P1-P4), and routing recommendations
- Research customer questions by synthesizing information from multiple sources with confidence scoring
- Draft professional, empathetic responses tailored to the situation, urgency, and communication channel
- Package escalations with full context, reproduction steps, and business impact for engineering or product
- Write knowledge base articles from resolved issues to reduce future ticket volume
- Track recurring issues and identify KB gaps

## Quick Start

### Deploy to ClawPod
[![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/deploy?template=customer-support)

### Self-host
```bash
cp -r ./* ~/.openclaw/workspace/
openclaw restart
```

## Skills Included

| Skill | Type | Description |
|-------|------|-------------|
| `ticket-triage` | Auto | Category taxonomy, priority framework (P1-P4), routing rules, duplicate detection |
| `customer-research` | Auto | Multi-source research, source prioritization, answer synthesis with confidence scoring |
| `response-drafting` | Auto | Communication best practices, tone guidelines, templates for common scenarios |
| `escalation` | Auto | Escalation tiers, structured format, impact assessment, follow-up cadence |
| `knowledge-management` | Auto | Article structure standards, writing for searchability, review cadence |
| `triage` | Command | Categorize, prioritize, and route a support ticket |
| `research` | Command | Multi-source research on a customer question |
| `draft-response` | Command | Draft a customer-facing response |
| `escalate` | Command | Package an escalation for engineering, product, or leadership |
| `kb-article` | Command | Draft a KB article from a resolved issue |

## Example Conversation

```
User: /triage Customer says their dashboard has been showing a blank
      page since this morning -- they're on the Enterprise plan

Agent: Analyzing the issue...

## Triage: Dashboard blank page -- Enterprise customer

**Category:** Bug
**Priority:** P2 -- High (core feature broken, enterprise customer)
**Product area:** Dashboard / Frontend

### Routing Recommendation
Route to: Tier 2 Support (investigate browser/account specifics,
then escalate to Engineering if reproducible)

### Suggested Initial Response
"Hi [Customer], thank you for reporting this. I understand how
frustrating it must be to not have access to your dashboard --
I'm making this a priority.

Could you let me know:
1. Which browser and version you're using?
2. Have you tried clearing your cache or using incognito mode?
3. Are any other team members experiencing the same issue?

I'm investigating this now and will update you within the hour."
```

## Origin

Adapted from Anthropic's Knowledge Work Plugins (`knowledge-work-plugins/customer-support`).
