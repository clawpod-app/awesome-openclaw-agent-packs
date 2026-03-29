# Design

> Accelerate design workflows -- critique, design system management, UX writing, accessibility audits, research synthesis, and developer handoff.

## What It Does

- Get structured design feedback on usability, visual hierarchy, accessibility, and consistency
- Audit, document, or extend your design system (components, tokens, patterns)
- Write or review UX copy -- microcopy, error messages, empty states, onboarding flows
- Run WCAG 2.1 AA accessibility audits with specific remediation steps
- Synthesize user research from interviews, surveys, and usability tests
- Generate developer handoff specs with measurements, tokens, states, and edge cases
- Plan and structure user research studies

## Quick Start

### Deploy to ClawPod
[![Deploy](https://img.shields.io/badge/Deploy-ClawPod-FF6B35)](https://clawpod.app/deploy?template=design)

### Self-host
```bash
cp -r ./* ~/.openclaw/workspace/
openclaw restart
```

## Skills Included

| Skill | Description |
|-------|-------------|
| `design-critique` | Evaluate designs for usability, hierarchy, consistency, and principles |
| `design-system` | Audit, document, or extend a design system |
| `ux-copy` | Write or review UX microcopy and content |
| `accessibility-review` | WCAG 2.1 AA compliance audits |
| `research-synthesis` | Synthesize user research into actionable insights |
| `user-research` | Plan user research -- interviews, surveys, usability testing |
| `design-handoff` | Generate developer handoff specs from designs |

## Example Conversation

```
User: /critique
Agent: Share a Figma link, screenshot, or describe your design. What should I focus on?
User: [Shares screenshot of a checkout flow] I'm worried about the form layout on mobile.
Agent: Here's my review, organized by priority:

  **Critical**
  - The "Place Order" button is below the fold on most mobile screens. Move it to a sticky footer.
  - Error states are missing for required fields.

  **Improvements**
  - The form uses 5 different font sizes. Consolidate to 3 for better hierarchy.
  - Spacing between form groups is inconsistent (16px, 24px, 20px). Standardize to 24px.

  **Accessibility**
  - Color contrast on helper text (#999 on #fff) fails WCAG AA. Use #767676 minimum.
  - No visible focus indicators on form inputs.

  Want me to generate a handoff spec with the fixes?
```

## Origin

Adapted from Anthropic's Knowledge Work Plugins (`knowledge-work-plugins/design`).
