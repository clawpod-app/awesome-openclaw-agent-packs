---
name: infrastructure-audit
description: Audit infrastructure health and deployment practices using DORA metrics. Review deployment frequency, lead time, MTTR, and change failure rate. Trigger with "DORA metrics", "infrastructure audit", "deployment frequency", or "how healthy is our pipeline".
---

# Infrastructure Audit

Review deployment practices and infrastructure health using DORA metrics.

## When to Use
- Weekly or monthly infrastructure health review
- After a series of incidents to identify systemic issues
- When evaluating CI/CD pipeline improvements

## Steps
1. Collect deployment data for the review period
2. Calculate DORA metrics: frequency, lead time, MTTR, change failure rate
3. Compare against industry benchmarks (Elite/High/Medium/Low)
4. Identify trends and patterns in failures
5. Recommend improvements with prioritized action items

## Output Format
```markdown
## Infrastructure Audit -- [Period]

### DORA Metrics
| Metric | Value | Benchmark | Rating |
|--------|-------|-----------|--------|
| Deploy Frequency | X/week | On-demand | Elite/High/Med/Low |
| Lead Time | X hours | <1 hour | Elite/High/Med/Low |
| MTTR | X minutes | <1 hour | Elite/High/Med/Low |
| Change Failure Rate | X% | 0-15% | Elite/High/Med/Low |

### Trends
- [Trend observation with data]

### Recommendations
1. [Highest priority improvement]
2. [Second priority]
3. [Third priority]
```
