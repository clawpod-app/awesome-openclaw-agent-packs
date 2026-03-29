# TOOLS

## Connector Pattern

This pack uses `~~category` placeholders to stay tool-agnostic. For example, `~~design tool` could be Figma, Sketch, or any other design tool with an MCP server.

## Required

| Tool | Purpose | MCP Configuration |
|------|---------|-------------------|
| `file_system` | Read/write handoff specs, UX copy docs, audit reports | Workspace access |

## Optional MCP Servers

| Category | Placeholder | Included Servers | Other Options |
|----------|-------------|-----------------|---------------|
| Chat | `~~chat` | Slack (`https://mcp.slack.com/mcp`) | Microsoft Teams |
| Design tool | `~~design tool` | Figma (`https://mcp.figma.com/mcp`) | Sketch, Adobe XD, Framer |
| Knowledge base | `~~knowledge base` | Notion (`https://mcp.notion.com/mcp`) | Confluence, Guru, Coda |
| Product analytics | `~~product analytics` | -- | Amplitude, Mixpanel, Heap, FullStory |
| Project tracker | `~~project tracker` | Linear (`https://mcp.linear.app/mcp`), Asana (`https://mcp.asana.com/v2/mcp`), Atlassian (`https://mcp.atlassian.com/v1/mcp`) | Shortcut, ClickUp |
| User feedback | `~~user feedback` | Intercom (`https://mcp.intercom.com/mcp`) | Productboard, Canny, UserVoice, Dovetail |

## .mcp.json

```json
{
  "mcpServers": {
    "slack": { "type": "http", "url": "https://mcp.slack.com/mcp" },
    "figma": { "type": "http", "url": "https://mcp.figma.com/mcp" },
    "linear": { "type": "http", "url": "https://mcp.linear.app/mcp" },
    "asana": { "type": "http", "url": "https://mcp.asana.com/v2/mcp" },
    "atlassian": { "type": "http", "url": "https://mcp.atlassian.com/v1/mcp" },
    "notion": { "type": "http", "url": "https://mcp.notion.com/mcp" },
    "intercom": { "type": "http", "url": "https://mcp.intercom.com/mcp" },
    "google-calendar": { "type": "http", "url": "https://YOUR_GCAL_MCP_URL" },
    "gmail": { "type": "http", "url": "https://YOUR_GMAIL_MCP_URL" }
  }
}
```
