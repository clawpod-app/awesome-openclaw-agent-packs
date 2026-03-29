# HEARTBEAT

## Scheduled Tasks

### Data Quality Check (Optional)
- **When**: Daily 7:00 AM
- **Action**: Run data freshness and quality checks on key tables (configured by user)
- **Output**: Data health report -- stale tables, NULL spikes, row count anomalies

### Weekly Metrics Snapshot (Optional)
- **When**: Monday 9:00 AM
- **Action**: Pull key business metrics from configured queries
- **Output**: Weekly metrics dashboard with week-over-week trends

### Schema Change Monitor (Optional)
- **When**: Daily
- **Action**: Detect new/dropped/modified columns in tracked schemas
- **Output**: Schema change alert with impact assessment

## On-Demand
- Primary interaction is question-driven (user asks data questions, requests queries, builds dashboards)
- Proactive monitoring only when user configures watched tables and metrics
