---
name: team-autonomy-score
description: Measure team's decision-making independence. Use when hearing "autonomy score," "team independence," "how dependent is my team," "are they ready," or "can my team run things."
---

# Team Autonomy Score

## What This Does

Measures how independently a team operates by scoring four dimensions of autonomy. This is the team-side complement to the Founder Dependency Score — it tells you whether your team is actually stepping into the authority you've given them.

## Framework Phase

**ASSIGN** — The Team Autonomy Score tracks progress through the Assign phase. A high autonomy score means authority transfer is working.

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context:

- Team size and structure
- Authority levels already assigned (from `authority-ladder`)
- How long the team has been operating with current authority
- Any recent delegation wins or failures

## The Four Autonomy Dimensions

### 1. Decision Speed
How quickly does the team make decisions without the founder?

| Score | Description |
|-------|-------------|
| 1 | Team waits days for founder input on routine decisions |
| 2 | Team waits hours — they flag and wait for same-day response |
| 3 | Team decides within the hour for Type 2 decisions |
| 4 | Team decides immediately for all Type 2 and most Type 1 decisions |
| 5 | Team proactively makes decisions the founder didn't even know about |

### 2. Escalation Frequency
How often does the team escalate decisions to the founder?

| Score | Description |
|-------|-------------|
| 1 | Multiple escalations daily — founder is a constant decision point |
| 2 | Several escalations per week — most are unnecessary |
| 3 | A few escalations per week — most are appropriate |
| 4 | Escalations are rare and always warranted |
| 5 | Team handles virtually everything — escalations are truly exceptional |

### 3. Proactive vs. Reactive
Does the team identify and solve problems before they become fires?

| Score | Description |
|-------|-------------|
| 1 | Team only responds when told — founder initiates everything |
| 2 | Team flags problems but waits for founder to solve them |
| 3 | Team flags problems AND proposes solutions |
| 4 | Team identifies and solves most problems independently |
| 5 | Team anticipates problems before they happen and prevents them |

### 4. Ownership Depth
Does the team own outcomes, not just tasks?

| Score | Description |
|-------|-------------|
| 1 | Team completes tasks but doesn't think about outcomes |
| 2 | Team completes tasks and reports results |
| 3 | Team owns the outcome and adjusts approach when results aren't right |
| 4 | Team owns the outcome and improves the process over time |
| 5 | Team owns the outcome, improves the process, and teaches others |

## Scoring

**Total Score: Sum of four dimensions (4-20)**

| Score Range | Autonomy Level | Interpretation |
|-------------|---------------|----------------|
| 4-8 | **Dependent** | Team operates as task-doers. Founder is still the brain. |
| 9-12 | **Emerging** | Team is developing independence but still leans on founder heavily. |
| 13-16 | **Independent** | Team makes most decisions well. Founder can focus on strategy. |
| 17-20 | **Self-Managing** | Team runs the business. Founder is optional for daily operations. |

## Process

1. Score each dimension (1-5) based on observed behavior, not hope
2. Calculate total (4-20)
3. Determine autonomy level
4. Identify the lowest-scoring dimension — that's the priority to improve
5. Create specific improvement actions for the weakest dimension
6. Set a target score and reassessment date

## Output Format

```
# Team Autonomy Score — [Business Name]

## Current Score: [X]/20
## Autonomy Level: [Dependent / Emerging / Independent / Self-Managing]

## Dimension Breakdown
| Dimension | Score | Assessment |
|-----------|-------|-----------|
| Decision Speed | [1-5] | [Brief observation] |
| Escalation Frequency | [1-5] | [Brief observation] |
| Proactive vs. Reactive | [1-5] | [Brief observation] |
| Ownership Depth | [1-5] | [Brief observation] |

## Weakest Dimension: [Name]
[Why this is the bottleneck and what it's costing the business]

## Improvement Plan
### [Weakest Dimension] — From [Current Score] to [Target Score]
1. [Specific action]
2. [Specific action]
3. [Specific action]

## Reassessment
- Next score check: [Date — typically 30 days out]
- Target score: [X]/20

## Recommended Next Step
[Based on weakest dimension: `authority-ladder` for decision speed, `decision-filter` for escalation, `weekly-rhythm` for proactive behavior, `outcome-shifter` for ownership]
```

## Quality Checklist

- [ ] Scores based on observed behavior, not founder hopes
- [ ] All four dimensions assessed — not just the obvious ones
- [ ] Weakest dimension identified with specific improvement actions
- [ ] Target score is realistic — not jumping from 8 to 18
- [ ] Reassessment date set — this is a tracking metric, not a one-time exercise
- [ ] Tone is encouraging — celebrate what's working alongside what needs improvement

## Example

**Input:** "I've had my PM and VA for 6 months. Sarah makes some decisions on her own, Marcus still checks with me on everything."

**Output (excerpt):**
```
## Current Score: 10/20
## Autonomy Level: Emerging

## Dimension Breakdown
| Dimension | Score | Assessment |
|-----------|-------|-----------|
| Decision Speed | 3 | Sarah decides quickly; Marcus waits for approval on everything |
| Escalation Frequency | 2 | 5-8 escalations per week, most from Marcus and most unnecessary |
| Proactive vs. Reactive | 2 | Sarah flags problems but both wait for you to solve them |
| Ownership Depth | 3 | Sarah owns project outcomes; Marcus completes tasks without outcome awareness |

## Weakest Dimension: Escalation Frequency
Marcus escalates 5+ times per week on decisions he could make himself. This creates a bottleneck and prevents him from building confidence.

## Improvement Plan
### Escalation Frequency — From 2 to 4
1. Create a "Decision Quick Reference" card: If [condition], you can decide. If [condition], ask me.
2. Use `decision-filter` to classify Marcus's common escalations as Type 1 or Type 2
3. For 2 weeks, respond to unnecessary escalations with: "What would you decide?" to build confidence
```

## Related Skills

- `authority-ladder` -> `handoff-script` -> this skill (measures the result)
- Low Decision Speed -> revisit `authority-ladder` and `decision-filter`
- Low Ownership -> use `outcome-shifter` to reframe tasks as outcomes
- Rerun monthly to track team development
- **Entry point:** `_router` — Start here if unsure which skill you need
