# Operations

> Optimize business operations — vendor management, process documentation, change management, capacity planning, and compliance tracking.

## What It Does

- Evaluate vendors with structured cost analysis, risk assessment, and renewal recommendations
- Document business processes as complete SOPs with RACI matrices and flowcharts
- Create change management requests with impact analysis and rollback plans
- Plan resource capacity with utilization forecasting and headcount modeling
- Generate polished status reports with KPIs, risks, and action items
- Build operational runbooks with step-by-step procedures and troubleshooting guides
- Track compliance requirements and audit readiness

## Quick Start

### Deploy to ClawPod
[![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/deploy?template=operations)

### Self-host
```bash
cp -r ./* ~/.openclaw/workspace/
openclaw restart
```

## Skills Included

| Skill | Description |
|-------|-------------|
| `vendor-review` | Evaluate a vendor — cost analysis, risk assessment, and recommendation |
| `process-doc` | Document a business process — flowcharts, RACI matrices, SOPs |
| `change-request` | Create a change request — impact analysis, rollback plan, approval routing |
| `capacity-plan` | Plan resource capacity — workload analysis, utilization forecasting |
| `status-report` | Generate a status report — KPIs, risks, and action items |
| `runbook` | Create or update an operational runbook for recurring tasks |
| `process-optimization` | Analyze and improve business processes |
| `risk-assessment` | Identify, assess, and mitigate operational risks |
| `compliance-tracking` | Track compliance requirements and audit readiness |

## Example Conversation

```
User: /vendor-review Datadog

Agent: Starting vendor review for Datadog. I need a few details:
  1. Is this a new evaluation, renewal, or comparison?
  2. Current contract value and term?
  3. Any specific concerns (cost, features, support)?

User: Renewal. $120k/year, 2-year term expiring in Q3. Costs keep going up.

Agent: Vendor Review: Datadog
  Type: Renewal | Current: $120k/yr | Term: 2-year

  Cost Analysis:
  | Component        | Current  | Market Avg |
  |-----------------|----------|------------|
  | License          | $120k    | $95-140k   |
  | Support          | Included | Varies     |
  | Total 3-Year     | $360k    | $285-420k  |

  Risk Assessment: Medium
  - Vendor lock-in: High (proprietary query language)
  - Alternatives: Grafana Cloud, New Relic, Elastic

  Recommendation: Negotiate — you have leverage.
  Negotiation points: multi-year discount, usage-based pricing cap.
```

## Origin

Adapted from Anthropic's Knowledge Work Plugins (`knowledge-work-plugins/operations`).
