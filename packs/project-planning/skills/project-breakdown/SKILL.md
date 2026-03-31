---
name: project-breakdown
description: Break down a project into milestones, tasks, estimates, and dependencies. Trigger with "plan this project", "break down [project]", "create a project plan for [goal]", or "how long will [project] take".
---

# Project Breakdown

Decompose a project into an actionable plan.

## When to Use
- Starting a new project and need structure
- User has a goal but no clear execution path
- Estimating timeline and effort for a project

## Steps
1. Clarify project goal, success criteria, and constraints
2. Define scope: explicitly state what's included and what's not
3. Identify major milestones (3-6) with clear deliverables
4. Break each milestone into tasks (3-8 per milestone)
5. Estimate each task, add dependencies, and identify the critical path
6. Add buffer time (20-30% for unknowns)

## Output Format
```markdown
## Project Plan: [Project Name]

### Goal
[What success looks like]

### Scope
**In Scope**: [What's included]
**Out of Scope**: [What's explicitly excluded]
**Deferred**: [What might come later]

### Milestones

#### M1: [Milestone Name] -- [Target Date]
| # | Task | Estimate | Depends On | Owner |
|---|------|----------|------------|-------|
| 1.1 | [task] | [Xd] | -- | [TBD] |
| 1.2 | [task] | [Xd] | 1.1 | [TBD] |

#### M2: [Milestone Name] -- [Target Date]
[Same format]

### Timeline
```
Week 1-2: M1 [████████░░░░░░░░]
Week 3-4: M2 [░░░░░░██████████]
Week 5:   M3 [░░░░░░░░░░░░████]
```

### Critical Path
[Tasks that directly determine the project end date]

### Total Estimate
- **Optimistic**: [X weeks]
- **Likely**: [X weeks] (includes 20% buffer)
- **Pessimistic**: [X weeks]
```
