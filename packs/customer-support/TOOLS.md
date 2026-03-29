# TOOLS

## Connector Pattern

This pack uses `~~category` placeholders in skill files. Each placeholder maps to whichever MCP server the user connects in that category. The pack is tool-agnostic -- workflows reference categories, not specific products.

## Required

| Tool | Purpose | Configuration |
|------|---------|---------------|
| `web_search` | Research customer questions, look up documentation, verify product capabilities | Built-in or search MCP |

## Optional MCP Servers

| Category | Placeholder | Included Servers | Other Options |
|----------|-------------|-----------------|---------------|
| Chat | `~~chat` | Slack (`https://mcp.slack.com/mcp`) | Microsoft Teams |
| Email | `~~email` | Microsoft 365 (`https://YOUR_MS365_MCP_URL`) | -- |
| Cloud storage | `~~cloud storage` | Microsoft 365 (`https://YOUR_MS365_MCP_URL`) | -- |
| Support platform | `~~support platform` | Intercom (`https://mcp.intercom.com/mcp`) | Zendesk, Freshdesk, HubSpot Service Hub |
| CRM | `~~CRM` | HubSpot (`https://YOUR_HUBSPOT_MCP_URL`) | Salesforce, Pipedrive |
| Knowledge base | `~~knowledge base` | Guru (`https://mcp.api.getguru.com/mcp`), Notion (`https://mcp.notion.com/mcp`) | Confluence, Help Scout |
| Project tracker | `~~project tracker` | Atlassian (`https://mcp.atlassian.com/v1/mcp`) | Linear, Asana |

## MCP Configuration (.mcp.json)

```json
{
  "mcpServers": {
    "slack": { "type": "http", "url": "https://mcp.slack.com/mcp" },
    "intercom": { "type": "http", "url": "https://mcp.intercom.com/mcp" },
    "hubspot": { "type": "http", "url": "https://YOUR_HUBSPOT_MCP_URL" },
    "guru": { "type": "http", "url": "https://mcp.api.getguru.com/mcp" },
    "atlassian": { "type": "http", "url": "https://mcp.atlassian.com/v1/mcp" },
    "notion": { "type": "http", "url": "https://mcp.notion.com/mcp" },
    "ms365": { "type": "http", "url": "https://YOUR_MS365_MCP_URL" },
    "google-calendar": { "type": "http", "url": "https://YOUR_GCAL_MCP_URL" },
    "gmail": { "type": "http", "url": "https://YOUR_GMAIL_MCP_URL" }
  }
}
```
