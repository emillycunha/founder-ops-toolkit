---
name: brain-dump
description: Extract processes from founder's head. Use when hearing "brain dump," "document what I do," "get it out of my head," "I'm the only one who knows," or "everything is in my head."
---

# Brain Dump

## What This Does

Guides a structured extraction of everything a founder carries in their head — every process, decision, recurring task, and piece of tribal knowledge — and organizes it into a categorized, actionable inventory.

## Framework Phase

**EXTRACT** — This is the first mini-framework in the Operations Reset Framework. Everything starts here. Until systems are visible, they can't be transferred or scaled.

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context (ask if not provided):

- What type of business? (agency, consultancy, coaching, professional services)
- How many team members?
- What does a typical week look like?
- What breaks when the founder is unavailable?

## The Brain Dump Method

### Phase 1: Capture Everything

Use these prompt categories to extract all tasks:

**Daily Operations**
- What do you do every morning before anything else?
- What tasks happen every single day?
- What questions does your team ask you daily?
- What decisions can only you make today?

**Weekly Recurring**
- What meetings do you run or attend?
- What reports or check-ins happen weekly?
- What do you review or approve each week?

**Monthly / Quarterly**
- What financial or strategic tasks happen on a cycle?
- What client milestones do you manage?
- What planning or review sessions do you own?

**Client-Facing**
- What parts of client delivery require you personally?
- What client communication only you handle?
- What onboarding steps involve you?

**Team-Facing**
- What training or mentoring do you do?
- What escalations come to you?
- What hiring or performance decisions are yours?

**Firefighting**
- What emergencies pull you away from planned work?
- What problems recur that you keep solving manually?
- What breaks when you take a day off?

### Phase 2: Categorize Each Task

For every captured task, classify:

1. **Frequency:** Daily, Weekly, Monthly, Quarterly, Ad-hoc
2. **Time per occurrence:** Minutes, estimate
3. **Criticality:** What happens if this doesn't get done? (Nothing / Delay / Revenue loss / Client loss)
4. **Could someone else do this?** Yes / With training / No — only me
5. **Is it documented?** Yes / Partially / No

### Phase 3: Identify Patterns

After capture and categorization, surface:

- Tasks that consume the most total time (frequency x time)
- Tasks with highest criticality that only the founder does
- Tasks that are undocumented and recurring
- Clusters of related tasks that form a single process

## Process

1. Set up a capture document or spreadsheet
2. Walk the founder through each prompt category (Phase 1)
3. List every task without filtering — quantity matters more than quality here
4. Categorize each task (Phase 2)
5. Sort by total time consumed (frequency x time per occurrence)
6. Flag the top 10 highest-time or highest-risk tasks
7. Identify patterns and clusters (Phase 3)
8. Produce the Brain Dump Inventory

## Output Format

```
# Brain Dump Inventory — [Founder Name]

## Summary
- Total tasks captured: [X]
- Estimated weekly hours in founder's head: [X]
- Undocumented recurring tasks: [X]
- Tasks only founder can do: [X]

## Top 10 Time Consumers
| # | Task | Frequency | Time/Occurrence | Weekly Total | Documented? | Only Me? |
|---|------|-----------|-----------------|--------------|-------------|----------|
| 1 | [Task] | [Freq] | [Min] | [Min] | [Y/N] | [Y/N] |

## Full Inventory by Category
### Daily Operations
- [Task]: [Freq] | [Time] | [Criticality] | [Delegatable?] | [Documented?]

### Weekly Recurring
...

### Monthly / Quarterly
...

### Client-Facing
...

### Team-Facing
...

### Firefighting
...

## Patterns Identified
- [Pattern 1]
- [Pattern 2]

## Recommended Next Step
Run `task-categorizer` to sort these into the 4-Box Map (Quick Wins, CEO Zone, Delegation Targets, Eliminate).
```

## Quality Checklist

- [ ] At least 20 tasks captured (most founders have 30-50+)
- [ ] Every prompt category explored — not just the obvious ones
- [ ] Time estimates are realistic, not rounded
- [ ] Criticality assessed honestly — not everything is critical
- [ ] "Only me" classification challenged — is it really only you, or just habit?
- [ ] Patterns identified connect related tasks into processes
- [ ] Tone is warm and supportive — this is an emotional exercise for founders

## Example

**Input:** "I run a branding agency with 4 team members. I do everything from client calls to reviewing designs to sending invoices."

**Output (excerpt):**
```
## Top 10 Time Consumers
| # | Task | Frequency | Time | Weekly Total | Doc? | Only Me? |
|---|------|-----------|------|-------------|------|----------|
| 1 | Client revision calls | 3x/week | 45 min | 135 min | No | Yes |
| 2 | Design review/approval | Daily | 30 min | 150 min | No | Yes |
| 3 | New client onboarding | 2x/month | 90 min | 45 min | Partial | Yes |
| 4 | Invoice creation | Weekly | 60 min | 60 min | No | No |

## Patterns Identified
- Client communication is fragmented across 4 different tasks totaling 5+ hrs/week
- Design approval is a daily bottleneck — team waits on founder every day
- Onboarding has no documented process despite happening regularly
```

## Related Skills

- This skill (start here) -> `task-categorizer` -> `waterline-audit`
- Feed results into `bottleneck-finder` and `founder-dependency-score`
- Extraction targets feed into `sop-generator`
- **Entry point:** `_router` — Start here if unsure which skill you need
