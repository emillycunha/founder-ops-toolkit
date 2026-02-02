---
name: outcome-shifter
description: Convert tasks to measurable outcomes. Use when hearing "outcome," "results not tasks," "what's the goal," "shift from tasks to outcomes," or "measure what matters."
---

# Outcome Shifter

## What This Does

Transforms task-oriented thinking ("do this") into outcome-oriented thinking ("achieve this"). Converts a founder's to-do list into measurable business outcomes that the team can own and track.

## Framework Phase

**SCALE** — The Outcome Shift is the third mini-framework in the Scale phase. It changes how the team thinks — from checking boxes to driving results.

**Context:** `/context/operations-reset-framework.md`

**Code source of truth:** `src/lib/momentum-rhythm/types.ts` — `TaskOutcome` interface (originalTask, businessOutcome, outcomeStatement)

## Before Starting

Gather this context:

- A list of tasks the founder or team regularly does
- The business goals these tasks are supposed to serve
- How success is currently measured (if at all)

## The Outcome Shift Formula (must match code)

Every task transforms through three fields:

```
originalTask     → What you currently write on your to-do list
businessOutcome  → What business result this task actually serves
outcomeStatement → The reframed outcome-focused version
```

### The Transformation Pattern

| Element | Description | Example |
|---------|-------------|---------|
| **Original Task** | What gets written on the to-do list | "Send client status emails" |
| **Business Outcome** | The result this task creates | "Clients feel informed and confident in our progress" |
| **Outcome Statement** | Task reframed as a measurable outcome | "100% of active clients receive a status update by Friday, resulting in zero 'what's the status?' follow-ups" |

### Why This Matters

**Task thinking:** "Did I do the thing?"
**Outcome thinking:** "Did the thing produce the result?"

A team that owns tasks checks boxes. A team that owns outcomes solves problems. When someone owns "zero missed client updates" instead of "send emails," they'll figure out the best way to achieve it — even if the method changes.

## How to Shift

For each task, ask three questions:

### 1. What result does this task create?
Not "what gets done" but "what changes in the business because of this?"

- Sending invoices → Revenue collection happens on time
- Responding to emails → Client questions are resolved within 4 hours
- Running a team meeting → Team is aligned on priorities for the week

### 2. How would you know if it worked?
What's the observable, measurable sign of success?

- Revenue: Invoices paid within 14 days (95%+)
- Speed: Client response time under 4 hours
- Clarity: Zero "what should I work on?" questions after Monday alignment

### 3. Can someone else own this outcome?
If the outcome is clear and measurable, anyone with the right authority can own it. The method might change — that's fine. The result is what matters.

## Process

1. List the tasks to transform (from to-do list, weekly rhythm, or team assignments)
2. For each task, identify the business outcome it serves
3. Rewrite as an outcome statement with a measurable indicator
4. Check: Is the outcome clear enough that someone else could own it?
5. Assign outcome ownership (from `accountability-matrix`)
6. Produce the Outcome Map

## Output Format

```
# Outcome Shift — [Founder Name / Team]

## Transformed Outcomes
| # | Original Task | Business Outcome | Outcome Statement |
|---|--------------|-----------------|-------------------|
| 1 | [Task] | [Result] | [Measurable outcome] |
| 2 | [Task] | [Result] | [Measurable outcome] |
| 3 | [Task] | [Result] | [Measurable outcome] |

## Weekly Outcome Targets
These replace the to-do list as the team's focus:
1. [Outcome statement + owner]
2. [Outcome statement + owner]
3. [Outcome statement + owner]

## Measurement
| Outcome | Metric | Target | Frequency |
|---------|--------|--------|-----------|
| [Outcome] | [What to measure] | [Target] | [Weekly/Monthly] |

## Recommended Next Step
Use `weekly-rhythm` to build these outcomes into the Monday Alignment and Friday Wrap. Use `scorecard-builder` to create an ongoing dashboard.
```

## Quality Checklist

- [ ] Every task has been transformed through all three fields (originalTask, businessOutcome, outcomeStatement)
- [ ] Outcome statements are measurable — not vague aspirations
- [ ] Outcomes focus on results, not activities
- [ ] At least one outcome per key business function
- [ ] Outcomes are clear enough that a team member could own them independently
- [ ] Fields match code interface: originalTask, businessOutcome, outcomeStatement

## Example

**Input:** "My weekly to-do list: send client updates, check project timelines, review deliverables, post on social media, follow up on invoices."

**Output (excerpt):**
```
## Transformed Outcomes
| # | Original Task | Business Outcome | Outcome Statement |
|---|--------------|-----------------|-------------------|
| 1 | Send client updates | Clients feel informed and confident | All active clients receive weekly status updates by Friday 3pm — zero "what's happening?" follow-ups |
| 2 | Check project timelines | Projects deliver on time | 95% of milestones hit within 2 days of target date |
| 3 | Review deliverables | Quality meets client expectations | Deliverables pass quality check on first review (under 10% revision rate) |
| 4 | Post on social media | Pipeline stays warm | 3 posts per week published, maintaining steady lead inquiries |
| 5 | Follow up on invoices | Cash flow stays healthy | 95% of invoices paid within 14 days |
```

## Related Skills

- This skill -> `weekly-rhythm` -> `scorecard-builder`
- Outcome ownership connects to `accountability-matrix`
- Team outcome adoption measured by `team-autonomy-score` (Ownership Depth dimension)
- **Entry point:** `_router` — Start here if unsure which skill you need
