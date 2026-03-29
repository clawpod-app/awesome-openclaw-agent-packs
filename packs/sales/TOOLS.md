# TOOLS

## Connector Pattern

This pack uses `~~category` placeholders in skill files. Each placeholder maps to whichever MCP server the user connects in that category. The pack is tool-agnostic -- workflows reference categories, not specific products.

## Required

| Tool | Purpose | Configuration |
|------|---------|---------------|
| `web_search` | Research prospects, companies, and competitors | Built-in or search MCP |

## Optional MCP Servers

| Category | Placeholder | Included Servers | Other Options |
|----------|-------------|-----------------|---------------|
| Calendar | `~~calendar` | Google Calendar (`https://YOUR_GCAL_MCP_URL`), Microsoft 365 (`https://YOUR_MS365_MCP_URL`) | -- |
| Chat | `~~chat` | Slack (`https://mcp.slack.com/mcp`) | Microsoft Teams |
| Competitive intelligence | `~~competitive intelligence` | Similarweb (`https://mcp.similarweb.com/mcp`) | Crayon, Klue |
| CRM | `~~CRM` | HubSpot (`https://YOUR_HUBSPOT_MCP_URL`), Close (`https://mcp.close.com/mcp`) | Salesforce, Pipedrive, Copper |
| Data enrichment | `~~data enrichment` | Clay (`https://api.clay.com/v3/mcp`), ZoomInfo (`https://mcp.zoominfo.com/mcp`), Apollo (`https://api.apollo.io/mcp`) | Clearbit, Lusha |
| Email | `~~email` | Gmail (`https://YOUR_GMAIL_MCP_URL`), Microsoft 365 (`https://YOUR_MS365_MCP_URL`) | -- |
| Knowledge base | `~~knowledge base` | Notion (`https://mcp.notion.com/mcp`) | Confluence, Guru |
| Meeting transcription | `~~conversation intelligence` | Fireflies (`https://api.fireflies.ai/mcp`) | Gong, Chorus, Otter.ai |
| Project tracker | `~~project tracker` | Atlassian (`https://mcp.atlassian.com/v1/mcp`) | Linear, Asana |
| Sales engagement | `~~sales engagement` | Outreach (`https://mcp.outreach.io/mcp`) | Salesloft, Apollo |

## MCP Configuration (.mcp.json)

```json
{
  "mcpServers": {
    "slack": { "type": "http", "url": "https://mcp.slack.com/mcp" },
    "hubspot": { "type": "http", "url": "https://YOUR_HUBSPOT_MCP_URL" },
    "close": { "type": "http", "url": "https://mcp.close.com/mcp" },
    "clay": { "type": "http", "url": "https://api.clay.com/v3/mcp" },
    "zoominfo": { "type": "http", "url": "https://mcp.zoominfo.com/mcp" },
    "notion": { "type": "http", "url": "https://mcp.notion.com/mcp" },
    "atlassian": { "type": "http", "url": "https://mcp.atlassian.com/v1/mcp" },
    "fireflies": { "type": "http", "url": "https://api.fireflies.ai/mcp" },
    "ms365": { "type": "http", "url": "https://YOUR_MS365_MCP_URL" },
    "apollo": { "type": "http", "url": "https://api.apollo.io/mcp" },
    "outreach": { "type": "http", "url": "https://mcp.outreach.io/mcp" },
    "google-calendar": { "type": "http", "url": "https://YOUR_GCAL_MCP_URL" },
    "gmail": { "type": "http", "url": "https://YOUR_GMAIL_MCP_URL" },
    "similarweb": { "type": "http", "url": "https://mcp.similarweb.com/mcp" }
  }
}
```
