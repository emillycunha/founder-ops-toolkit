---
name: client-onboarding
description: Build client onboarding workflows. Use when hearing "onboarding," "new client," "kickoff process," "client welcome," or "first 30 days."
---

# Client Onboarding

## What This Does

Creates a structured client onboarding workflow that delivers a consistent, professional first experience without requiring the founder to run every step. This is one of the highest-impact processes to systemize.

## Framework Phase

**Cross-Phase** — Client onboarding touches all three phases: documenting the process (EXTRACT), delegating steps to the team (ASSIGN), and installing a repeatable cadence (SCALE).

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context:

- What happens today when a new client signs (even if it's ad hoc)
- What information is needed from the client
- What deliverables or setup needs to happen before work begins
- What the client's ideal first experience would feel like
- Common onboarding problems (delays, confusion, missed steps)

## The 5 Onboarding Phases

### Phase 1: Pre-Welcome (Before kickoff)
Trigger: Contract signed and deposit received

- Send welcome email (templates + next steps)
- Collect client intake information (questionnaire or form)
- Set up internal project folder and tracking
- Schedule kickoff call
- Prepare kickoff materials

**Owner:** Can be delegated to VA or PM after SOP exists

### Phase 2: Kickoff (Day 1)
Trigger: Kickoff call or first meeting

- Introduce the team (who does what)
- Review project scope, timeline, and expectations
- Walk through communication preferences and tools
- Confirm key milestones and deliverables
- Answer client questions

**Owner:** Founder for high-value clients, PM for standard clients

### Phase 3: Setup (Days 1-5)
Trigger: After kickoff

- Grant client access to shared tools/platforms
- Assign internal team roles for this project
- Create project timeline/milestones
- Begin initial deliverables
- Send first status update

**Owner:** PM or team lead

### Phase 4: First Win (Days 5-14)
Trigger: First deliverable ready

- Deliver first tangible output or milestone
- Collect feedback on the deliverable AND the process
- Adjust approach based on feedback
- Reinforce communication cadence

**Owner:** Whoever is responsible for delivery

### Phase 5: Steady State (Days 14-30)
Trigger: Onboarding complete, transition to ongoing work

- Confirm regular check-in schedule
- Ensure client knows who to contact for what
- Founder steps back (if involved in kickoff)
- Add client to regular reporting cadence

**Owner:** PM or account manager

## Process

1. Map the current onboarding process (even if informal)
2. Organize steps into the 5 phases
3. For each phase, define: steps, owner, timeline, tools
4. Create templates for each phase (welcome email, intake form, kickoff agenda)
5. Identify which steps the founder must do vs. can delegate
6. Build the SOP using `sop-generator`
7. Produce the onboarding workflow

## Output Format

```
# Client Onboarding Workflow — [Business Name]

## Overview
- Total onboarding duration: [X days]
- Phases: 5 (Pre-Welcome → Kickoff → Setup → First Win → Steady State)
- Founder involvement required in: [X of 5 phases]

## Phase Checklist

### Phase 1: Pre-Welcome (Days -3 to 0)
- [ ] Send welcome email — Owner: [Name] — Template: [location]
- [ ] Send intake questionnaire — Owner: [Name] — Tool: [tool]
- [ ] Create project folder — Owner: [Name] — Template: [location]
- [ ] Schedule kickoff call — Owner: [Name]
- [ ] Prepare kickoff deck — Owner: [Name] — Template: [location]

### Phase 2: Kickoff (Day 1)
- [ ] Run kickoff call — Owner: [Name] — Agenda: [location]
- [ ] Confirm scope and timeline — Owner: [Name]
- [ ] Introduce team members — Owner: [Name]
- [ ] Set communication expectations — Owner: [Name]

### Phase 3: Setup (Days 1-5)
...

### Phase 4: First Win (Days 5-14)
...

### Phase 5: Steady State (Days 14-30)
...

## Templates Needed
| Template | Status | Location |
|----------|--------|----------|
| Welcome email | [Exists/Needs creation] | [Location] |
| Intake questionnaire | [Exists/Needs creation] | [Location] |
| Kickoff agenda | [Exists/Needs creation] | [Location] |

## Recommended Next Step
Use `sop-generator` to create the full SOP for each phase. Use `handoff-script` to delegate phases to team members.
```

## Quality Checklist

- [ ] All 5 phases covered with specific steps
- [ ] Every step has a clear owner
- [ ] Templates identified (and creation plan if they don't exist)
- [ ] Founder involvement minimized — only where genuinely needed
- [ ] Client experience feels warm and professional (brand voice applies here)
- [ ] First Win happens within 14 days — early momentum matters
- [ ] Transition to Steady State is explicit — onboarding has a clear end

## Example

**Input:** "I personally handle every new client. I send them an email, schedule a call, set up their project, and do the first deliverable. It takes me 6 hours per new client."

**Output (excerpt):**
```
## Overview
- Current: 6 hours founder time per client
- After systemization: 1.5 hours founder time (kickoff call only)
- Time saved: 4.5 hours per new client

### Phase 1: Pre-Welcome
- [ ] Send welcome email — Owner: VA (Marcus) — Template: Google Drive > Templates
- [ ] Send intake questionnaire — Owner: VA (Marcus) — Tool: Google Forms
- [ ] Create project folder — Owner: VA (Marcus) — Template: Drive template
- [ ] Schedule kickoff call — Owner: VA (Marcus) — Tool: Calendly

### Phase 2: Kickoff
- [ ] Run kickoff call — Owner: Founder — Agenda: Drive > Templates > Kickoff
```

## Related Skills

- `process-mapper` -> this skill -> `sop-generator` -> `handoff-script`
- Onboarding metrics feed into `scorecard-builder`
- Common onboarding process to systemize with `hire-vs-systemize`
- **Entry point:** `_router` — Start here if unsure which skill you need
