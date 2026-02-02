---
name: weekly-rhythm
description: Build founder operating cadence with the 5 Essential Blocks. Use when hearing "weekly rhythm," "ideal week," "operating cadence," "weekly schedule," or "how should I structure my week."
---

# Weekly Rhythm

## What This Does

Designs a predictable weekly operating cadence using the 5 Essential Blocks, calculates Strategic Margin, and installs the rhythm that makes the business run without heroics.

## Framework Phase

**SCALE** — The Weekly Rhythm is the first mini-framework in the Scale phase. It replaces reactive firefighting with a predictable, sustainable operating cadence.

**Context:** `/context/operations-reset-framework.md`

**Code source of truth:** `src/lib/momentum-rhythm/types.ts` — `BlockType`, `BlockDefinition`, `StrategicMarginMetrics`

## Before Starting

Gather this context:

- Current working hours (start time, end time, days)
- What the founder's current week looks like (chaotic, semi-structured, or structured)
- Top priorities from `outcome-shifter` (if available)
- Team check-in needs from `accountability-matrix` (if available)

## The 5 Essential Blocks (must match code)

| Block | Duration | Day | Purpose |
|-------|----------|-----|---------|
| **Monday Alignment** | 30 min | Monday | Set weekly priorities, review last week's outcomes, align team |
| **CEO Deep Work** | 4 hrs | Flexible | Protected strategy time — no meetings, no Slack, no email |
| **Mid-Week Pulse** | 15 min | Wednesday | Quick bottleneck check — what's stuck, what needs attention |
| **Friday Wrap** | 30 min | Friday | Review outcomes vs. targets, celebrate wins, set up next week |
| **Buffer Zone** | 1 hr | Flexible | Scheduled "fire time" — dedicated space for the unexpected |

### Block Details

**Monday Alignment (30 min)**
- Review last week's outcomes (from `outcome-shifter`)
- Set this week's top 3 priorities
- Identify any blockers
- Align team on what matters this week

**CEO Deep Work (4 hrs)**
- Protected strategic time — the highest-leverage block
- No meetings, no Slack, no notifications
- Work ON the business: strategy, relationships, growth
- This is the time that creates compound returns

**Mid-Week Pulse (15 min)**
- Quick team check-in using the 3-Question Filter:
  - Green lights: What's on track?
  - Yellow lights: What's stuck or waiting on someone?
  - Red lights: What fires are burning?
- Catch problems before they become Friday emergencies

**Friday Wrap (30 min)**
- Review: Did we hit our outcomes for the week?
- Celebrate: What went well?
- Learn: What didn't work and why?
- Set up: What's the #1 priority for next Monday?

**Buffer Zone (1 hr)**
- Intentional space for unplanned work
- Instead of fires interrupting Deep Work, they go here
- If no fires: use for learning, reading, or low-priority tasks
- Prevents the entire week from being derailed by surprises

## Strategic Margin (must match code)

**Formula:**
```
Strategic Margin = (Deep Work Minutes + Buffer Minutes) / Total Working Minutes
```

**Thresholds:**
- **Under 20%:** Burnout Alert — founder has almost no protected time
- **20-30%:** Minimum viable — functional but tight
- **30-40%:** Healthy — good balance of execution and strategy
- **40%+:** Optimal — founder has real space to work ON the business

## Process

1. Define working hours (start, end, days per week)
2. Place the 5 Essential Blocks on the calendar
3. Calculate Strategic Margin
4. Check for Burnout Alert (under 20%)
5. Adjust if needed — the goal is minimum 20% Strategic Margin
6. Add the 3-Question Filter template for Mid-Week Pulse
7. Produce the weekly calendar

## Output Format

```
# Weekly Rhythm — [Founder Name]

## Working Hours
- Days: [Mon-Fri / other]
- Hours: [Start] to [End]
- Total weekly hours: [X]

## The 5 Essential Blocks
| Block | Day | Time | Duration |
|-------|-----|------|----------|
| Monday Alignment | Monday | [Time] | 30 min |
| CEO Deep Work | [Day] | [Time] | 4 hrs |
| Mid-Week Pulse | Wednesday | [Time] | 15 min |
| Friday Wrap | Friday | [Time] | 30 min |
| Buffer Zone | [Day] | [Time] | 1 hr |

## Strategic Margin
- Deep Work: [X] min
- Buffer: [X] min
- Total Working: [X] min
- **Strategic Margin: [X]%**
- Status: [Burnout Alert / Minimum / Healthy / Optimal]

## 3-Question Filter (Mid-Week Pulse Template)
**Team members report:**
1. Green lights — What's on track this week?
2. Yellow lights — What's stuck or waiting on someone?
3. Red lights — What fires need immediate attention?

## Weekly Calendar
| Time | Monday | Tuesday | Wednesday | Thursday | Friday |
|------|--------|---------|-----------|----------|--------|
| [Start] | Alignment | [Open] | [Open] | [Open] | [Open] |
| ... | [Blocks placed] | ... | Pulse | ... | Wrap |

## Recommended Next Step
Use `outcome-shifter` to define the outcomes you'll track each week, then `scorecard-builder` for ongoing metrics.
```

## Quality Checklist

- [ ] All 5 Essential Blocks placed on the calendar
- [ ] Block names and durations match code exactly
- [ ] Strategic Margin calculated correctly
- [ ] Burnout Alert triggered if under 20%
- [ ] Deep Work block is truly protected — no meetings scheduled during it
- [ ] Buffer Zone exists — don't fill every minute
- [ ] Calendar is realistic — not an aspirational fantasy

## Example

**Input:** "I work Monday-Friday, 9am-5pm. Currently no structure — I just react to whatever comes in."

**Output (excerpt):**
```
## The 5 Essential Blocks
| Block | Day | Time | Duration |
|-------|-----|------|----------|
| Monday Alignment | Monday | 9:00 AM | 30 min |
| CEO Deep Work | Tuesday | 9:00 AM | 4 hrs |
| Mid-Week Pulse | Wednesday | 9:00 AM | 15 min |
| Friday Wrap | Friday | 4:00 PM | 30 min |
| Buffer Zone | Thursday | 3:00 PM | 1 hr |

## Strategic Margin
- Deep Work: 240 min + Buffer: 60 min = 300 min
- Total Working: 2400 min (40 hrs)
- **Strategic Margin: 12.5%**
- Status: Burnout Alert — under 20%. Consider adding a second Deep Work block (even 2 hours) to reach the minimum.
```

## Related Skills

- `outcome-shifter` -> this skill -> `scorecard-builder` -> `meeting-audit`
- Strategic Margin informs `capacity-planner`
- 3-Question Filter connects to `team-autonomy-score`
- **Entry point:** `_router` — Start here if unsure which skill you need
