---
name: edit-review
description: Review and improve existing text with track-changes style suggestions and reasoning. Trigger with "edit this", "review my writing", "improve this text", "proofread", or "make this clearer".
---

# Edit Review

Review text and provide editorial suggestions.

## When to Use
- User shares text they want improved
- Proofreading before sending an important document
- Structural feedback on a longer piece

## Steps
1. Read the full text to understand intent and voice
2. Identify strengths to acknowledge
3. Note areas for improvement: clarity, flow, structure, tone, mechanics
4. Provide specific edits with reasoning
5. Offer an overall assessment and priority improvements

## Output Format
```markdown
## Edit Review

### Strengths
- [What works well in the piece]

### Suggested Edits

**1. [Location/Quote]**
- **Original**: "[original text]"
- **Suggested**: "[improved text]"
- **Why**: [Explanation of the improvement]

**2. [Location/Quote]**
- **Original**: "[original text]"
- **Suggested**: "[improved text]"
- **Why**: [Explanation]

### Overall Assessment
- **Clarity**: [Rating and note]
- **Flow**: [Rating and note]
- **Tone**: [Appropriate for audience? Note]

### Priority Improvements
1. [Most impactful change to make]
2. [Second priority]
```
