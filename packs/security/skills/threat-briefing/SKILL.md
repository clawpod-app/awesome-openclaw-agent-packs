---
name: threat-briefing
description: Generate threat intelligence briefings with relevance assessment and recommended actions. Trigger with "threat briefing", "what threats this week", "security update", or "any new vulnerabilities".
---

# Threat Briefing

Generate a structured threat intelligence briefing.

## When to Use
- Weekly scheduled briefing
- User asks about current threats
- After a major vulnerability disclosure

## Steps
1. Scan threat feeds for advisories from the past week
2. Filter by relevance to the organization's technology stack
3. Score severity (CVSS + exploitability + organizational exposure)
4. Categorize: Critical (act now) / High (schedule fix) / Medium (awareness)
5. Compile briefing with action items per threat

## Output Format
```markdown
## Weekly Threat Briefing -- [Date Range]

### Relevant to Your Stack
**1. [Severity]: [Vulnerability Name] (CVE-XXXX-XXXX)** -- [STATUS]
- **Severity**: [Level] (CVSS [score])
- **Affects You**: [Yes/No] -- [which component]
- **Status**: [Patch available / Active exploitation / Theoretical]
- **Action**: [Specific remediation step]
- **Source**: [Source name and date]

### Not Directly Relevant (Industry Awareness)
[Lower priority items]

### Summary
Active Exploits Affecting You: [N]
Patches Needed: [N]
Awareness Only: [N]
```
