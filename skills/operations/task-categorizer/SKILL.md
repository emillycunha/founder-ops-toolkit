---
name: task-categorizer
description: Sort tasks into the 4-Box Map (Quick Wins, CEO Zone, Delegation Targets, Eliminate). Use when hearing "what should I delegate," "where do I start," "prioritize my tasks," or "4-box map."
---

# Task Categorizer

## What This Does

Takes a list of founder tasks and sorts them into the 4-Box Map — a two-axis grid of Impact (high/low) x Extraction Difficulty (easy/hard) — to identify what to delegate first, what to keep, and what to stop doing entirely.

## Framework Phase

**EXTRACT** — The 4-Box Map is the second mini-framework in the Extract phase. It takes the raw Brain Dump output and creates a prioritized extraction roadmap.

**Context:** `/context/operations-reset-framework.md`

**Code source of truth:** `src/lib/ops-inventory/scoring.ts` — `getQuadrant()` function

## Before Starting

Gather this context:

- A task list (ideally from `brain-dump` skill output)
- For each task: what it involves, how often, and whether it's currently documented
- Understanding of what "high impact" means for this specific business

## The 4-Box Map

Two axes, four quadrants:

```
                    EASY to Extract
                         |
    QUICK WINS           |      DELEGATION
    High impact,         |      Low impact,
    easy to extract      |      easy to hand off
    Document these first |      Delegate immediately
    ─────────────────────┼─────────────────────
    CEO ZONE             |      ELIMINATE
    High impact,         |      Low impact,
    hard to extract      |      hard to extract
    Keep for now         |      Stop doing these
                         |
                    HARD to Extract
```

### Quadrant Definitions (must match code)

| Quadrant | Impact | Difficulty | Action | Description |
|----------|--------|------------|--------|-------------|
| **Quick Wins** | High | Easy | Document first | High impact, easy to extract. Document these first. |
| **CEO Zone** | High | Hard | Keep for now | High impact, hard to extract. Keep these for now. |
| **Delegation Targets** | Low | Easy | Delegate immediately | Low impact, easy to hand off. Delegate immediately. |
| **Eliminate** | Low | Hard | Stop doing | Low impact, hard to extract. Stop doing these. |

### How to Assess Impact

**High Impact** — The task directly affects:
- Revenue generation or protection
- Client satisfaction or retention
- Strategic direction of the business
- Team performance or development

**Low Impact** — The task is:
- Administrative or maintenance
- Could be done less frequently without consequence
- Doesn't directly affect revenue or client outcomes
- Habit-driven rather than outcome-driven

### How to Assess Extraction Difficulty

**Easy to Extract** — The task:
- Is repeatable and follows a pattern
- Could be taught in under 2 hours
- Doesn't require founder-specific judgment
- Has clear success criteria

**Hard to Extract** — The task:
- Requires deep context or relationships
- Involves nuanced judgment calls
- Changes significantly each time
- Depends on founder's unique expertise

## Process

1. Take the task list (from Brain Dump or provided by founder)
2. For each task, assess Impact: High or Low
3. For each task, assess Extraction Difficulty: Easy or Hard
4. Place each task in the corresponding quadrant
5. Count tasks per quadrant
6. Identify the Quick Wins — these are the extraction starting point
7. Flag Eliminate tasks for the founder to review and stop doing
8. Produce the categorized output

## Output Format

```
# 4-Box Map — [Founder Name]

## Summary
- Total tasks categorized: [X]
- Quick Wins (document first): [X] tasks
- CEO Zone (keep for now): [X] tasks
- Delegation Targets (hand off): [X] tasks
- Eliminate (stop doing): [X] tasks

## Quick Wins — Document These First
These are your highest-leverage extraction targets. High impact, easy to extract.
| Task | Why High Impact | Why Easy to Extract |
|------|----------------|---------------------|
| [Task] | [Reason] | [Reason] |

## CEO Zone — Keep For Now
These require your judgment. Revisit after you've freed up capacity.
| Task | Why High Impact | Why Hard to Extract |
|------|----------------|---------------------|
| [Task] | [Reason] | [Reason] |

## Delegation Targets — Hand Off Immediately
Low stakes, easy handoff. Perfect for building team confidence.
| Task | Current Owner | Delegate To | Notes |
|------|--------------|-------------|-------|
| [Task] | Founder | [Suggestion] | [Any context] |

## Eliminate — Stop Doing These
These consume effort without meaningful return.
| Task | Why Low Impact | What Happens If You Stop |
|------|---------------|--------------------------|
| [Task] | [Reason] | [Consequence — likely minimal] |

## Recommended Next Step
Run `waterline-audit` to separate CEO-level work from systemizable work within each quadrant.
```

## Quality Checklist

- [ ] Every task has both Impact and Difficulty assessed
- [ ] Impact assessment is based on business outcomes, not emotional attachment
- [ ] "Hard to extract" isn't being used as an excuse to avoid delegation
- [ ] Quick Wins identified — there should be at least a few
- [ ] Eliminate quadrant is honest — founders often resist stopping tasks
- [ ] Quadrant names match code exactly: quick-wins, ceo-zone, delegation, eliminate

## Example

**Input:** Brain dump of 15 tasks from a marketing consultancy founder

**Output (excerpt):**
```
## Quick Wins — Document These First
| Task | Why High Impact | Why Easy to Extract |
|------|----------------|---------------------|
| Client weekly status emails | Keeps clients informed, prevents churn | Template-based, repeatable |
| Social media scheduling | Drives lead pipeline | Process is the same every week |
| Invoice generation | Revenue collection | Straightforward, tool-based |

## Eliminate — Stop Doing These
| Task | Why Low Impact | What Happens If You Stop |
|------|---------------|--------------------------|
| Manually formatting reports | Cosmetic only | Use a template instead |
| Attending industry webinars "just in case" | No clear ROI | Reclaim 2 hrs/week |
```

## Related Skills

- `brain-dump` -> this skill -> `waterline-audit`
- Quick Wins feed directly into `sop-generator`
- Delegation Targets feed into `authority-ladder` and `handoff-script`
- **Entry point:** `_router` — Start here if unsure which skill you need
