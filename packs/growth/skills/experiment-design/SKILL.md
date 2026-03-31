---
name: experiment-design
description: Design structured growth experiments with hypotheses, ICE scoring, and success criteria. Trigger with "design an experiment", "growth experiment for [metric]", "how do we improve [metric]", or "test idea for [channel]".
---

# Experiment Design

Design a structured growth experiment.

## When to Use
- User wants to improve a specific metric
- Testing a new growth channel or tactic
- Optimizing an existing funnel step

## Steps
1. Define the growth lever (acquisition, activation, retention, revenue, referral)
2. Identify the current metric and target improvement
3. Generate 3-5 experiment ideas
4. Score each with ICE (Impact 1-10, Confidence 1-10, Ease 1-10)
5. Design the top experiment with full specification

## Output Format
```markdown
## Growth Experiment -- [Metric]

### Current State
- **Metric**: [current value]
- **Target**: [target value]
- **Lever**: [AARRR stage]

### Experiment Ideas (ICE Scored)
| # | Idea | Impact | Confidence | Ease | Score |
|---|------|--------|------------|------|-------|
| 1 | [idea] | [1-10] | [1-10] | [1-10] | [avg] |

### Top Experiment: [Name]
- **Hypothesis**: If we [change], then [metric] will [improve by X%] because [reasoning]
- **Control**: [Current state]
- **Variant**: [What changes]
- **Primary Metric**: [What to measure]
- **Sample Size**: [Minimum for significance]
- **Duration**: [Expected runtime]
- **Success Criteria**: [Threshold for declaring winner]
```
