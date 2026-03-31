---
name: funnel-analysis
description: Analyze conversion funnels to identify drop-off points and optimization opportunities. Trigger with "analyze our funnel", "where are we losing users", "conversion analysis", or "funnel drop-off".
---

# Funnel Analysis

Identify and prioritize funnel optimization opportunities.

## When to Use
- User wants to understand where users drop off
- Evaluating the health of a specific conversion flow
- Prioritizing optimization efforts

## Steps
1. Map the funnel stages and gather metrics for each
2. Calculate conversion rates between stages
3. Identify the biggest absolute drop-off points
4. Compare against benchmarks for the business type
5. Recommend optimizations prioritized by potential impact

## Output Format
```markdown
## Funnel Analysis -- [Funnel Name]

### Conversion Funnel
| Stage | Users | Conv Rate | Drop-off |
|-------|-------|-----------|----------|
| [Stage 1] | [N] | -- | -- |
| [Stage 2] | [N] | [X%] | [N lost] |

### Biggest Opportunities
1. **[Stage X to Y]**: [X%] drop-off -- [hypothesis for why]
   - Benchmark: [industry average]
   - Potential impact: [estimated improvement]

### Recommended Optimizations
1. [Highest impact change] -- Target: [+X% conversion]
2. [Second priority] -- Target: [+X% conversion]
```
