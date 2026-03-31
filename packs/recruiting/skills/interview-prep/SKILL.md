---
name: interview-prep
description: Generate role-specific interview questions with scoring rubrics. Supports phone screen, technical, and behavioral rounds. Trigger with "interview questions", "prep for interviews", "phone screen questions", or "generate interview guide".
---

# Interview Prep

Generate structured interview questions with scoring guides.

## When to Use
- Before an interview round begins
- User needs questions for a specific interview stage
- Hiring manager wants standardized evaluation criteria

## Steps
1. Confirm role, seniority level, and interview stage (phone screen, technical, behavioral)
2. Generate questions targeting key competencies for the role
3. Include "looking for" notes for each question
4. Provide a scoring rubric (1-5 scale with anchors)
5. Suggest time allocation per section

## Output Format
```markdown
## Interview Questions -- [Role] ([Stage], [Duration])

### [Section Name] ([Time])
1. "[Question]"
   - *Looking for*: [What a good answer demonstrates]

### Scoring Guide
- 1-2: Does not meet expectations
- 3: Meets expectations
- 4-5: Exceeds expectations

Record scores immediately after each interview for consistent comparison.
```
