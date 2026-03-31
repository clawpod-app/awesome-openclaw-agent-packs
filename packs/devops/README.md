# DevOps

> Monitor deployments, track pipeline health, and respond to infrastructure incidents with an AI-powered DevOps guardian.

## Skills Included
- **deploy-monitor**: Track CI/CD pipeline status, report build failures with context, monitor post-deploy health metrics
- **incident-response**: Assess production incidents, analyze rollback criteria, coordinate response with structured recommendations
- **infrastructure-audit**: Review DORA metrics, deployment frequency trends, and infrastructure health

## Quick Start
1. Deploy to [ClawPod](https://clawpod.app/templates/devops?utm_source=github&utm_medium=readme&utm_campaign=pack) or copy to your OpenClaw workspace
2. Connect your CI/CD platform (GitHub Actions, GitLab CI, etc.) via MCP
3. Start chatting -- ask "What's the status of today's deploys?"

## Example Conversations
```
User: What's the status of today's deploys?
Agent: Shows a table of all deployments with service, environment, status, time, author, and flags any failures with root cause analysis.
```

```
User: Should we roll back the latest deploy?
Agent: Checks post-deploy metrics (error rate, latency, CPU), compares against baseline, and gives a clear rollback recommendation with reasoning.
```

## Attribution
Adapted from [mergisi/awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) (MIT License) -- `agents/devops/deploy-guardian/SOUL.md`.
