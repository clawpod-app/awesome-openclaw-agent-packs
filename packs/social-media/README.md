# Social Media

> Create platform-native social media content that sounds human, stops the scroll, and drives engagement across Twitter, LinkedIn, and more.

## Skills Included
- **social-post**: Write platform-specific posts with hooks, multiple variants, and posting recommendations
- **content-calendar**: Plan weekly content calendars with balanced content mix and optimal timing

## Quick Start
1. Deploy to [ClawPod](https://clawpod.app/templates/social-media?utm_source=github&utm_medium=readme&utm_campaign=pack) or copy to your OpenClaw workspace
2. Share your brand voice and target platforms
3. Start chatting -- try "Tweet about our new PostgreSQL integration"
4. Optionally install TweetClaw for X/Twitter research and reviewed actions

## Optional X/Twitter Integration

[TweetClaw](https://github.com/Xquik-dev/tweetclaw) is an OpenClaw plugin, not an MCP server. It adds X/Twitter search, reply tracking, follower export, media workflows, monitors, and approval-gated actions.

```bash
openclaw plugins install clawhub:@xquik/tweetclaw
openclaw config set tools.alsoAllow '["explore", "tweetclaw"]'
```

Configure credentials through the plugin settings. Keep keys out of prompts, documentation, and shell history. Review every write-like, private, paid, recurring, extraction, monitor, webhook, or account-scoped request before approval.

Xquik is an independent third-party service. Not affiliated with X Corp. "Twitter" and "X" are trademarks of X Corp.

## Example Conversations
```
User: Tweet about our new PostgreSQL integration
Agent: Provides 2-3 tweet variants with different angles (feature-focused, use-case-driven, developer-relatable), with posting time suggestions.
```

## Attribution
Inspired by [mergisi/awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) (MIT License) -- `agents/marketing/social-media/SOUL.md`.
