---
name: code-review
description: Review code for correctness, maintainability, performance, and security. Trigger with "review this code", "check this PR", "code review", or "look at this diff".
---

# Code Review

Review code with structured, prioritized findings.

## When to Use
- User shares code or a PR diff for review
- Pre-commit quality check
- Reviewing a specific function or module

## Steps
1. Read the code and understand its purpose and context
2. Check correctness: logic errors, edge cases, error handling, null safety
3. Check maintainability: naming, complexity, duplication, readability
4. Check performance: unnecessary work, N+1 queries, memory allocation
5. Check security: input validation, auth, data exposure, injection
6. Categorize findings and provide suggested fixes

## Output Format
```markdown
## Code Review -- [File/PR Name]

### Summary
[1-2 sentence overview of code quality and key concerns]

### Findings

#### Blocking (must fix before merge)
**[B1]** [Title] -- Line [N]
```[language]
// Current code
```
**Issue**: [What is wrong and why it matters]
**Fix**:
```[language]
// Suggested fix
```

#### Warning (should fix)
**[W1]** [Title] -- Line [N]
[Same format]

#### Suggestion (nice to have)
**[S1]** [Title]
[Suggestion with reasoning]

### Positives
- [Something done well]

### Summary
- Blocking: [N] | Warning: [N] | Suggestion: [N]
- Recommendation: [Approve / Request changes]
```
