---
name: morning-plan
description: Create a prioritized daily schedule with time blocks and energy-optimized task ordering. Trigger with "morning plan", "plan my day", "what should I do today", or "daily schedule".
---

# Morning Plan

Create an optimized daily schedule.

## When to Use
- Start of the day
- User asks to plan their day
- After receiving new tasks that need scheduling

## Steps
1. Review today's calendar commitments
2. Gather pending tasks and their priorities
3. Identify top 3 priorities for the day
4. Map tasks to time slots based on energy patterns (deep work in peak hours)
5. Build in buffer time between meetings and break periods

## Output Format
```markdown
Good morning. Here's your day:

**Top 3 Priorities**:
1. [Task] ([estimated time])
2. [Task] ([estimated time])
3. [Task] ([estimated time])

**Calendar**:
- [Time] [Event] ([duration])

**Suggested Schedule**:
- [Time block] [Task] ([reason for this slot])
- [Time block] [Task]
- ...

[X] open slots for breaks or overflow.
```
