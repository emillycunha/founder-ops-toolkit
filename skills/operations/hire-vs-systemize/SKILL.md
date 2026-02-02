---
name: hire-vs-systemize
description: Decide whether to hire or build a system. Use when hearing "should I hire," "hire or automate," "need help," "bring someone on," or "build a system for this."
---

# Hire vs. Systemize

## What This Does

Provides a structured decision framework for determining whether a business need is best solved by hiring a person, building a system/process, or combining both. Prevents the common mistake of hiring before systems exist.

## Framework Phase

**ASSIGN** (Cross-phase application) — This decision often arises during the Assign phase when founders realize they need help, but the answer isn't always "hire someone."

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context:

- What specific problem or need is driving the hire/system question
- Current team size and capacity
- Whether the work is documented (SOPs exist)
- Budget constraints
- Urgency of the need

## The Decision Framework

### The Core Question

Before asking "should I hire?", ask: **"Does a system for this exist yet?"**

If no system exists, hiring someone to do undocumented work means the founder will spend MORE time managing the new hire than doing the work themselves. The Operations Reset Framework says: **Extract first, then Assign.**

### The Four Quadrants

| | System Exists | No System |
|---|---|---|
| **High Judgment** | Hire (they can follow the system AND apply judgment) | Extract first — document the process, then hire |
| **Low Judgment** | Systemize further (automate or use tools) | Extract first — then automate before hiring |

### Decision Criteria

Score each criterion to make the decision:

| Criterion | Hire | Systemize | Score |
|-----------|------|-----------|-------|
| **Frequency** | Happens constantly, needs human flexibility | Happens on a predictable schedule | Hire: +1 / System: +1 |
| **Complexity** | Requires nuanced judgment each time | Follows a repeatable pattern | Hire: +1 / System: +1 |
| **Variability** | Every instance is different | Every instance is similar | Hire: +1 / System: +1 |
| **Relationship** | Requires human connection (clients, partners) | Transactional or internal only | Hire: +1 / System: +1 |
| **Cost** | Person is affordable for the volume | Tool/automation is cheaper than a person | Hire: +1 / System: +1 |
| **Speed to Implement** | Can hire and onboard quickly | System takes time to build | Hire: +1 / System: +1 |

**Total: 6 points possible**
- 4+ Hire points: Lean toward hiring
- 4+ System points: Lean toward systemizing
- 3-3 split: Build a system, then hire someone to run it

### The Hybrid Option

Often the best answer is: **Build the system first, then hire someone to operate it.**

This means:
1. Document the process (EXTRACT)
2. Build the SOP (EXTRACT)
3. Hire someone to follow the SOP (ASSIGN)
4. Install check-ins and metrics (SCALE)

## Process

1. Define the specific need or problem
2. Check: Does a system/SOP exist for this work?
3. Assess: Is this high-judgment or low-judgment work?
4. Score the 6 decision criteria
5. Determine: Hire, Systemize, or Hybrid
6. If Hire: Define the role and authority level
7. If Systemize: Identify the right tool or automation
8. If Hybrid: Define the extraction sequence first

## Output Format

```
# Hire vs. Systemize — [Need/Role]

## The Need
[What problem or gap is being addressed]

## Current State
- System/SOP exists: [Yes / Partially / No]
- Judgment level: [High / Low]
- Quadrant: [Hire / Systemize / Extract First / Extract Then Automate]

## Decision Criteria
| Criterion | Assessment | Points To |
|-----------|-----------|-----------|
| Frequency | [Assessment] | [Hire/System] |
| Complexity | [Assessment] | [Hire/System] |
| Variability | [Assessment] | [Hire/System] |
| Relationship | [Assessment] | [Hire/System] |
| Cost | [Assessment] | [Hire/System] |
| Speed | [Assessment] | [Hire/System] |

**Score:** Hire [X] / Systemize [X]

## Recommendation: [Hire / Systemize / Hybrid]
[Specific recommendation with reasoning]

## Implementation Plan
### If Hire:
- Role: [Title and key responsibilities]
- Authority Level: [From `authority-ladder`]
- First task: [What they start with]

### If Systemize:
- Tool/automation: [Specific recommendation]
- SOP needed: [Yes/No — use `sop-generator`]

### If Hybrid:
1. First: [Extract — use `process-mapper` and `sop-generator`]
2. Then: [Hire — define the role]
3. Finally: [Scale — install `weekly-rhythm` check-ins]
```

## Quality Checklist

- [ ] "Should I hire?" questioned first — is the real problem a missing system?
- [ ] System/SOP existence checked before recommending a hire
- [ ] All 6 criteria scored honestly
- [ ] Hybrid option considered — it's usually the best answer
- [ ] Cost comparison is realistic (include training/management time for hires)
- [ ] Recommendation includes specific next steps, not just "hire someone"

## Example

**Input:** "I need help with social media. Should I hire a social media manager?"

**Output (excerpt):**
```
## Current State
- System/SOP exists: No — founder posts when they remember, no content calendar, no templates
- Judgment level: Low — social media posting follows repeatable patterns
- Quadrant: Extract First, Then Automate

## Score: Hire 2 / Systemize 4

## Recommendation: Hybrid
Don't hire yet. First:
1. Create a content calendar template and posting SOP using `sop-generator`
2. Set up a scheduling tool (Buffer, Later, or Hootsuite) — this eliminates 60% of the manual work
3. After the system runs for 4 weeks, evaluate: Does the remaining work justify a hire, or can a VA handle it 2 hrs/week?

Estimated savings: $2,000-3,000/month vs. hiring a social media manager, with the same output quality.
```

## Related Skills

- This skill helps decide the path, then routes to:
  - Hire path: `authority-ladder` -> `handoff-script`
  - System path: `process-mapper` -> `sop-generator`
  - Hybrid path: Extract skills first, then Assign skills
- **Entry point:** `_router` — Start here if unsure which skill you need
