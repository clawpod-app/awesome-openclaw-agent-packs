# TOOLS

## Connector Pattern

This pack uses `~~category` placeholders to stay tool-agnostic. For example, `~~HRIS` could be Workday, BambooHR, Rippling, or any other HRIS with an MCP server.

## Required

| Tool | Purpose | MCP Configuration |
|------|---------|-------------------|
| `file_system` | Read/write offer letters, onboarding docs, review templates | Workspace access |

## Optional MCP Servers

| Category | Placeholder | Included Servers | Other Options |
|----------|-------------|-----------------|---------------|
| ATS | `~~ATS` | -- | Greenhouse, Lever, Ashby, Workable |
| Calendar | `~~calendar` | Google Calendar (`https://YOUR_GCAL_MCP_URL`) | Microsoft 365 |
| Chat | `~~chat` | Slack (`https://mcp.slack.com/mcp`) | Microsoft Teams |
| Compensation data | `~~compensation data` | -- | Pave, Radford, Levels.fyi |
| Email | `~~email` | Gmail (`https://YOUR_GMAIL_MCP_URL`), Microsoft 365 (`https://YOUR_MS365_MCP_URL`) | -- |
| HRIS | `~~HRIS` | -- | Workday, BambooHR, Rippling, Gusto |
| Knowledge base | `~~knowledge base` | Notion (`https://mcp.notion.com/mcp`), Atlassian (`https://mcp.atlassian.com/v1/mcp`) | Guru, Coda |

## .mcp.json

```json
{
  "mcpServers": {
    "slack": { "type": "http", "url": "https://mcp.slack.com/mcp" },
    "google-calendar": { "type": "http", "url": "https://YOUR_GCAL_MCP_URL" },
    "gmail": { "type": "http", "url": "https://YOUR_GMAIL_MCP_URL" },
    "notion": { "type": "http", "url": "https://mcp.notion.com/mcp" },
    "atlassian": { "type": "http", "url": "https://mcp.atlassian.com/v1/mcp" },
    "ms365": { "type": "http", "url": "https://YOUR_MS365_MCP_URL" }
  }
}
```
