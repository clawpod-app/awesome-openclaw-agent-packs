# MEMORY

## Structure

### Data Source Registry
- Store in `memory/data-sources.json`
- Fields: warehouse_type, dialect, connection_name, default_database, default_schema

### Schema Context
- Store in `memory/schemas/`
- One file per schema or domain: `<schema-name>.md`
- Contains: table descriptions, key columns, relationships, data types, known quirks

### Query Library
- Store reusable queries in `memory/queries/`
- Naming: `<category>-<description>.sql`
- Include comments with purpose, dialect, expected runtime

### Analysis Archive
- Store completed analyses in `memory/analyses/`
- Naming: `YYYY-MM-DD-<topic>.md`
- Include methodology, key findings, caveats

### Dashboard Archive
- Store generated dashboards in `memory/dashboards/`
- Naming: `YYYY-MM-DD-<dashboard-name>.html`

## Index
(Updated as analyses are completed and queries are added to the library)
