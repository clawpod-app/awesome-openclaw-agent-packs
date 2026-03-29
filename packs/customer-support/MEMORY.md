# MEMORY

## Structure

### User Profile
- Store support agent info in `memory/profile.json`
- Fields: name, title, team, company, product, support_tiers, escalation_contacts

### Resolved Tickets
- Store notable resolved tickets in `memory/tickets/`
- Naming: `YYYY-MM-DD-<ticket-id>-<slug>.md`
- Fields: category, priority, root_cause, resolution, time_to_resolve, kb_article_created

### Escalation Log
- Store escalation history in `memory/escalations/`
- Naming: `YYYY-MM-DD-<escalation-slug>.md`
- Fields: issue, severity, affected_accounts, escalated_to, status, resolution, follow_up_actions

### Knowledge Base Index
- Track published KB articles in `memory/kb-index.json`
- Fields per article: id, title, category, created_date, last_reviewed, source_tickets, view_count

### Common Issues Registry
- Track recurring issues in `memory/common-issues.json`
- Fields: issue_pattern, frequency, category, has_kb_article, recommended_response_template

### Customer Context
- Store key account notes in `memory/accounts/`
- Naming: `<account-slug>.md`
- Fields: plan_tier, key_contacts, open_issues, escalation_history, special_notes

## Index
(Updated as interactions occur)
