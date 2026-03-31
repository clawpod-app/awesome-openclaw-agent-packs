---
name: test-plan
description: Create comprehensive test plans with test cases, edge cases, and acceptance criteria. Trigger with "test plan for [feature]", "how should I test [feature]", "test cases for [flow]", or "QA checklist".
---

# Test Plan

Create a structured test plan for a feature or flow.

## When to Use
- New feature ready for QA
- Preparing for a release
- User wants systematic test coverage for an area

## Steps
1. Understand the feature requirements and user flows
2. Identify test scenarios: happy path, edge cases, error states, boundary conditions
3. Write test cases with clear steps and expected results
4. Prioritize by risk and business impact
5. Note any test environment requirements or prerequisites

## Output Format
```markdown
## Test Plan -- [Feature Name]

### Scope
- **Feature**: [What is being tested]
- **Prerequisites**: [Setup needed]
- **Environments**: [Where to test]

### Test Cases

#### Happy Path
| # | Test Case | Steps | Expected Result | Priority |
|---|-----------|-------|-----------------|----------|
| 1 | [name] | [steps] | [result] | High |

#### Edge Cases
| # | Test Case | Steps | Expected Result | Priority |
|---|-----------|-------|-----------------|----------|
| 1 | [name] | [steps] | [result] | Medium |

#### Error States
| # | Test Case | Steps | Expected Result | Priority |
|---|-----------|-------|-----------------|----------|
| 1 | [name] | [steps] | [result] | High |

### Coverage Notes
- [What is covered]
- [What is NOT covered and why]
```
