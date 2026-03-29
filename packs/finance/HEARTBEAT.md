# HEARTBEAT

## Scheduled Tasks

### Close Checklist Tracker
- **When**: Daily during close period (configurable: business day 1-10 of each month)
- **Action**: Review close checklist, track completed vs. outstanding tasks, flag blockers
- **Output**: Close status dashboard with task completion % and next actions

### Reconciliation Reminder
- **When**: Business day 3 of each month
- **Action**: Check which account reconciliations are due and not yet started
- **Output**: Outstanding reconciliation list with deadlines

### Variance Alert (Optional)
- **When**: After financial statements are generated
- **Action**: Flag variances exceeding materiality thresholds with no narrative explanation
- **Output**: Unexplained variance report requiring attention

### SOX Testing Calendar (Optional)
- **When**: Quarterly, 15th of the month following quarter-end
- **Action**: Check which SOX controls are due for testing in the current cycle
- **Output**: SOX testing schedule with sample selection requirements

## On-Demand
- Primary interaction is task-driven (user requests entries, reconciliations, statements)
- Close period tasks are time-sensitive and follow the close calendar
