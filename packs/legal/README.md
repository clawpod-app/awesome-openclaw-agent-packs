# Legal Soul Pack

> Speed up contract review, NDA triage, and compliance workflows for in-house legal teams. Draft legal briefs, organize precedent research, and manage institutional knowledge.

## What It Does

- Review contracts against your organization's negotiation playbook with GREEN/YELLOW/RED flags
- Triage incoming NDAs for rapid routing (standard approval vs. counsel review)
- Check vendor agreement status across connected systems
- Generate daily, topic, and incident legal briefings
- Produce templated responses for common inquiry types (DSRs, discovery holds, vendor questions)
- Assess legal risk with structured severity frameworks
- Prepare meeting briefs with context and action items

## Quick Start

### Deploy to ClawPod
[![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/deploy?template=legal)

### Self-host
```bash
cp -r ./* ~/.openclaw/workspace/
openclaw restart
```

Configure your playbook in `memory/playbook/legal.local.md` to define standard positions, acceptable ranges, and escalation triggers.

## Skills Included

| Skill | Description |
|-------|-------------|
| `review-contract` | Playbook-based contract analysis, deviation classification, redline generation |
| `triage-nda` | NDA screening with GREEN/YELLOW/RED classification and routing |
| `vendor-check` | Vendor agreement status lookup across connected systems |
| `brief` | Legal team briefings -- daily, topic-specific, or incident-based |
| `legal-response` | Templated responses for common inquiry types |
| `compliance-check` | Privacy regulation review (GDPR, CCPA), DPA analysis, data subject requests |
| `legal-risk-assessment` | Risk severity framework with classification levels and escalation criteria |
| `meeting-briefing` | Meeting prep with context gathering and action item tracking |
| `signature-request` | Route documents for e-signature via connected tools |

## Example Conversation

```
User: /review-contract
      [uploads vendor SaaS agreement]
      We're the customer. Need to close by end of quarter.
      Focus on data protection and liability.

Agent: Reviewing against your playbook. Here's the clause-by-clause analysis:

  GREEN: Term and termination -- annual with 30-day convenience clause (matches standard)
  YELLOW: Limitation of liability -- cap at 6 months (your standard is 12 months)
    Suggested redline: "...not to exceed twelve (12) months of fees paid or payable..."
  RED: Data protection -- no DPA offered, cross-border transfer without safeguards
    Escalation: Request DPA with sub-processor notification and 72-hour breach notice

  3 GREEN | 2 YELLOW | 1 RED -- recommend addressing RED before signing.
```

## Origin

Adapted from Anthropic's Knowledge Work Plugins (`legal` plugin v1.2.0).
