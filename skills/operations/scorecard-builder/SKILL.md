---
name: scorecard-builder
description: Create KPI dashboards by function. Use when hearing "scorecard," "KPIs," "metrics," "dashboard," "what should I track," or "how do I measure this."
---

# Scorecard Builder

## What This Does

Creates a simple, actionable KPI scorecard organized by business function. Gives the founder and team a clear dashboard of what's working, what's not, and where to focus — without drowning in data.

## Framework Phase

**SCALE** — The Scorecard is the measurement layer of the Scale phase. It makes the operating rhythm data-driven rather than gut-driven.

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context:

- Key business functions (from `accountability-matrix` if available)
- Outcome statements (from `outcome-shifter` if available)
- What the founder currently tracks (if anything)
- Revenue model and key business drivers

## Scorecard Design Principles

### 1. Fewer is Better
Most founders track too many things or nothing at all. A good scorecard has 8-15 metrics total, not 50.

### 2. Leading vs. Lagging Indicators

| Type | What It Measures | When You See It | Example |
|------|-----------------|-----------------|---------|
| **Leading** | Activity that predicts future results | Early — before the result happens | Proposals sent this week |
| **Lagging** | Results of past activity | Late — after the result has happened | Revenue this month |

A good scorecard includes BOTH — leading indicators tell you what's coming, lagging indicators tell you what happened.

### 3. The Traffic Light Rule
Every metric should be instantly readable:
- **Green:** On track — no action needed
- **Yellow:** Watch — trending wrong, needs attention soon
- **Red:** Off track — needs immediate action

Define green/yellow/red thresholds for each metric in advance.

## Common KPIs by Business Function

### Sales & Pipeline
| Metric | Type | Example Target |
|--------|------|---------------|
| New leads this week | Leading | 5+ per week |
| Proposals sent | Leading | 3+ per week |
| Close rate | Lagging | 30%+ |
| Monthly revenue | Lagging | $[target] |
| Pipeline value | Leading | 3x monthly target |

### Client Delivery
| Metric | Type | Example Target |
|--------|------|---------------|
| On-time delivery rate | Lagging | 95%+ |
| Client satisfaction score | Lagging | 4.5/5+ |
| Active projects | Leading | [capacity target] |
| First-pass approval rate | Lagging | 80%+ |
| Average project duration | Lagging | Within scope estimate |

### Operations
| Metric | Type | Example Target |
|--------|------|---------------|
| Founder hours on strategic work | Leading | 40%+ of week |
| Team escalation count | Leading | Under 5/week |
| SOP coverage rate | Leading | 80%+ of recurring tasks |
| Founder Dependency Score | Lagging | Under 50 |
| Process completion rate | Lagging | 95%+ |

### Financial
| Metric | Type | Example Target |
|--------|------|---------------|
| Monthly recurring revenue | Lagging | $[target] |
| Accounts receivable (over 30 days) | Lagging | Under 10% |
| Gross margin | Lagging | 60%+ |
| Cash runway | Leading | 3+ months |
| Average project value | Lagging | $[target] |

## Process

1. Identify the 3-4 most important business functions to track
2. For each function, select 2-4 metrics (mix of leading and lagging)
3. Set green/yellow/red thresholds for each metric
4. Assign an owner for each metric (from `accountability-matrix`)
5. Define review cadence (weekly in Monday Alignment and Friday Wrap)
6. Create the scorecard template

## Output Format

```
# Business Scorecard — [Business Name]

## Review Cadence
- Weekly: Monday Alignment + Friday Wrap
- Monthly: Deep review of trends

## Scorecard
### [Function 1: e.g., Sales & Pipeline]
| Metric | Type | Target | Green | Yellow | Red | Owner |
|--------|------|--------|-------|--------|-----|-------|
| [Metric] | [Lead/Lag] | [Target] | [Threshold] | [Threshold] | [Threshold] | [Name] |

### [Function 2: e.g., Client Delivery]
| Metric | Type | Target | Green | Yellow | Red | Owner |
|--------|------|--------|-------|--------|-----|-------|
| [Metric] | [Lead/Lag] | [Target] | [Threshold] | [Threshold] | [Threshold] | [Name] |

### [Function 3: e.g., Operations]
| Metric | Type | Target | Green | Yellow | Red | Owner |
|--------|------|--------|-------|--------|-----|-------|
| [Metric] | [Lead/Lag] | [Target] | [Threshold] | [Threshold] | [Threshold] | [Name] |

## Total Metrics: [X]
- Leading indicators: [X]
- Lagging indicators: [X]

## This Week's Snapshot
| Metric | Status | Value | Notes |
|--------|--------|-------|-------|
| [Metric] | [G/Y/R] | [Value] | [Brief note] |

## Recommended Next Step
Review this scorecard during `weekly-rhythm` Monday Alignment and Friday Wrap.
```

## Quality Checklist

- [ ] 8-15 total metrics — not too few, not too many
- [ ] Mix of leading and lagging indicators
- [ ] Green/yellow/red thresholds defined for every metric
- [ ] Every metric has an owner
- [ ] Scorecard connects to the weekly rhythm (reviewed weekly)
- [ ] Metrics are actually trackable — not aspirational data that doesn't exist yet
- [ ] Founder Dependency Score or Team Autonomy Score included as an operations metric

## Example

**Input:** "I run a web design agency. 3 employees. I want to know if things are going well without having to check everything myself."

**Output (excerpt):**
```
### Sales & Pipeline
| Metric | Type | Target | Green | Yellow | Red | Owner |
|--------|------|--------|-------|--------|-----|-------|
| New inquiries/week | Leading | 4+ | 4+ | 2-3 | 0-1 | Founder |
| Proposals sent/week | Leading | 2+ | 2+ | 1 | 0 | Sarah (PM) |
| Monthly revenue | Lagging | $25K | $25K+ | $20-25K | Under $20K | Founder |

### Client Delivery
| Metric | Type | Target | Green | Yellow | Red | Owner |
|--------|------|--------|-------|--------|-----|-------|
| On-time delivery | Lagging | 95% | 95%+ | 85-94% | Under 85% | Sarah (PM) |
| Revision rounds | Lagging | Under 2 | 0-1 | 2 | 3+ | Sarah (PM) |
```

## Related Skills

- `outcome-shifter` -> `weekly-rhythm` -> this skill
- Metrics connect to `ops-health-check` for overall assessment
- Review alongside `meeting-audit` to ensure meetings drive metric improvement
- **Entry point:** `_router` — Start here if unsure which skill you need
