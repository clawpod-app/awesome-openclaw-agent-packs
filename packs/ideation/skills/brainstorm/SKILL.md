---
name: brainstorm
description: Generate ideas using structured brainstorming frameworks. Trigger with "brainstorm ideas for [challenge]", "help me think of [topic]", "10 ideas for [problem]", or "creative solutions for [situation]".
---

# Brainstorm

Generate ideas using structured ideation frameworks.

## When to Use
- User needs ideas for a challenge or opportunity
- Exploring a new project or feature direction
- Getting unstuck on a creative problem

## Steps
1. Clarify the challenge and any constraints
2. Choose the appropriate framework:
   - **SCAMPER**: Substitute, Combine, Adapt, Modify, Put to use, Eliminate, Reverse
   - **How Might We**: Reframe the challenge as opportunity questions
   - **Reverse Brainstorming**: How could we make this worse? Then flip it
   - **Random Association**: Connect unrelated concepts for novel ideas
3. Generate 10+ ideas without judgment (divergent phase)
4. Offer to evaluate and prioritize (convergent phase)
5. Develop top ideas into actionable concepts

## Output Format
```markdown
## Brainstorm: [Challenge]

**Framework**: [SCAMPER / How Might We / etc.]
**Constraint**: [Any constraints noted]

### Ideas (Divergent Phase -- no judgment)
1. [Idea] -- [Brief explanation]
2. [Idea] -- [Brief explanation]
...
10. [Idea]

### Wild Cards (intentionally ambitious)
11. [Bold idea]
12. [Bold idea]

---
Want me to evaluate these with an impact/effort matrix and develop the top 3?
```
