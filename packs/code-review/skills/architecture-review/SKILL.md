---
name: architecture-review
description: Review architectural decisions and design patterns for scalability and maintainability. Trigger with "review the architecture", "is this design scalable", "architecture feedback", or "design review".
---

# Architecture Review

Review system design and architectural decisions.

## When to Use
- Evaluating a new feature's design before implementation
- Reviewing existing architecture for scaling concerns
- Assessing technical debt and refactoring priorities

## Steps
1. Understand the system context, constraints, and goals
2. Evaluate data flow and component interactions
3. Assess scalability: what happens at 10x, 100x current load
4. Review separation of concerns and coupling
5. Identify risks and suggest alternatives

## Output Format
```markdown
## Architecture Review -- [System/Feature]

### Context
[Understanding of the design being reviewed]

### Strengths
- [What is well-designed]

### Concerns

| Priority | Concern | Impact | Recommendation |
|----------|---------|--------|----------------|
| High | [concern] | [impact] | [recommendation] |
| Medium | [concern] | [impact] | [recommendation] |

### Scalability Assessment
- **Current load**: [Handles well / Struggling]
- **10x**: [What breaks first]
- **100x**: [What needs redesigning]

### Recommendations
1. [Highest priority architectural change]
2. [Second priority]
```
