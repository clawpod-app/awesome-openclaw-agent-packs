# TOOLS

## Required

| Tool | Purpose | Configuration |
|------|---------|---------------|
| `file_system` | Read/write journal entries, reconciliations, workpapers, statements | Workspace access |
| `exec` | Run financial calculations, variance analysis, data processing | Python 3 runtime |

## Optional

| Tool | Purpose | Configuration |
|------|---------|---------------|
| `web_search` | Research accounting standards, regulatory guidance | Search API |

## MCP Integrations

Connector pattern: use `~~category` placeholders in skill files. Any MCP server in that category works.

| Category | Placeholder | Included Servers | Other Options |
|----------|-------------|------------------|---------------|
| Data warehouse | `~~data warehouse` | Snowflake*, Databricks*, BigQuery | Redshift, PostgreSQL |
| Email | `~~email` | Microsoft 365 | -- |
| Office suite | `~~office suite` | Microsoft 365 | -- |
| Chat | `~~chat` | Slack | Microsoft Teams |
| ERP / Accounting | `~~erp` | -- (no MCP servers yet) | NetSuite, SAP, QuickBooks, Xero |
| Analytics / BI | `~~analytics` | -- (no MCP servers yet) | Tableau, Looker, Power BI |

\* Placeholder -- MCP URL not yet configured

### MCP Server Configuration (`.mcp.json`)

```json
{
  "mcpServers": {
    "snowflake": { "type": "http", "url": "" },
    "databricks": { "type": "http", "url": "" },
    "bigquery": { "type": "http", "url": "https://bigquery.googleapis.com/mcp" },
    "slack": { "type": "http", "url": "https://mcp.slack.com/mcp" },
    "ms365": { "type": "http", "url": "https://YOUR_MS365_MCP_URL" },
    "google-calendar": { "type": "http", "url": "https://YOUR_GCAL_MCP_URL" },
    "gmail": { "type": "http", "url": "https://YOUR_GMAIL_MCP_URL" }
  }
}
```
