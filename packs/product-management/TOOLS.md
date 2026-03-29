# TOOLS

## Connector Pattern

This pack uses `~~category` placeholders to stay tool-agnostic. For example, `~~project tracker` could be Linear, Asana, Jira, or any other tracker with an MCP server.

## Required

| Tool | Purpose | MCP Configuration |
|------|---------|-------------------|
| `file_system` | Read/write specs, roadmaps, research docs | Workspace access |

## Optional MCP Servers

| Category | Placeholder | Included Servers | Other Options |
|----------|-------------|-----------------|---------------|
| Calendar | `~~calendar` | Google Calendar (`https://YOUR_GCAL_MCP_URL`) | Microsoft 365 |
| Chat | `~~chat` | Slack (`https://mcp.slack.com/mcp`) | Microsoft Teams |
| Competitive intelligence | `~~competitive intelligence` | Similarweb (`https://mcp.similarweb.com/mcp`) | Crayon, Klue |
| Design | `~~design` | Figma (`https://mcp.figma.com/mcp`) | Sketch, Adobe XD |
| Email | `~~email` | Gmail (`https://YOUR_GMAIL_MCP_URL`) | Microsoft 365 |
| Knowledge base | `~~knowledge base` | Notion (`https://mcp.notion.com/mcp`) | Confluence, Guru, Coda |
| Meeting transcription | `~~meeting transcription` | Fireflies (`https://api.fireflies.ai/mcp`) | Gong, Dovetail, Otter.ai |
| Product analytics | `~~product analytics` | Amplitude (`https://mcp.amplitude.com/mcp`), Pendo (`https://app.pendo.io/mcp/v0/shttp`) | Mixpanel, Heap, FullStory |
| Project tracker | `~~project tracker` | Linear (`https://mcp.linear.app/mcp`), Asana (`https://mcp.asana.com/v2/mcp`), monday.com (`https://mcp.monday.com/mcp`), ClickUp (`https://mcp.clickup.com/mcp`), Atlassian (`https://mcp.atlassian.com/v1/mcp`) | Shortcut, Basecamp |
| User feedback | `~~user feedback` | Intercom (`https://mcp.intercom.com/mcp`) | Productboard, Canny, UserVoice |

## .mcp.json

```json
{
  "mcpServers": {
    "slack": { "type": "http", "url": "https://mcp.slack.com/mcp" },
    "linear": { "type": "http", "url": "https://mcp.linear.app/mcp" },
    "asana": { "type": "http", "url": "https://mcp.asana.com/v2/mcp" },
    "monday": { "type": "http", "url": "https://mcp.monday.com/mcp" },
    "clickup": { "type": "http", "url": "https://mcp.clickup.com/mcp" },
    "atlassian": { "type": "http", "url": "https://mcp.atlassian.com/v1/mcp" },
    "notion": { "type": "http", "url": "https://mcp.notion.com/mcp" },
    "figma": { "type": "http", "url": "https://mcp.figma.com/mcp" },
    "amplitude": { "type": "http", "url": "https://mcp.amplitude.com/mcp" },
    "pendo": { "type": "http", "url": "https://app.pendo.io/mcp/v0/shttp" },
    "intercom": { "type": "http", "url": "https://mcp.intercom.com/mcp" },
    "fireflies": { "type": "http", "url": "https://api.fireflies.ai/mcp" },
    "google-calendar": { "type": "http", "url": "https://YOUR_GCAL_MCP_URL" },
    "gmail": { "type": "http", "url": "https://YOUR_GMAIL_MCP_URL" },
    "similarweb": { "type": "http", "url": "https://mcp.similarweb.com/mcp" }
  }
}
```
