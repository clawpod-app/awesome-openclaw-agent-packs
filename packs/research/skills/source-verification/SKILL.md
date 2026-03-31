---
name: source-verification
description: Verify claims by tracing to primary sources, checking recency, and assessing credibility. Trigger with "verify this claim", "fact check", "is this true", or "check the source on [claim]".
---

# Source Verification

Verify claims and assess source credibility.

## When to Use
- User encounters a claim that needs verification
- Fact-checking information before using it in decisions
- Evaluating the reliability of a specific source

## Steps
1. Identify the specific claim to verify
2. Trace to the original/primary source
3. Check source credibility (publication, author, methodology)
4. Look for corroboration from independent sources
5. Assess recency and whether the information is still current

## Output Format
```markdown
## Fact Check: [Claim]

**Verdict**: Confirmed / Partially True / Unverified / False
**Confidence**: High / Medium / Low

### Original Source
- **Source**: [Where the claim originates]
- **Credibility**: [Assessment]
- **Date**: [When published]

### Corroboration
- [Supporting or contradicting source 1]
- [Supporting or contradicting source 2]

### Context
[Important nuance or context that affects interpretation]

### Conclusion
[Summary of findings with caveats]
```
