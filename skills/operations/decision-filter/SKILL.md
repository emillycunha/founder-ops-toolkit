---
name: decision-filter
description: Categorize Type 1 vs Type 2 decisions using the Decision Filter. Use when hearing "decision filter," "what needs approval," "reversible," "one-way door," "two-way door," or "can they decide this."
---

# Decision Filter

## What This Does

Classifies business decisions into Type 1 (One-Way Door — hard to reverse, needs founder approval) and Type 2 (Two-Way Door — reversible, team can decide). Includes the 3-Question Bypass to upgrade team authority on borderline decisions.

## Framework Phase

**ASSIGN** — The Decision Filter is the third mini-framework in the Assign phase. It gives teams a clear rule for when they can act independently vs. when they need to check.

**Context:** `/context/operations-reset-framework.md`

**Code source of truth:** `src/lib/authority-transfer/types.ts` — `DecisionType` (type-1, type-2), `DecisionCategory`, `BypassAnswers`

## Before Starting

Gather this context:

- List of recurring decisions the founder currently makes
- Which decisions cause the most bottlenecks (from `bottleneck-finder` if available)
- Team member authority levels (from `authority-ladder` if available)

## The Two Decision Types (must match code)

### Type 1: One-Way Door
Decisions that are hard or impossible to reverse. These need founder involvement.

**Characteristics:**
- Significant financial commitment
- Long-term contractual obligations
- Reputation or brand impact
- Team structure changes (hiring/firing)
- Strategic direction shifts

**Examples:**
- Signing a 12-month vendor contract
- Hiring a new team member
- Changing pricing structure
- Taking on a client outside your niche
- Making a public brand statement

### Type 2: Two-Way Door
Decisions that are easily reversible. Team can make these without founder approval.

**Characteristics:**
- Low financial risk
- Easily changed or undone
- Short-term impact
- Operational in nature
- Won't affect client relationships negatively

**Examples:**
- Rescheduling a non-urgent meeting
- Choosing a project management tool feature to try
- Responding to a routine client question
- Adjusting internal workflow steps
- Ordering office supplies

## Decision Categories (from code)

Classify each decision by domain:

| Category | Description | Examples |
|----------|-------------|---------|
| **Financial** | Money in or out | Pricing, refunds, purchases, investments |
| **Client** | Client-facing decisions | Scope, timelines, communication, deliverables |
| **Team** | People decisions | Hiring, schedules, performance, roles |
| **Operational** | Internal process decisions | Tools, workflows, procedures, priorities |

## The 3-Question Bypass (from code)

For decisions that seem like Type 1 but might be Type 2, run this bypass test:

### Question 1: What would you do if the founder were unreachable for 3 days?
- If the team has a reasonable answer -> potential upgrade to Type 2
- If the team would be stuck -> stays Type 1

### Question 2: What's the worst-case outcome if the decision is wrong?
- **Low risk:** Minor inconvenience, easily fixed -> upgrade to Type 2
- **Medium risk:** Some cost or rework needed -> Type 2 with inform
- **High risk:** Significant financial, legal, or relationship damage -> stays Type 1

### Question 3: Can you test at small scale first?
- **Yes:** Run a small test, learn, then decide bigger -> upgrade to Type 2
- **No:** The decision is all-or-nothing -> stays Type 1

**Bypass Result:** If 2 of 3 questions favor upgrading, the decision can be reclassified as Type 2 with the team member at Level 3 (Decide & Inform).

## Process

1. List all recurring decisions the founder makes
2. Categorize each: Financial, Client, Team, or Operational
3. Classify each as Type 1 or Type 2 using the criteria
4. For borderline decisions, apply the 3-Question Bypass
5. Mark upgraded decisions (wasUpgraded = true)
6. Assign each decision to the appropriate team member and authority level
7. Create the Decision Authority Map

## Output Format

```
# Decision Filter — [Business Name]

## Summary
- Total decisions mapped: [X]
- Type 1 (Founder Required): [X]
- Type 2 (Team Can Decide): [X]
- Upgraded via Bypass: [X]

## Type 1 Decisions — Founder Required
| Decision | Category | Why Type 1 | Assigned To |
|----------|----------|-----------|-------------|
| [Decision] | [Cat] | [Reason] | Founder |

## Type 2 Decisions — Team Can Decide
| Decision | Category | Assigned To | Authority Level |
|----------|----------|-------------|----------------|
| [Decision] | [Cat] | [Name] | Level [X] |

## Bypass Upgrades
| Decision | Original | 3-Question Result | New Classification |
|----------|----------|-------------------|-------------------|
| [Decision] | Type 1 | [2/3 or 3/3 favor upgrade] | Type 2 — Decide & Inform |

## Quick Reference for the Team
**You CAN decide without asking:**
- [List of Type 2 decisions]

**Always check with [Founder Name] first:**
- [List of Type 1 decisions]

## Recommended Next Step
Use `handoff-script` to communicate these authority boundaries to each team member.
```

## Quality Checklist

- [ ] Decision types match code definitions: Type 1 = One-Way Door, Type 2 = Two-Way Door
- [ ] Categories match code: financial, client, team, operational
- [ ] 3-Question Bypass applied to borderline decisions
- [ ] More decisions classified as Type 2 than Type 1 (most operational decisions are reversible)
- [ ] Quick reference is simple enough to pin on a wall
- [ ] Tone empowers the team — this is about freedom, not restriction

## Example

**Input:** "My team always asks me before responding to client questions, changing project timelines, approving expenses, and hiring contractors."

**Output (excerpt):**
```
## Type 2 Decisions — Team Can Decide
| Decision | Category | Assigned To | Authority Level |
|----------|----------|-------------|----------------|
| Routine client questions | Client | Sarah (PM) | Level 3 — Decide & Inform |
| Timeline shifts under 3 days | Client | Sarah (PM) | Level 3 — Decide & Inform |
| Expenses under $200 | Financial | Marcus (VA) | Level 3 — Decide & Inform |

## Type 1 Decisions — Founder Required
| Decision | Category | Why Type 1 |
|----------|----------|-----------|
| Hiring contractors | Team | Irreversible commitment, impacts budget and culture |
| Timeline shifts over 1 week | Client | May affect scope and revenue |

## Bypass Upgrades
| Decision | Original | Result | New |
|----------|----------|--------|-----|
| Expenses $200-$500 | Type 1 | 3/3 favor upgrade (team has budget, reversible, can test) | Type 2 — Decide & Inform |
```

## Related Skills

- `authority-ladder` -> `70-percent-rule` -> this skill -> `handoff-script`
- Decision classifications feed into `accountability-matrix`
- Bypassed decisions should be reviewed after 30 days to confirm the upgrade
- **Entry point:** `_router` — Start here if unsure which skill you need
