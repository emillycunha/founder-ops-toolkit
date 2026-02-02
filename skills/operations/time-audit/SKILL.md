---
name: time-audit
description: Analyze where hours actually go. Use when hearing "time audit," "time tracking," "where's my time," "I'm always busy but nothing gets done," or "I work all day but have nothing to show for it."
---

# Time Audit

## What This Does

Analyzes how a founder actually spends their hours across four work categories, identifies the gap between how they think they spend time and reality, and highlights the biggest time recovery opportunities.

## Framework Phase

**EXTRACT** — The Time Audit reveals the true cost of founder dependency. It provides data that feeds the Brain Dump and 4-Box Map with real numbers instead of guesses.

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context:

- A typical week's activities (or ideally, tracked time data for 1-2 weeks)
- Total working hours per week
- What the founder wants to be spending time on vs. what actually happens

## The Four Time Categories

Every founder task falls into one of four categories:

### 1. Strategic (CEO Work)
Work that moves the business forward long-term.

Examples: Business development, partnership building, product vision, market positioning, high-level client relationships, strategic planning

**Healthy target: 40-50% of working hours**

### 2. Operational (Management Work)
Work that keeps the business running day-to-day.

Examples: Team check-ins, project oversight, quality reviews, client deliverables, process management

**Healthy target: 25-35% of working hours**

### 3. Administrative (Maintenance Work)
Work that supports the business but doesn't directly create value.

Examples: Email, scheduling, invoicing, filing, tool management, data entry, report formatting

**Healthy target: 10-15% of working hours**

### 4. Firefighting (Reactive Work)
Unplanned work responding to problems, emergencies, or things that went wrong.

Examples: Client escalations, team mistakes, broken processes, urgent fixes, last-minute changes

**Healthy target: Under 10% of working hours**

## The Gap Analysis

Most founders discover a significant gap:

| Category | Typical Founder Reality | Healthy Target |
|----------|------------------------|----------------|
| Strategic | 10-15% | 40-50% |
| Operational | 35-45% | 25-35% |
| Administrative | 20-30% | 10-15% |
| Firefighting | 15-25% | Under 10% |

The gap between Strategic (actual) and Strategic (target) is the founder's "lost capacity" — time that should be spent on growth but is consumed by operations.

## Process

1. List all activities from the past week (or use Brain Dump data)
2. Categorize each activity into Strategic, Operational, Administrative, or Firefighting
3. Estimate time spent on each activity
4. Calculate total hours per category
5. Calculate percentages per category
6. Compare to healthy targets
7. Identify the biggest category gaps
8. Flag specific activities that could shift categories (e.g., operational work that could be delegated, firefighting that could be prevented)

## Output Format

```
# Time Audit — [Founder Name]

## Weekly Time Breakdown
| Category | Hours | % of Week | Target % | Gap |
|----------|-------|-----------|----------|-----|
| Strategic | [X] | [X]% | 40-50% | [+/- X]% |
| Operational | [X] | [X]% | 25-35% | [+/- X]% |
| Administrative | [X] | [X]% | 10-15% | [+/- X]% |
| Firefighting | [X] | [X]% | <10% | [+/- X]% |
| **Total** | [X] | 100% | — | — |

## Key Finding
[One sentence: Where the biggest gap is and what it means]

## Time Recovery Opportunities
### Move from Operational to Delegated
| Activity | Current Hours | Could Be | Savings |
|----------|--------------|----------|---------|
| [Activity] | [X] hrs/week | Delegated | [X] hrs |

### Move from Administrative to Automated/Eliminated
| Activity | Current Hours | Could Be | Savings |
|----------|--------------|----------|---------|
| [Activity] | [X] hrs/week | Automated | [X] hrs |

### Prevent Firefighting
| Recurring Fire | Current Hours | Root Cause | Prevention |
|---------------|--------------|------------|------------|
| [Fire] | [X] hrs/week | [Cause] | [Fix] |

## Total Recoverable Hours: [X] hrs/week

## Recommended Next Step
Use `brain-dump` to document the highest-recovery activities, then `task-categorizer` to prioritize extraction.
```

## Quality Checklist

- [ ] All four categories represented — founders often forget administrative and firefighting time
- [ ] Time estimates add up to actual working hours (not more)
- [ ] Gap analysis compares to realistic targets, not perfection
- [ ] Recovery opportunities are specific and actionable
- [ ] Firefighting root causes identified, not just symptoms
- [ ] Tone acknowledges the founder's effort — they're not lazy, they're misallocated

## Example

**Input:** "I work about 50 hours a week running my interior design firm. Three employees."

**Output (excerpt):**
```
## Weekly Time Breakdown
| Category | Hours | % of Week | Target % | Gap |
|----------|-------|-----------|----------|-----|
| Strategic | 5 | 10% | 40-50% | -30% |
| Operational | 22 | 44% | 25-35% | +9% |
| Administrative | 13 | 26% | 10-15% | +11% |
| Firefighting | 10 | 20% | <10% | +10% |

## Key Finding
You're spending 10% of your time on strategy when you should be closer to 40-50%. That's 15-20 hours of strategic capacity lost to operational and admin work every week.
```

## Related Skills

- This skill (diagnostic) -> `brain-dump` -> `task-categorizer`
- Firefighting data feeds into `bottleneck-finder`
- Strategic gap informs `weekly-rhythm` design
- **Entry point:** `_router` — Start here if unsure which skill you need
