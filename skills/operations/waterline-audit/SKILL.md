---
name: waterline-audit
description: Separate CEO work from systemizable work. Use when hearing "waterline," "what should I keep," "CEO tasks," "above the line," or "what's really my job."
---

# Waterline Audit

## What This Does

Draws a clear line between work that genuinely requires the founder (above the waterline) and work that can be systemized, documented, and handed off (below the waterline). This creates the extraction priority list.

## Framework Phase

**EXTRACT** — The Waterline Audit is the third mini-framework in the Extract phase. It builds on the Brain Dump and 4-Box Map to create the definitive extraction roadmap.

**Context:** `/context/operations-reset-framework.md`

**Code source of truth:** `src/lib/ops-inventory/scoring.ts` — `calculateWaterlinePercentage()`, `calculatePriorityScore()`, `getImmediateSopTargets()`

## Before Starting

Gather this context:

- Categorized task list (ideally from `task-categorizer` output with 4-Box Map)
- Understanding of what makes this founder's judgment uniquely valuable
- Current team capabilities and capacity

## The Waterline Concept

Think of the founder's work as a ship. The waterline separates two zones:

**Above the Waterline** — CEO Genius Zone
Work that genuinely requires the founder's unique judgment, relationships, or strategic vision. This is where the founder should spend their time.

Criteria for "above":
- Requires founder-specific relationships (key clients, strategic partners)
- Involves irreversible strategic decisions
- Demands pattern recognition only the founder has
- Directly shapes the business direction
- Cannot be taught — it's instinct built from experience

**Below the Waterline** — Systemizable Work
Work that can be documented, templated, and transferred to others. This is the extraction target.

Criteria for "below":
- Follows a repeatable pattern
- Has clear inputs and outputs
- Could be taught to someone in a reasonable timeframe
- Doesn't require founder-specific relationships
- Success is measurable without founder judgment

## Waterline Percentage

The percentage of tasks below the waterline indicates extraction potential:

- **0-25% below:** Founder is mostly doing CEO-level work (healthy)
- **26-50% below:** Meaningful extraction opportunity exists
- **51-75% below:** Founder is doing too much systemizable work (common)
- **76-100% below:** Most of the founder's work should be someone else's job (urgent)

## SOP Priority Scoring

Tasks below the waterline are scored for extraction priority. The scoring from the code:

| Factor | Score Boost |
|--------|-------------|
| Quick Win quadrant | +40 (highest priority — easy + high impact) |
| Delegation quadrant | +30 (easy to hand off) |
| CEO Zone quadrant | +20 (important but harder) |
| Eliminate quadrant | +10 (lowest priority) |
| Below waterline | +25 |
| High impact | +15 |
| Easy to extract | +10 |

Top 5 highest-scoring tasks become the immediate SOP targets.

## Process

1. Take the categorized task list (from `task-categorizer` or direct input)
2. For each task, apply the above/below criteria
3. Mark each task as above or below the waterline
4. Calculate the waterline percentage
5. Score below-waterline tasks for SOP priority
6. Identify the top 5 immediate SOP targets
7. Estimate hours that could be reclaimed
8. Produce the Waterline Audit output

## Output Format

```
# Waterline Audit — [Founder Name]

## Waterline Summary
- Total tasks audited: [X]
- Above the waterline (CEO work): [X] tasks ([X]%)
- Below the waterline (systemizable): [X] tasks ([X]%)
- Estimated weekly hours reclaimable: [X]

## Waterline Assessment
[Brief interpretation of the waterline percentage — what it means for this founder]

## Above the Waterline — Your CEO Zone
These are genuinely yours. Protect this time.
| Task | Why It Stays Above |
|------|-------------------|
| [Task] | [Specific reason this needs the founder] |

## Below the Waterline — Extraction Targets
These should be documented and handed off.
| Task | Quadrant | Priority Score | Why Below |
|------|----------|---------------|-----------|
| [Task] | [Quick Win/Delegation/etc.] | [Score] | [Reason] |

## Top 5 SOP Targets (Start Here)
| # | Task | Priority Score | Reason |
|---|------|---------------|--------|
| 1 | [Task] | [Score] | [e.g., "High impact, easy to document"] |
| 2 | [Task] | [Score] | [Reason] |
| 3 | [Task] | [Score] | [Reason] |
| 4 | [Task] | [Score] | [Reason] |
| 5 | [Task] | [Score] | [Reason] |

## Recommended Next Step
Use `sop-generator` to document the top 5 SOP targets. Then use `authority-ladder` to define who takes ownership.
```

## Quality Checklist

- [ ] Every task has a clear above/below classification with reasoning
- [ ] "Above the waterline" isn't being used to hoard tasks out of habit or fear
- [ ] Waterline percentage is calculated accurately
- [ ] SOP priority scoring matches the code logic
- [ ] Top 5 targets are genuinely actionable — not aspirational
- [ ] Hours estimate is conservative, not optimistic
- [ ] Assessment tone acknowledges that letting go is hard

## Example

**Input:** 20 categorized tasks from a web design agency founder

**Output (excerpt):**
```
## Waterline Summary
- Total tasks audited: 20
- Above the waterline: 5 tasks (25%)
- Below the waterline: 15 tasks (75%)
- Estimated weekly hours reclaimable: 12

## Top 5 SOP Targets
| # | Task | Priority Score | Reason |
|---|------|---------------|--------|
| 1 | Client onboarding emails | 90 | High impact, easy to document |
| 2 | Weekly project status updates | 80 | Ready to hand off immediately |
| 3 | Design file organization | 55 | Ready to hand off immediately |
| 4 | Proposal formatting | 75 | High impact, easy to document |
| 5 | Invoice follow-ups | 65 | Ready to hand off immediately |
```

## Related Skills

- `brain-dump` -> `task-categorizer` -> this skill -> `sop-generator`
- Feed waterline results into `founder-dependency-score`
- Top targets feed into `sop-generator` and then `handoff-script`
- **Entry point:** `_router` — Start here if unsure which skill you need
