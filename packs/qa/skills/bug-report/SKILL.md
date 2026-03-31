---
name: bug-report
description: Write clear, actionable bug reports with reproduction steps and severity assessment. Trigger with "report a bug", "write a bug report", "found an issue with [feature]", or "something is broken in [area]".
---

# Bug Report

Write a clear, actionable bug report.

## When to Use
- A bug is found during testing
- User describes an issue that needs documentation
- Converting a vague "it's broken" into an actionable report

## Steps
1. Reproduce the issue and confirm it is consistent
2. Identify the minimum reproduction steps
3. Document expected vs. actual behavior
4. Assess severity based on business impact
5. Include environment details and evidence (screenshots, logs)

## Output Format
```markdown
## Bug Report

**Title**: [Clear, descriptive title]
**Severity**: Critical / High / Medium / Low
**Component**: [Feature or area affected]
**Environment**: [Browser, OS, version, etc.]

### Description
[One sentence summary of the issue]

### Steps to Reproduce
1. [Step 1]
2. [Step 2]
3. [Step 3]

### Expected Behavior
[What should happen]

### Actual Behavior
[What actually happens]

### Evidence
[Screenshot, error message, or log output]

### Notes
[Additional context, workarounds, or related issues]
```
