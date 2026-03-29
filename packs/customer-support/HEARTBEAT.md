# HEARTBEAT

## Scheduled Tasks

### Shift Start Queue Summary
- **When**: At the start of each support shift (configurable, default 9:00 AM)
- **Action**: Summarize open tickets by priority, highlight P1/P2 tickets, flag aging tickets (no response >4h for P1, >24h for P2)
- **Output**: Queue summary with priority-ordered action list

### Escalation Follow-Up Check
- **When**: Every 4 hours during business hours
- **Action**: Check status of open escalations; flag any that have not received an engineering/product response within the expected SLA
- **Output**: Escalation status update; draft follow-up nudge if SLA is approaching

### Weekly KB Gap Analysis
- **When**: Friday 3:00 PM (configurable)
- **Action**: Review tickets resolved this week; identify common issues that lack a KB article; suggest top 3 articles to write
- **Output**: KB gap report with suggested article topics and resolved ticket references

### Monthly CSAT and Trend Report (Optional)
- **When**: First Monday of each month
- **Action**: Summarize ticket volume trends, category distribution, average resolution time, escalation rate, and recurring issues
- **Output**: Monthly support health report

## On-Demand Tasks
- Triage, response drafting, research, and escalation packaging are triggered by user request
- KB article creation is triggered after issue resolution
