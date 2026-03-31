---
name: ad-copy
description: Create platform-specific ad copy within character limits with A/B test variants. Supports Google Ads, Facebook, and LinkedIn. Trigger with "ad copy", "Google Ads copy", "Facebook ad", or "LinkedIn ad".
---

# Ad Copy

Create platform-aware ad copy with variants for testing.

## When to Use
- User needs ad copy for paid campaigns
- User wants to test different messaging angles
- User needs copy adapted to specific platform constraints

## Steps
1. Confirm platform, product, audience, and campaign goal
2. Check platform-specific constraints (Google Ads: 30-char headlines, 90-char descriptions; Facebook: 125-char primary text; LinkedIn: 150-char intro)
3. Write 3 variants with different angles (benefit, pain, urgency)
4. Include character counts for each element
5. Provide A/B test hypothesis for each variant

## Output Format
```markdown
## Ad Copy -- [Platform] -- [Product]

### Variant A: [Angle]
- **Headline**: [copy] ([X] chars)
- **Description**: [copy] ([X] chars)
- **Hypothesis**: [Expected performance and why]

### Variant B: [Angle]
- **Headline**: [copy] ([X] chars)
- **Description**: [copy] ([X] chars)
- **Hypothesis**: [Expected performance and why]

### Variant C: [Angle]
- **Headline**: [copy] ([X] chars)
- **Description**: [copy] ([X] chars)
- **Hypothesis**: [Expected performance and why]

**Test Plan**: Run A vs B first ([reasoning]), then test winner vs C.
```
