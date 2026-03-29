# Human Resources

> Streamline people operations -- recruiting, onboarding, performance reviews, compensation analysis, and policy guidance.

## What It Does

- Draft offer letters with compensation details, equity breakdown, and benefits summary
- Generate onboarding checklists and first-week plans for new hires
- Structure performance reviews with self-assessment prompts, manager templates, and calibration prep
- Look up and explain company policies (PTO, benefits, expenses, remote work)
- Benchmark compensation against market data and analyze band placement
- Generate headcount, attrition, diversity, and org health reports
- Manage recruiting pipelines from sourcing through offer
- Create structured interview plans with competency-based questions and scorecards
- Plan headcount and optimize org structure

## Quick Start

### Deploy to ClawPod
[![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/deploy?template=human-resources)

### Self-host
```bash
cp -r ./* ~/.openclaw/workspace/
openclaw restart
```

## Skills Included

| Skill | Description |
|-------|-------------|
| `draft-offer` | Draft offer letters with comp details and terms |
| `onboarding` | Generate onboarding checklists and first-week plans |
| `performance-review` | Structure performance reviews and calibration |
| `policy-lookup` | Find and explain company policies |
| `comp-analysis` | Benchmark compensation and analyze band placement |
| `people-report` | Generate headcount, attrition, and diversity reports |
| `recruiting-pipeline` | Manage recruiting pipeline stages |
| `interview-prep` | Create structured interview plans and scorecards |
| `org-planning` | Headcount planning and org design |

## Example Conversation

```
User: /draft-offer
Agent: I'll help you draft an offer letter. What's the role and level?
User: Senior Software Engineer, L5, based in San Francisco.
Agent: Got it. What's the compensation package?
  - Base salary?
  - Equity (RSUs/options, shares, vesting)?
  - Signing bonus?
  - Start date?
User: $195K base, 5000 RSUs over 4 years with 1-year cliff, $20K signing bonus, start March 15.
Agent: [Generates complete offer letter with compensation breakdown, benefits summary, and standard terms]
```

## Origin

Adapted from Anthropic's Knowledge Work Plugins (`knowledge-work-plugins/human-resources`).
