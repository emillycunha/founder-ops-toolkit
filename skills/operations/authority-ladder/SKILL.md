---
name: authority-ladder
description: Define 5 levels of delegation authority. Use when hearing "delegation levels," "who decides," "authority," "how much can they decide," or "permission to act."
---

# Authority Ladder

## What This Does

Defines five escalating levels of decision-making authority and assigns each team member to the appropriate level for each business function. This creates clarity about what the team can decide without the founder.

## Framework Phase

**ASSIGN** — The Authority Ladder is the first mini-framework in the Assign phase. It replaces the vague "just handle it" with specific, graduated authority levels.

**Context:** `/context/operations-reset-framework.md`

**Code source of truth:** `src/lib/authority-transfer/types.ts` — `AuthorityLevel` type (1-5)

## Before Starting

Gather this context:

- Team member names and roles
- Current decision-making patterns (who decides what today)
- Areas where the founder is most frequently consulted
- Previous delegation failures or trust issues (if any)

## The 5 Authority Levels (must match code)

| Level | Name | What It Means | Founder Involvement |
|-------|------|--------------|---------------------|
| **1** | **Research Only** | Gather information and present options. No action taken. | Founder decides everything |
| **2** | **Recommend** | Research + recommend a path. Founder still approves. | Founder approves before action |
| **3** | **Decide & Inform** | Make the decision, then tell the founder what you did. | Founder is informed after the fact |
| **4** | **Full Autonomy** | Make the decision. No need to inform unless it's notable. | Founder is not involved |
| **5** | **Train Others** | Own the decision AND teach others how to make it. | Founder has fully transferred this |

### How to Assign Levels

Use these criteria to determine the right level:

**Level 1 — Research Only** when:
- Team member is new to this area
- The stakes are high and irreversible
- Founder needs to build confidence in the team member's judgment

**Level 2 — Recommend** when:
- Team member understands the domain
- Decisions have moderate stakes
- Founder wants visibility but not control

**Level 3 — Decide & Inform** when:
- Team member has proven judgment in this area
- Decisions are reversible (Type 2)
- Speed matters more than founder oversight

**Level 4 — Full Autonomy** when:
- Team member consistently makes good decisions here
- The domain is well-defined with clear guardrails
- Founder involvement adds no value

**Level 5 — Train Others** when:
- Team member is the expert in this area
- They can transfer their knowledge to new team members
- The founder has fully let go of this domain

## Readiness States (from code)

Before assigning authority levels, assess each team member's readiness:

| State | Meaning | Action |
|-------|---------|--------|
| **Ready** | Can take on this authority level now | Assign and communicate |
| **Developing** | Needs some support or training first | Create a development plan |
| **Not Ready** | Significant gap exists | Start at a lower level |

### Common Blockers (from code)

When a team member isn't ready, identify the blocker:

| Blocker | Description | Fix |
|---------|-------------|-----|
| **Training** | Lacks the knowledge or skill | Provide training or SOP |
| **Authority** | Has the skill but hasn't been given permission | Explicitly grant authority |
| **Confidence** | Has skill and permission but second-guesses themselves | Start small, build wins |
| **Letting Go** | The blocker is the founder, not the team member | Founder needs to release control |

## Process

1. List all team members with their roles
2. Identify the key decision areas (client, financial, team, operational)
3. For each team member + decision area, assess readiness (Ready, Developing, Not Ready)
4. Assign an authority level (1-5) based on readiness and decision stakes
5. Identify blockers for any "Developing" or "Not Ready" assessments
6. Create the Authority Matrix
7. Communicate levels clearly to each team member

## Output Format

```
# Authority Ladder — [Business Name]

## Team Overview
| Member | Role | Overall Readiness |
|--------|------|------------------|
| [Name] | [Role] | [Ready/Developing/Not Ready] |

## Authority Matrix
| Decision Area | [Team Member 1] | [Team Member 2] | [Team Member 3] |
|--------------|-----------------|-----------------|-----------------|
| Client Communication | Level [X] | Level [X] | Level [X] |
| Financial (under $[X]) | Level [X] | Level [X] | Level [X] |
| Team Scheduling | Level [X] | Level [X] | Level [X] |
| Project Scope Changes | Level [X] | Level [X] | Level [X] |
| Vendor/Tool Decisions | Level [X] | Level [X] | Level [X] |

## Blockers to Address
| Member | Area | Current Level | Target Level | Blocker | Fix |
|--------|------|--------------|-------------|---------|-----|
| [Name] | [Area] | [X] | [X] | [Type] | [Action] |

## Escalation Rules
- Level 1-2 decisions: Always check with [Founder Name] before acting
- Level 3 decisions: Act first, notify [Founder Name] within 24 hours
- Level 4-5 decisions: No notification needed unless exceptional

## Recommended Next Step
Use `70-percent-rule` to evaluate delegation readiness for specific tasks, then `decision-filter` to classify decision types.
```

## Quality Checklist

- [ ] All 5 levels used — not just Level 1 and Level 4
- [ ] Authority levels match code definitions exactly
- [ ] Readiness honestly assessed — not aspirational
- [ ] Blockers identified with specific fixes, not vague "needs development"
- [ ] Escalation rules are clear and simple
- [ ] "Letting go" blocker honestly evaluated — is the founder the real barrier?
- [ ] Tone is empowering — this is about trust, not control

## Example

**Input:** "I have a project manager (Sarah) and a VA (Marcus). Sarah handles client projects, Marcus handles admin. I approve everything."

**Output (excerpt):**
```
## Authority Matrix
| Decision Area | Sarah (PM) | Marcus (VA) |
|--------------|-----------|-------------|
| Client Communication | Level 3 — Decide & Inform | Level 2 — Recommend |
| Financial (under $500) | Level 2 — Recommend | Level 1 — Research Only |
| Project Timeline | Level 3 — Decide & Inform | Level 1 — Research Only |
| Social Media Posts | Level 4 — Full Autonomy | Level 3 — Decide & Inform |
| Vendor Selection | Level 2 — Recommend | Level 1 — Research Only |

## Blockers to Address
| Member | Area | Current | Target | Blocker | Fix |
|--------|------|---------|--------|---------|-----|
| Sarah | Financial | Level 2 | Level 3 | Letting Go | Founder needs to set a $500 threshold and let Sarah decide below it |
| Marcus | Client Comms | Level 2 | Level 3 | Training | Create client communication SOP and templates |
```

## Related Skills

- This skill -> `70-percent-rule` -> `decision-filter` -> `handoff-script`
- Authority assignments inform `accountability-matrix`
- Blocker fixes may require `sop-generator` (training) or `brain-dump` (letting go)
- **Entry point:** `_router` — Start here if unsure which skill you need
