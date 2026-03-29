# MEMORY

## Structure

### User Profile
- Store sales rep info in `memory/profile.json`
- Fields: name, title, company, product, value_props, competitors, quota (annual/quarterly)

### Pipeline Snapshots
- Store pipeline data in `memory/pipeline/`
- Naming: `YYYY-MM-DD-pipeline-snapshot.json`
- Fields per deal: name, stage, amount, close_date, last_activity, contacts, risk_flags

### Call History
- Store call summaries in `memory/calls/`
- Naming: `YYYY-MM-DD-<account>-call-summary.md`
- Fields: attendees, key_topics, action_items, follow_up_draft, next_steps

### Account Research
- Store research reports in `memory/accounts/`
- Naming: `<company-slug>-research.md`
- Fields: company_overview, key_contacts, recent_news, competitive_landscape, recommended_approach

### Forecast History
- Store forecast snapshots in `memory/forecasts/`
- Naming: `YYYY-MM-DD-forecast.json`
- Fields: quota, commit, upside, best_case, worst_case, gap_analysis

## Index
(Updated as interactions occur)
