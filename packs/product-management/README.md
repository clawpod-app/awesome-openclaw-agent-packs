# Product Management

> Write feature specs, plan roadmaps, synthesize user research, and keep stakeholders aligned -- your AI product management partner.

## What It Does

- Generate structured PRDs and feature specs from problem statements
- Create and reprioritize product roadmaps (Now/Next/Later, quarterly, OKR-aligned)
- Draft stakeholder updates tailored to execs, engineering, or customers
- Synthesize interview notes, surveys, and support tickets into actionable insights
- Research competitors and generate comparison briefs
- Analyze product metrics and surface trends
- Brainstorm product ideas with a sharp thinking partner (JTBD, First Principles, How Might We)
- Plan sprints with capacity and dependency awareness

## Quick Start

### Deploy to ClawPod
[![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/deploy?template=product-management)

### Self-host
```bash
cp -r ./* ~/.openclaw/workspace/
openclaw restart
```

## Skills Included

| Skill | Description |
|-------|-------------|
| `write-spec` | Write a feature spec or PRD from a problem statement |
| `roadmap-update` | Create, update, or reprioritize a product roadmap |
| `stakeholder-update` | Generate status updates for any audience |
| `synthesize-research` | Synthesize user research into structured insights |
| `competitive-brief` | Create competitive analysis briefs |
| `metrics-review` | Analyze product metrics and identify trends |
| `product-brainstorming` | Explore problem spaces and stress-test ideas |
| `sprint-planning` | Plan sprint scope with priorities and dependencies |

## Example Conversation

```
User: /write-spec
Agent: What feature or problem are you speccing out?
User: We need to add SSO support for enterprise customers.
Agent: Before I draft the spec, a few questions:
  1. Who's the primary user -- IT admins or end users?
  2. Which identity providers do you need to support?
  3. What's the success metric -- enterprise conversion rate?
User: IT admins set it up, end users just log in. SAML and OIDC. Success = 30% increase in enterprise trial-to-paid.
Agent: [Generates full PRD with problem statement, user stories, requirements, success metrics, and open questions]
```

## Origin

Adapted from Anthropic's Knowledge Work Plugins (`knowledge-work-plugins/product-management`).
