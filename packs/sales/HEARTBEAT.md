# HEARTBEAT

## Scheduled Tasks

### Daily Sales Briefing
- **When**: 8:00 AM on workdays (configurable)
- **Action**: Compile today's meetings, pipeline alerts, email priorities, and suggested actions
- **Output**: Prioritized briefing delivered to chat
- **Requires**: Calendar, CRM, and email connectors for full coverage; works in partial mode with any subset

### Weekly Pipeline Health Check
- **When**: Monday 8:30 AM (configurable)
- **Action**: Scan pipeline for stale deals (no activity 14+ days), deals past expected close date, single-threaded opportunities, and forecast gaps
- **Output**: Pipeline health summary with risk flags and recommended actions

### Weekly Forecast Snapshot
- **When**: Friday 4:00 PM (configurable)
- **Action**: Generate weighted forecast with best/likely/worst scenarios based on current pipeline
- **Output**: Forecast summary with commit vs. upside breakdown and gap-to-quota analysis

### Competitive Intel Refresh (Optional)
- **When**: First Monday of each month
- **Action**: Re-check top competitors for product updates, pricing changes, new releases, and press mentions
- **Output**: Alert user only if significant changes detected

## On-Demand Tasks
- Call summaries, outreach drafts, and account research are triggered by user request
- No proactive outreach drafting without user initiation
