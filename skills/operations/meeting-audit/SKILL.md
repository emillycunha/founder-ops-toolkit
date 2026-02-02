---
name: meeting-audit
description: Analyze meeting load and necessity. Use when hearing "too many meetings," "meeting audit," "calendar review," "meetings are killing my productivity," or "do I need this meeting."
---

# Meeting Audit

## What This Does

Evaluates every recurring meeting for necessity, efficiency, and ROI. Identifies meetings to keep, modify, or eliminate — reclaiming hours for strategic work.

## Framework Phase

**SCALE** — The Meeting Audit optimizes the operating rhythm. Meetings are the most visible symptom of poor delegation and missing systems.

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context:

- List of all recurring meetings (weekly, biweekly, monthly)
- For each: who attends, duration, purpose, frequency
- The founder's current weekly meeting hours
- Weekly Rhythm (from `weekly-rhythm` if available) — which meetings conflict with Essential Blocks?

## Meeting Classification

### The Four Meeting Types

| Type | Purpose | Should Exist? |
|------|---------|--------------|
| **Decision** | Make a specific decision that can't be made async | Only if the decision genuinely requires live discussion |
| **Status** | Share updates on progress | Rarely — most status can be async (3-Question Filter) |
| **Creative** | Brainstorm, plan, or solve complex problems together | Yes — collaborative work often needs live interaction |
| **Social** | Team bonding, culture, morale | Yes — but keep intentional and brief |

### The Necessity Test

For each meeting, ask:

1. **What decision or outcome does this meeting produce?**
   - If no clear output → Eliminate or convert to async

2. **Could this be an email, Slack message, or shared doc instead?**
   - If yes → Convert to async update

3. **Does the founder need to be in this meeting?**
   - If no → Remove founder, let team run it

4. **Does everyone in this meeting need to be here?**
   - If no → Reduce attendees to essential only

5. **Is this meeting the right length?**
   - Most 60-min meetings can be 30. Most 30-min meetings can be 15.

## The 3-Question Filter (replaces most status meetings)

Instead of a status meeting, team members submit a brief async update:

1. **Green lights:** What's on track?
2. **Yellow lights:** What's stuck or waiting on someone?
3. **Red lights:** What fires need immediate attention?

This takes 5 minutes to write and 3 minutes to read — compared to a 30-60 minute meeting with the same information.

## Process

1. List all recurring meetings the founder attends
2. For each meeting: type, duration, frequency, attendees
3. Apply the Necessity Test (5 questions)
4. Classify each meeting: Keep, Modify, Convert to Async, or Eliminate
5. Calculate time reclaimed
6. Check for conflicts with Essential Blocks from `weekly-rhythm`
7. Produce the Meeting Audit

## Output Format

```
# Meeting Audit — [Founder Name]

## Current Meeting Load
- Total recurring meetings: [X]
- Weekly meeting hours: [X]
- % of working week in meetings: [X]%

## Meeting Audit Results
### Keep (as-is)
| Meeting | Type | Duration | Frequency | Why Keep |
|---------|------|----------|-----------|----------|
| [Meeting] | [Type] | [Duration] | [Freq] | [Reason] |

### Modify
| Meeting | Change | Current | New | Time Saved |
|---------|--------|---------|-----|-----------|
| [Meeting] | [Shorten/Remove founder/Reduce freq] | [Current] | [New] | [Min/week] |

### Convert to Async
| Meeting | Replace With | Time Saved |
|---------|-------------|-----------|
| [Meeting] | [3-Question Filter / Shared doc / Slack update] | [Min/week] |

### Eliminate
| Meeting | Why | Time Saved |
|---------|-----|-----------|
| [Meeting] | [Reason] | [Min/week] |

## Time Reclaimed
- Meetings eliminated: [X] hrs/week
- Meetings shortened: [X] hrs/week
- Founder removed from: [X] meetings ([X] hrs/week)
- **Total reclaimed: [X] hrs/week**

## New Meeting Load
- Total recurring meetings: [X] (down from [X])
- Weekly meeting hours: [X] (down from [X])
- % of working week: [X]% (down from [X]%)

## Recommended Next Step
Update `weekly-rhythm` to protect the reclaimed time. Use the 3-Question Filter for async check-ins.
```

## Quality Checklist

- [ ] Every recurring meeting evaluated — not just the obvious time-wasters
- [ ] Necessity Test applied with honest answers
- [ ] Status meetings challenged — most can be async
- [ ] Founder attendance questioned — do you actually need to be there?
- [ ] Meeting lengths challenged — default to shorter
- [ ] 3-Question Filter recommended for status replacements
- [ ] Reclaimed time is protected, not just freed (connects to `weekly-rhythm`)

## Example

**Input:** "I have 12 hours of meetings per week. Team standup daily (30 min), client check-ins (3x week, 45 min each), team 1:1s (2x week, 30 min each), and a monthly planning session (2 hrs)."

**Output (excerpt):**
```
## Meeting Audit Results
### Modify
| Meeting | Change | Current | New | Time Saved |
|---------|--------|---------|-----|-----------|
| Team standup | Reduce to 3x/week, 15 min | 5x30m = 150m | 3x15m = 45m | 105 min |
| Client check-ins | Founder attends only 1, PM runs other 2 | 3x45m = 135m | 1x45m = 45m | 90 min |

### Convert to Async
| Meeting | Replace With | Time Saved |
|---------|-------------|-----------|
| 2 of 5 standups | 3-Question Filter via Slack | 60 min |

## Total Reclaimed: 4.25 hrs/week
```

## Related Skills

- `outcome-shifter` -> `weekly-rhythm` -> `scorecard-builder` -> this skill
- Reclaimed time feeds into `weekly-rhythm` Strategic Margin
- 3-Question Filter connects to `team-autonomy-score` (Proactive vs. Reactive)
- **Entry point:** `_router` — Start here if unsure which skill you need
