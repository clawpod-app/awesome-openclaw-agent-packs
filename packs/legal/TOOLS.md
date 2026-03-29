# TOOLS

## Required

| Tool | Purpose | Configuration |
|------|---------|---------------|
| `file_system` | Read contracts, playbooks, templates; write analyses and briefs | Workspace access |

## Optional

| Tool | Purpose | Configuration |
|------|---------|---------------|
| `web_search` | Research legal questions, regulations, precedents | Search API |
| `web_fetch` | Fetch regulatory guidance, legal resources | HTTP client |

## MCP Integrations

Connector pattern: use `~~category` placeholders in skill files. Any MCP server in that category works.

| Category | Placeholder | Included Servers | Other Options |
|----------|-------------|------------------|---------------|
| Calendar | `~~calendar` | Google Calendar | Microsoft 365 |
| Chat | `~~chat` | Slack | Microsoft Teams |
| Cloud storage | `~~cloud storage` | Box, Egnyte | Dropbox, SharePoint, Google Drive |
| CLM | `~~CLM` | -- | Ironclad, Agiloft |
| CRM | `~~CRM` | -- | Salesforce, HubSpot |
| Email | `~~email` | Gmail | Microsoft 365 |
| E-signature | `~~e-signature` | DocuSign | Adobe Sign |
| Office suite | `~~office suite` | Microsoft 365 | Google Workspace |
| Project tracker | `~~project tracker` | Atlassian (Jira/Confluence) | Linear, Asana |

### MCP Server Configuration (`.mcp.json`)

```json
{
  "mcpServers": {
    "slack": { "type": "http", "url": "https://mcp.slack.com/mcp" },
    "box": { "type": "http", "url": "https://mcp.box.com" },
    "egnyte": { "type": "http", "url": "https://mcp-server.egnyte.com/mcp" },
    "atlassian": { "type": "http", "url": "https://mcp.atlassian.com/v1/mcp" },
    "ms365": { "type": "http", "url": "https://YOUR_MS365_MCP_URL" },
    "docusign": { "type": "http", "url": "https://mcp.docusign.com/mcp" },
    "google-calendar": { "type": "http", "url": "https://YOUR_GCAL_MCP_URL" },
    "gmail": { "type": "http", "url": "https://YOUR_GMAIL_MCP_URL" }
  }
}
```
