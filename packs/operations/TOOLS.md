# TOOLS

## Connector Pattern

This pack uses `~~category` placeholders for tool-agnostic references. Skills reference categories like `~~ITSM`, `~~project tracker`, and `~~knowledge base` — these resolve to whatever MCP server you connect in that category.

See the connector table below for details.

## Required

| Tool | Purpose | MCP Configuration |
|------|---------|-------------------|
| `file_system` | Read/write process docs, reports, runbooks | Workspace access |

## Recommended MCP Servers

| Server | Type | URL | Category |
|--------|------|-----|----------|
| Slack | HTTP | `https://mcp.slack.com/mcp` | ~~chat |
| Google Calendar | HTTP | `https://YOUR_GCAL_MCP_URL` | ~~calendar |
| Gmail | HTTP | `https://YOUR_GMAIL_MCP_URL` | ~~email |
| Microsoft 365 | HTTP | `https://YOUR_MS365_MCP_URL` | ~~email, ~~office suite |
| Notion | HTTP | `https://mcp.notion.com/mcp` | ~~knowledge base |
| Atlassian | HTTP | `https://mcp.atlassian.com/v1/mcp` | ~~knowledge base, ~~project tracker |
| Asana | HTTP | `https://mcp.asana.com/v2/mcp` | ~~project tracker |
| ServiceNow | HTTP | `https://mcp.servicenow.com/mcp` | ~~ITSM |

## Connectors

| Category | Placeholder | Included Servers | Other Options |
|----------|-------------|-----------------|---------------|
| Calendar | `~~calendar` | Google Calendar | Microsoft 365 |
| Chat | `~~chat` | Slack | Microsoft Teams |
| Email | `~~email` | Gmail, Microsoft 365 | -- |
| ITSM | `~~ITSM` | ServiceNow | Zendesk, Freshservice, Jira Service Management |
| Knowledge base | `~~knowledge base` | Notion, Atlassian (Confluence) | Guru, Coda |
| Project tracker | `~~project tracker` | Asana, Atlassian (Jira) | Linear, monday.com, ClickUp |
| Procurement | `~~procurement` | -- | Coupa, SAP Ariba, Zip |
| Office suite | `~~office suite` | Microsoft 365 | Google Workspace |
