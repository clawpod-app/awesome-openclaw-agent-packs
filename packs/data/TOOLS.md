# TOOLS

## Required

| Tool | Purpose | Configuration |
|------|---------|---------------|
| `file_system` | Read/write queries, analyses, dashboards, CSV files | Workspace access |
| `exec` | Run Python scripts for visualization, statistical analysis, data processing | Python 3 runtime |

## Optional

| Tool | Purpose | Configuration |
|------|---------|---------------|
| `browser` | Open generated HTML dashboards for review | Headless browser |

## MCP Integrations

Connector pattern: use `~~category` placeholders in skill files. Any MCP server in that category works.

| Category | Placeholder | Included Servers | Other Options |
|----------|-------------|------------------|---------------|
| Data warehouse | `~~data warehouse` | Snowflake*, Databricks*, BigQuery, Definite | Redshift, PostgreSQL, MySQL |
| Notebook | `~~notebook` | Hex | Jupyter, Deepnote, Observable |
| Product analytics | `~~product analytics` | Amplitude | Mixpanel, Heap |
| Project tracker | `~~project tracker` | Atlassian (Jira/Confluence) | Linear, Asana |

\* Placeholder -- MCP URL not yet configured

### MCP Server Configuration (`.mcp.json`)

```json
{
  "mcpServers": {
    "snowflake": { "type": "http", "url": "" },
    "databricks": { "type": "http", "url": "" },
    "bigquery": { "type": "http", "url": "https://bigquery.googleapis.com/mcp" },
    "hex": { "type": "http", "url": "https://app.hex.tech/mcp" },
    "amplitude": { "type": "http", "url": "https://mcp.amplitude.com/mcp" },
    "atlassian": { "type": "http", "url": "https://mcp.atlassian.com/v1/mcp" },
    "definite": { "type": "http", "url": "https://api.definite.app/v3/mcp/http" }
  }
}
```
