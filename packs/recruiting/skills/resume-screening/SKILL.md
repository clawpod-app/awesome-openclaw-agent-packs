---
name: resume-screening
description: Screen resumes against job requirements and rank candidates with weighted scoring. Trigger with "screen resumes", "rank candidates", "review applications", or "who should we interview".
---

# Resume Screening

Screen and rank candidates against job requirements.

## When to Use
- New batch of applications received
- User wants to prioritize candidates for interviews
- Re-screening after role requirements change

## Steps
1. Parse job requirements into must-have and nice-to-have criteria
2. Review each resume against criteria with weighted scoring
3. Tier candidates: Strong Match, Good Match, Partial Match, No Match
4. Rank within tiers by total score
5. Present top candidates with scoring breakdown and rationale

## Output Format
```markdown
## Resume Screening -- [Role Name]

**Applications**: [N]
**Requirements**: [Summary of must-haves]

### Screening Results
| Tier | Count | Criteria |
|------|-------|----------|
| Strong Match | [N] | Meets all must-haves + 2+ nice-to-haves |
| Good Match | [N] | Meets all must-haves |
| Partial Match | [N] | Missing 1 must-have, strong in others |
| No Match | [N] | Missing 2+ must-haves |

### Top 5 Candidates
| Rank | Name | Experience | Key Skills | Score |
|------|------|------------|------------|-------|
| 1 | [Name] | [Summary] | [Skills] | [Score] |

**Notes**: [Key observations about top candidates]
**Recommendation**: [Next step -- interview top N candidates]
```
