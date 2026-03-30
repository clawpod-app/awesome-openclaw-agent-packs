# Contributing to Awesome OpenClaw Agent Packs

Thanks for your interest in contributing! Here's how to get involved.

## Submitting a New Pack

### Requirements

Every pack must include these 6 files + a skills directory:

| File | Purpose |
|------|---------|
| `SOUL.md` | Agent identity, personality, values, communication style |
| `AGENTS.md` | Startup behavior, available skills, workflows |
| `HEARTBEAT.md` | Scheduled/recurring tasks |
| `TOOLS.md` | Connected tools and MCP configuration |
| `MEMORY.md` | Cross-session memory and context retention |
| `README.md` | Setup guide with example conversations |
| `skills/` | At least 1 skill with a complete `SKILL.md` |

### Steps

1. Fork this repo
2. Create your pack in `packs/your-pack-name/`
3. Test on a real OpenClaw or [ClawPod](https://clawpod.app) instance
4. Submit a PR using the pull request template

### Skill Format

Each skill lives in `skills/skill-name/SKILL.md` and follows this structure:

```markdown
# Skill Name

## When to Use
Describe when the agent should use this skill.

## Steps
1. Step one
2. Step two
3. ...

## Output Format
What the agent should return.

## Example
Show an example interaction.
```

## Requesting a Pack

Don't see a role you need? [Open a pack request issue](https://github.com/clawpod-app/awesome-openclaw-agent-packs/issues/new?template=pack-request.md).

## Reporting Bugs

Found an issue with an existing pack? [Open a bug report](https://github.com/clawpod-app/awesome-openclaw-agent-packs/issues/new?template=bug-report.md).

## Code of Conduct

Be respectful. We're all here to build useful AI agents.
