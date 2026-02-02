---
name: ops-health-check
description: Score overall operational maturity across all 3 framework phases. Use when hearing "ops health," "operations audit," "how are we doing," "operational maturity," or "where should I focus."
---

# Ops Health Check

## What This Does

Scores operational maturity across all three phases of the Operations Reset Framework (Extract, Assign, Scale), identifies the weakest phase, and recommends where to focus first. This is the comprehensive diagnostic that tells founders where they stand.

## Framework Phase

**Cross-Phase** — The Ops Health Check spans all three phases and serves as the starting point for founders who aren't sure where to begin.

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context:

- General understanding of the business (size, team, revenue range)
- Willingness to answer honestly — this assessment only helps if it's truthful
- No prior tool results needed — this is designed to work standalone

## The Three-Phase Assessment

### Phase 1: EXTRACT — Is the system visible?

Score each question 1-5 (1 = Not at all, 5 = Completely):

1. **Documentation:** What percentage of your recurring processes are documented?
2. **Visibility:** Can your team find answers without asking you?
3. **Knowledge transfer:** If you were gone for a month, how much tribal knowledge would be lost?
4. **Task clarity:** Does your team know exactly what to do each day without your direction?

**Phase Score: Average of 4 questions (1-5)**

### Phase 2: ASSIGN — Does the team own outcomes?

Score each question 1-5:

1. **Decision authority:** Can your team make most daily decisions without checking with you?
2. **Ownership:** Does your team own outcomes (not just tasks)?
3. **Delegation:** Have you successfully delegated work that used to be yours?
4. **Accountability:** Is there a clear owner for every key business function?

**Phase Score: Average of 4 questions (1-5)**

### Phase 3: SCALE — Does the business run predictably?

Score each question 1-5:

1. **Weekly rhythm:** Do you have a predictable operating cadence?
2. **Metrics:** Do you track KPIs that tell you if things are on track?
3. **Consistency:** Does the business perform similarly week to week (not in bursts)?
4. **Sustainability:** Could you maintain this pace for 5 more years?

**Phase Score: Average of 4 questions (1-5)**

## Scoring and Interpretation

### Overall Score
Average of all three phase scores (1-5)

| Score | Maturity Level | Description |
|-------|---------------|-------------|
| 1.0-2.0 | **Founder-Dependent** | Business runs on the founder's energy and memory. No systems, no delegation, no rhythm. |
| 2.1-3.0 | **Early Systems** | Some documentation exists, some delegation attempted. Inconsistent. Still heavily founder-reliant. |
| 3.1-4.0 | **Structured** | Real systems in place, team has genuine ownership, operating rhythm exists. Founder can step back for short periods. |
| 4.1-5.0 | **Independent** | Business runs without the founder for weeks. Strong systems, clear ownership, predictable operations. |

### Phase Priority

The lowest-scoring phase is where to focus:

| Lowest Phase | Priority | Start With |
|-------------|----------|-----------|
| EXTRACT | Get systems out of your head first | `brain-dump` -> `task-categorizer` -> `waterline-audit` |
| ASSIGN | Give your team real ownership | `authority-ladder` -> `70-percent-rule` -> `decision-filter` |
| SCALE | Install predictable rhythm | `outcome-shifter` -> `weekly-rhythm` -> `scorecard-builder` |

## Process

1. Walk through the 12 questions (4 per phase)
2. Score each 1-5
3. Calculate phase averages
4. Calculate overall average
5. Determine maturity level
6. Identify the lowest-scoring phase
7. Recommend the starting skill pipeline for that phase

## Output Format

```
# Ops Health Check — [Business Name]

## Overall Score: [X]/5 — [Maturity Level]

## Phase Scores
| Phase | Score | Status |
|-------|-------|--------|
| EXTRACT (Systems visible?) | [X]/5 | [Strongest/Middle/Weakest] |
| ASSIGN (Team owns outcomes?) | [X]/5 | [Strongest/Middle/Weakest] |
| SCALE (Business runs predictably?) | [X]/5 | [Strongest/Middle/Weakest] |

## Detailed Breakdown
### EXTRACT — [X]/5
| Question | Score | Observation |
|----------|-------|-------------|
| Documentation | [1-5] | [Brief note] |
| Visibility | [1-5] | [Brief note] |
| Knowledge transfer | [1-5] | [Brief note] |
| Task clarity | [1-5] | [Brief note] |

### ASSIGN — [X]/5
...

### SCALE — [X]/5
...

## Priority: Start with [EXTRACT / ASSIGN / SCALE]
[Why this phase is the priority and what it's costing the business]

## Recommended First Steps
1. [Skill] — [Why]
2. [Skill] — [Why]
3. [Skill] — [Why]
```

## Quality Checklist

- [ ] All 12 questions scored honestly — not aspirationally
- [ ] Phase averages calculated correctly
- [ ] Maturity level matches the score range
- [ ] Weakest phase identified with specific observations
- [ ] Recommended skills match the weakest phase pipeline
- [ ] Tone is encouraging — this is a starting point, not a report card

## Example

**Input:** A service-based consultant with 2 team members, no SOPs, partial delegation, and no weekly rhythm.

**Output (excerpt):**
```
## Overall Score: 2.1/5 — Early Systems

## Phase Scores
| Phase | Score | Status |
|-------|-------|--------|
| EXTRACT | 1.5/5 | Weakest |
| ASSIGN | 2.5/5 | Middle |
| SCALE | 2.3/5 | Middle |

## Priority: Start with EXTRACT
Almost nothing is documented. Your team has some delegation but they're working from verbal instructions and memory. Until systems are visible, delegation will be fragile and scaling will be impossible.

## Recommended First Steps
1. `brain-dump` — Get everything out of your head into a master task list
2. `task-categorizer` — Sort tasks into the 4-Box Map to identify Quick Wins
3. `waterline-audit` — Draw the line between CEO work and systemizable work
```

## Related Skills

- This skill routes to the weakest phase pipeline:
  - EXTRACT: `brain-dump` -> `task-categorizer` -> `waterline-audit`
  - ASSIGN: `authority-ladder` -> `70-percent-rule` -> `decision-filter`
  - SCALE: `outcome-shifter` -> `weekly-rhythm` -> `scorecard-builder`
- Rerun quarterly to track progress
- **Entry point:** `_router` — Start here if unsure which skill you need
