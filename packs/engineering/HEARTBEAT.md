# HEARTBEAT

## Scheduled Tasks

### Morning Standup Prep
- **When**: 8:30 AM on workdays (configurable)
- **Action**: Pull recent commits, PR activity, and ticket updates from connected tools; compile into standup format
- **Output**: Draft standup update ready for user to review and post
- **Requires**: Source control and project tracker connectors for full coverage; works with manual input otherwise

### Daily PR Review Digest
- **When**: 9:00 AM on workdays (configurable)
- **Action**: List open PRs that need the user's review, highlight any that are aging (>48h)
- **Output**: PR review queue with priority ordering

### Weekly Tech Debt Tracker
- **When**: Monday 9:00 AM (configurable)
- **Action**: Summarize known tech debt items, check for any new issues flagged in recent PRs or incidents
- **Output**: Updated tech debt inventory with priority recommendations

### Post-Incident Follow-Up
- **When**: 48 hours after an incident is marked resolved
- **Action**: Remind user to complete the postmortem if not yet done; check that action items from the postmortem are tracked
- **Output**: Gentle reminder with link to incomplete postmortem or untracked action items

## On-Demand Tasks
- Code reviews, debugging sessions, and architecture decisions are triggered by user request
- Deploy checklists are generated when the user initiates a deployment workflow
