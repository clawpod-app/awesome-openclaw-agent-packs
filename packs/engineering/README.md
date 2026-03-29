# Engineering

> Streamline engineering workflows -- standups, code review, architecture decisions, incident response, and technical documentation. Works with your existing tools or standalone.

## What It Does

- Generate standup updates from recent commits, PRs, and tickets
- Review code changes for security, performance, correctness, and style
- Run structured debugging sessions: reproduce, isolate, diagnose, fix
- Create architecture decision records (ADRs) with trade-off analysis
- Manage incident response: triage, communicate, mitigate, write postmortems
- Generate pre-deployment checklists with rollback plans
- Identify, categorize, and prioritize technical debt
- Design test strategies across unit, integration, and e2e layers
- Write and maintain technical documentation

## Quick Start

### Deploy to ClawPod
[![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/deploy?template=engineering)

### Self-host
```bash
cp -r ./* ~/.openclaw/workspace/
openclaw restart
```

## Skills Included

| Skill | Type | Description |
|-------|------|-------------|
| `code-review` | Auto | Review code for bugs, security, performance, and maintainability |
| `incident-response` | Auto | Triage and manage production incidents -- status updates, runbooks, postmortems |
| `system-design` | Auto | Design systems and services -- architecture, API design, data modeling |
| `tech-debt` | Auto | Identify, categorize, and prioritize technical debt with remediation plans |
| `testing-strategy` | Auto | Design test strategies -- unit, integration, e2e coverage and test plans |
| `documentation` | Auto | Write and maintain technical docs -- READMEs, API docs, runbooks |
| `standup` | Command | Generate standup update from recent activity |
| `review` | Command | Structured code review covering security, perf, correctness, style |
| `debug` | Command | Structured debugging: reproduce, isolate, diagnose, fix |
| `architecture` | Command | ADR creation with options analysis and trade-offs |
| `incident` | Command | Incident response workflow: triage, communicate, mitigate, postmortem |
| `deploy-checklist` | Command | Pre-deployment verification checklist |

## Example Conversation

```
User: /debug Users are getting 500 errors on the checkout page

Agent: Starting structured debugging session.

## Debug: 500 errors on checkout page

### Step 1 -- Reproduce
- What URL/endpoint is failing? /api/checkout/submit
- Is it every request or intermittent?
- When did it start? Any recent deploys?

### Step 2 -- Isolate
Let me check what we know:
- Is the error in the application logs or the load balancer?
- Are other endpoints on the same service healthy?
- Any database or downstream service issues?

Share your logs or monitoring data and I'll help narrow down the root cause.

### Step 3 -- Diagnose
[Awaiting data to form hypotheses...]

### Step 4 -- Fix
[Will recommend minimal fix once root cause is confirmed]
```

## Origin

Adapted from Anthropic's Knowledge Work Plugins (`knowledge-work-plugins/engineering`).
