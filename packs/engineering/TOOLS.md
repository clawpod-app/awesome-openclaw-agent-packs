# TOOLS

## Connector Pattern

This pack uses `~~category` placeholders in skill files. Each placeholder maps to whichever MCP server the user connects in that category. The pack is tool-agnostic -- workflows reference categories, not specific products.

## Required

| Tool | Purpose | Configuration |
|------|---------|---------------|
| `web_search` | Research technologies, look up error messages, find documentation | Built-in or search MCP |

## Optional MCP Servers

| Category | Placeholder | Included Servers | Other Options |
|----------|-------------|-----------------|---------------|
| Chat | `~~chat` | Slack (`https://mcp.slack.com/mcp`) | Microsoft Teams |
| Source control | `~~source control` | GitHub (`https://api.github.com/mcp`) | GitLab, Bitbucket |
| Project tracker | `~~project tracker` | Linear (`https://mcp.linear.app/mcp`), Asana (`https://mcp.asana.com/v2/mcp`), Atlassian (`https://mcp.atlassian.com/v1/mcp`) | Shortcut, ClickUp |
| Knowledge base | `~~knowledge base` | Notion (`https://mcp.notion.com/mcp`) | Confluence, Guru, Coda |
| Monitoring | `~~monitoring` | Datadog (`https://mcp.datadoghq.com/mcp`) | New Relic, Grafana, Splunk |
| Incident management | `~~incident management` | PagerDuty (`https://mcp.pagerduty.com/mcp`) | Opsgenie, Incident.io, FireHydrant |
| CI/CD | `~~CI/CD` | -- | CircleCI, GitHub Actions, Jenkins, BuildKite |

## MCP Configuration (.mcp.json)

```json
{
  "mcpServers": {
    "slack": { "type": "http", "url": "https://mcp.slack.com/mcp" },
    "linear": { "type": "http", "url": "https://mcp.linear.app/mcp" },
    "asana": { "type": "http", "url": "https://mcp.asana.com/v2/mcp" },
    "atlassian": { "type": "http", "url": "https://mcp.atlassian.com/v1/mcp" },
    "notion": { "type": "http", "url": "https://mcp.notion.com/mcp" },
    "github": { "type": "http", "url": "https://api.github.com/mcp" },
    "pagerduty": { "type": "http", "url": "https://mcp.pagerduty.com/mcp" },
    "datadog": { "type": "http", "url": "https://mcp.datadoghq.com/mcp" },
    "google-calendar": { "type": "http", "url": "https://YOUR_GCAL_MCP_URL" },
    "gmail": { "type": "http", "url": "https://YOUR_GMAIL_MCP_URL" }
  }
}
```
