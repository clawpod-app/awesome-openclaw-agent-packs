---
name: incident-response
description: Assess production incidents and recommend rollback decisions. Analyze error rates, latency, and resource metrics to determine severity and next steps. Trigger with "should we roll back", "production incident", "service is down", or "error rate spike".
---

# Incident Response

Assess production incidents and provide structured rollback recommendations.

## When to Use
- Production service shows elevated error rates or latency
- User reports a customer-facing issue after a deploy
- Monitoring alerts fire for a deployed service

## Steps
1. Identify the affected service and recent deployment history
2. Gather current metrics: error rate, latency (P50/P95/P99), CPU, memory
3. Compare against pre-deploy baseline metrics
4. Assess severity using threshold analysis
5. Recommend: no action / monitor / rollback with clear reasoning

## Output Format
```markdown
## Incident Assessment -- [Service]

**Trigger**: [What happened]
**Last Deploy**: [time] by [author] -- commit [sha]

### Current Metrics vs Baseline
| Metric | Current | Baseline | Delta | Status |
|--------|---------|----------|-------|--------|
| Error Rate | X% | Y% | +Z% | OK/WARN/CRITICAL |
| P99 Latency | Xms | Yms | +Zms | OK/WARN/CRITICAL |

### Recommendation
[Rollback / Monitor / No action needed] -- [reasoning]

### If Rollback Needed
1. [Step-by-step rollback procedure]
2. [Verification steps]
```
