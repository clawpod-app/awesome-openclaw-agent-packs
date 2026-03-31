---
name: risk-register
description: Identify project risks with likelihood, impact scoring, and mitigation strategies. Trigger with "what could go wrong with [project]", "risk assessment", "project risks", or "what are the risks".
---

# Risk Register

Identify and plan for project risks.

## When to Use
- Starting a new project -- proactive risk identification
- Mid-project review -- updating risk landscape
- After encountering an unexpected issue -- capturing lessons

## Steps
1. Review the project plan, scope, and dependencies
2. Identify risks across categories: technical, resource, scope, external, dependency
3. Score each risk: likelihood (1-5) and impact (1-5)
4. Calculate risk score (likelihood x impact)
5. Define mitigation and contingency for high-scoring risks

## Output Format
```markdown
## Risk Register -- [Project Name]

### Risks

| # | Risk | Category | Likelihood | Impact | Score | Mitigation |
|---|------|----------|------------|--------|-------|-----------|
| R1 | [risk] | Technical | [1-5] | [1-5] | [L*I] | [mitigation] |
| R2 | [risk] | Resource | [1-5] | [1-5] | [L*I] | [mitigation] |

### High-Priority Risks (Score >= 12)

**R[N]: [Risk Name]**
- **Scenario**: [What happens if this occurs]
- **Mitigation**: [How to reduce likelihood]
- **Contingency**: [What to do if it happens anyway]
- **Early Warning**: [How to detect this risk materializing]

### Risk Summary
- Total risks identified: [N]
- High (12+): [N] | Medium (6-11): [N] | Low (1-5): [N]
- Top risk to watch: [R#] -- [brief note]
```
