---
name: accountability-matrix
description: Define who owns what using a RACI-style framework. Use when hearing "accountability," "who owns this," "RACI," "ownership," "who's responsible," or "things fall through the cracks."
---

# Accountability Matrix

## What This Does

Creates a clear ownership map for every key business function using a simplified RACI framework (Responsible, Accountable, Consulted, Informed). Eliminates the "I thought you were handling that" problem.

## Framework Phase

**ASSIGN** — The Accountability Matrix is the structural output of the Assign phase. It makes invisible ownership visible and ensures nothing falls through the cracks.

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context:

- Team members and their roles
- Key business functions or areas of responsibility
- Authority levels already assigned (from `authority-ladder`)
- Areas where ownership is currently unclear or duplicated

## RACI Simplified for Small Teams

### The Four Roles

| Role | Symbol | Meaning | Rule |
|------|--------|---------|------|
| **Responsible** | R | Does the work | At least one R per function. Can be multiple people. |
| **Accountable** | A | Owns the outcome. The buck stops here. | Exactly one A per function. Never more than one. |
| **Consulted** | C | Provides input before a decision is made | Ask them first. Their expertise matters. |
| **Informed** | I | Told about the outcome after the fact | Keep them in the loop. No input needed. |

### Key Rules

1. **Every function has exactly ONE "A"** — If everyone is accountable, nobody is accountable.
2. **The "A" can also be the "R"** — Common in small teams where the person doing the work also owns the outcome.
3. **Fewer Cs is better** — Too many "Consulted" roles slow decisions down. Only include people whose input genuinely changes the outcome.
4. **The founder should be "I" for as many functions as possible** — That's the goal of the Operations Reset.

### Common Business Functions for Service Businesses

| Function | Description |
|----------|-------------|
| Lead Generation | Getting potential clients into the pipeline |
| Sales / Closing | Converting leads to clients |
| Client Onboarding | Setting up new clients for success |
| Service Delivery | Doing the actual client work |
| Client Communication | Ongoing updates and relationship management |
| Quality Assurance | Ensuring deliverables meet standards |
| Invoicing & Collections | Getting paid |
| Financial Management | Budgets, expenses, forecasting |
| Team Management | Schedules, performance, development |
| Content / Marketing | Creating visibility for the business |
| Operations / Tools | Managing systems and processes |
| Strategic Planning | Business direction and growth |

## Process

1. List all team members
2. Identify key business functions (use the common list above as a starting point)
3. For each function, assign R, A, C, and I to each team member
4. Verify: Every function has exactly one A
5. Verify: The founder is A for as few functions as possible (Strategic Planning is usually the only one)
6. Identify gaps — functions with no clear owner
7. Identify overloads — one person with too many A's
8. Produce the matrix

## Output Format

```
# Accountability Matrix — [Business Name]

## Team
| Name | Role |
|------|------|
| [Name] | [Role] |

## RACI Matrix
| Function | [Founder] | [Team Member 1] | [Team Member 2] |
|----------|-----------|-----------------|-----------------|
| Lead Generation | [R/A/C/I] | [R/A/C/I] | [R/A/C/I] |
| Sales / Closing | [R/A/C/I] | [R/A/C/I] | [R/A/C/I] |
| Client Onboarding | [R/A/C/I] | [R/A/C/I] | [R/A/C/I] |
| Service Delivery | [R/A/C/I] | [R/A/C/I] | [R/A/C/I] |
| Client Communication | [R/A/C/I] | [R/A/C/I] | [R/A/C/I] |
| Quality Assurance | [R/A/C/I] | [R/A/C/I] | [R/A/C/I] |
| Invoicing | [R/A/C/I] | [R/A/C/I] | [R/A/C/I] |
| Financial Management | [R/A/C/I] | [R/A/C/I] | [R/A/C/I] |
| Team Management | [R/A/C/I] | [R/A/C/I] | [R/A/C/I] |
| Content / Marketing | [R/A/C/I] | [R/A/C/I] | [R/A/C/I] |
| Operations / Tools | [R/A/C/I] | [R/A/C/I] | [R/A/C/I] |
| Strategic Planning | [R/A/C/I] | [R/A/C/I] | [R/A/C/I] |

## Ownership Summary
- Founder is Accountable for: [X] of [Y] functions
- [Team Member 1] is Accountable for: [X] of [Y] functions
- Functions with no clear Accountable: [list or "None"]

## Gaps & Overloads
- **Gaps:** [Functions without clear ownership]
- **Overloads:** [People with too many A's — typically the founder]

## Action Items
1. [Specific change to make]
2. [Specific change to make]
```

## Quality Checklist

- [ ] Every function has exactly ONE person as Accountable (A)
- [ ] Founder is NOT Accountable for most functions — Strategic Planning is usually the only one
- [ ] No team member has more A's than they can genuinely own
- [ ] "Consulted" roles are minimal — only where input changes outcomes
- [ ] Gaps identified — no function left unowned
- [ ] Matrix is simple enough to reference weekly

## Example

**Input:** "Me (founder), Sarah (PM), Marcus (VA). I do most things but Sarah runs projects and Marcus does admin."

**Output (excerpt):**
```
## RACI Matrix
| Function | Founder | Sarah (PM) | Marcus (VA) |
|----------|---------|-----------|-------------|
| Lead Generation | A, R | I | R |
| Sales / Closing | A, R | C | I |
| Client Onboarding | C | A, R | R |
| Service Delivery | C | A, R | I |
| Client Communication | I | A, R | R |
| Invoicing | I | C | A, R |
| Strategic Planning | A, R | C | I |

## Ownership Summary
- Founder is Accountable for: 3 of 12 functions (Lead Gen, Sales, Strategy)
- Sarah is Accountable for: 5 of 12 functions
- Marcus is Accountable for: 4 of 12 functions
```

## Related Skills

- `authority-ladder` -> `decision-filter` -> `handoff-script` -> this skill
- Accountability gaps feed back into `authority-ladder` for level assignment
- Review monthly alongside `team-autonomy-score`
- **Entry point:** `_router` — Start here if unsure which skill you need
