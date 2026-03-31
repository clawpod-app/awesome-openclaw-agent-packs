---
name: idea-evaluation
description: Evaluate and prioritize ideas using scoring frameworks with clear criteria. Trigger with "evaluate these ideas", "prioritize these options", "which idea is best", or "rank these ideas".
---

# Idea Evaluation

Score and prioritize ideas with structured criteria.

## When to Use
- After a brainstorming session to select top ideas
- Comparing multiple options for a decision
- Prioritizing a backlog of ideas

## Steps
1. Confirm the list of ideas to evaluate
2. Define evaluation criteria (or suggest appropriate ones)
3. Score each idea against criteria
4. Create a prioritization matrix (impact vs. effort or custom)
5. Recommend top ideas with reasoning

## Output Format
```markdown
## Idea Evaluation

### Criteria
| Criterion | Weight | Description |
|-----------|--------|-------------|
| Impact | [X%] | [What impact means here] |
| Effort | [X%] | [What effort means here] |
| Confidence | [X%] | [How sure we are it will work] |

### Scoring
| # | Idea | Impact | Effort | Confidence | Total |
|---|------|--------|--------|------------|-------|
| 1 | [idea] | [1-10] | [1-10] | [1-10] | [weighted] |

### Priority Matrix
**Quick Wins** (High Impact, Low Effort): [ideas]
**Big Bets** (High Impact, High Effort): [ideas]
**Fill-Ins** (Low Impact, Low Effort): [ideas]
**Skip** (Low Impact, High Effort): [ideas]

### Recommendation
Top 3 to pursue:
1. [Idea] -- [Why this is #1]
2. [Idea] -- [Why]
3. [Idea] -- [Why]
```
