# MEMORY

## Structure

### User Profile
- Store engineer info in `memory/profile.json`
- Fields: name, title, team, company, tech_stack, default_branch, deploy_process

### Architecture Decisions
- Store ADRs in `memory/adrs/`
- Naming: `ADR-NNNN-<title-slug>.md`
- Fields: status, context, decision, options_considered, trade_offs, consequences

### Incident History
- Store postmortems in `memory/incidents/`
- Naming: `YYYY-MM-DD-<incident-slug>.md`
- Fields: severity, timeline, root_cause, impact, action_items, lessons_learned

### Code Review Notes
- Store recurring review findings in `memory/reviews/`
- Naming: `<repo-or-service>-review-patterns.md`
- Purpose: track repeated issues to provide targeted review guidance

### Tech Debt Registry
- Store tech debt inventory in `memory/tech-debt.json`
- Fields per item: id, description, category, severity, effort_estimate, owner, status, created_date

### Debug Sessions
- Store resolved debugging sessions in `memory/debug/`
- Naming: `YYYY-MM-DD-<issue-slug>.md`
- Fields: symptoms, root_cause, fix_applied, prevention_steps

## Index
(Updated as interactions occur)
