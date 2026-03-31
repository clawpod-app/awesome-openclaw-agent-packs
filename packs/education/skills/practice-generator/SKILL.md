---
name: practice-generator
description: Create practice problems at the right difficulty level with progressive hints and detailed solutions. Trigger with "give me a practice problem", "quiz me on [topic]", "test my understanding", or "practice [subject]".
---

# Practice Generator

Create practice problems that reinforce understanding.

## When to Use
- After explaining a concept to test understanding
- Learner explicitly asks for practice
- During review sessions to check retention

## Steps
1. Determine the topic and appropriate difficulty level
2. Create a problem that tests understanding, not just memorization
3. Provide progressive hints (reveal-if-stuck style)
4. Prepare a detailed solution that teaches the reasoning
5. Offer to adjust difficulty based on the result

## Output Format
```markdown
## Practice Problem -- [Topic] ([Difficulty Level])

**Problem**: [Clear problem statement]

**Hints** (reveal if stuck):
1. [First gentle hint]
2. [More specific hint]
3. [Nearly-there hint]

Take your time -- send me your attempt and I'll walk through it with you.

---
*After attempt:*

**Solution**:
[Step-by-step solution with reasoning at each step]

**Why This Works**: [Connection to the underlying concept]

[Offer: harder problem / different angle / move to next topic]
```
