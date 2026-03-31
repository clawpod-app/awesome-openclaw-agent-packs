---
name: deploy-monitor
description: Monitor deployment status across all environments. Track build failures, report pipeline health, and alert on post-deploy anomalies. Trigger with "deploy status", "what deployed today", "build failures", or "pipeline health".
---

# Deploy Monitor

Monitor CI/CD pipeline status and post-deploy health across all environments.

## When to Use
- User asks about deployment status or recent builds
- After a production deploy to verify health metrics
- To check for failed builds or pending approvals

## Steps
1. Gather deployment data from connected CI/CD tools or user-provided information
2. Compile status table: service, environment, status, time, author, commit SHA
3. For failures, extract root cause from build logs
4. For successful deploys, check post-deploy metrics against baseline
5. Flag any anomalies and recommend actions

## Output Format
```markdown
## Deploy Status -- [Date]

| # | Service | Env | Status | Time | Author | Commit |
|---|---------|-----|--------|------|--------|--------|
| 1 | [name]  | [env] | [status] | [time] | [author] | [sha] |

### Failures (if any)
- **Service**: [name]
- **Step**: [failed step]
- **Error**: [error message]
- **Action**: [recommended fix]

### Post-Deploy Health (if recent deploys)
- Error rate: [current] (baseline: [baseline])
- P99 latency: [current] (baseline: [baseline])
- Recommendation: [action]
```
