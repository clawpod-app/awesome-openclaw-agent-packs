# TOOLS

## Required

| Tool | Purpose | Configuration |
|------|---------|---------------|
| `file_system` | Read/write content drafts, reports, briefs | Workspace access |

## Optional

| Tool | Purpose | Configuration |
|------|---------|---------------|
| `web_search` | Research trends, competitors, keywords | Search API |
| `web_fetch` | Fetch reference content and competitor pages | HTTP client |
| `exec` | Run analysis scripts for reporting | Python 3 runtime |

## MCP Integrations

Connector pattern: use `~~category` placeholders in skill files. Any MCP server in that category works.

| Category | Placeholder | Included Servers | Other Options |
|----------|-------------|------------------|---------------|
| Chat | `~~chat` | Slack | Microsoft Teams |
| Design | `~~design` | Canva, Figma | Adobe Creative Cloud |
| Marketing automation | `~~marketing automation` | HubSpot | Marketo, Pardot, Mailchimp |
| Product analytics | `~~product analytics` | Amplitude | Mixpanel, Google Analytics |
| Knowledge base | `~~knowledge base` | Notion | Confluence, Guru |
| SEO | `~~SEO` | Ahrefs, Similarweb | Semrush, Moz |
| Email marketing | `~~email marketing` | Klaviyo | Mailchimp, Brevo, Customer.io |
| Marketing analytics | `~~marketing analytics` | Supermetrics | Google Analytics, Mailchimp, Semrush |

### MCP Server Configuration (`.mcp.json`)

```json
{
  "mcpServers": {
    "slack": { "type": "http", "url": "https://mcp.slack.com/mcp" },
    "canva": { "type": "http", "url": "https://mcp.canva.com/mcp" },
    "figma": { "type": "http", "url": "https://mcp.figma.com/mcp" },
    "hubspot": { "type": "http", "url": "https://YOUR_HUBSPOT_MCP_URL" },
    "amplitude": { "type": "http", "url": "https://mcp.amplitude.com/mcp" },
    "notion": { "type": "http", "url": "https://mcp.notion.com/mcp" },
    "ahrefs": { "type": "http", "url": "https://api.ahrefs.com/mcp/mcp" },
    "similarweb": { "type": "http", "url": "https://mcp.similarweb.com" },
    "klaviyo": { "type": "http", "url": "https://mcp.klaviyo.com/mcp" },
    "supermetrics": { "type": "http", "url": "https://mcp.supermetrics.com/mcp" },
    "google-calendar": { "type": "http", "url": "https://YOUR_GCAL_MCP_URL" },
    "gmail": { "type": "http", "url": "https://YOUR_GMAIL_MCP_URL" }
  }
}
```
