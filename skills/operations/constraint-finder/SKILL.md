---
name: constraint-finder
description: Identify single biggest bottleneck to fix. Use when hearing "constraint," "what's slowing us," "biggest problem," "where do I start," or "one thing to fix."
---

# Constraint Finder

## What This Does

Applies the Theory of Constraints to identify the single most impactful bottleneck limiting business growth, then creates a focused action plan to address it. Unlike `bottleneck-finder` which diagnoses all bottlenecks, this skill finds THE ONE constraint that matters most right now.

## Framework Phase

**EXTRACT** (Cross-phase application) — Constraint identification can surface issues in any phase (Extract, Assign, or Scale), but the diagnostic method is an extraction exercise.

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context:

- What is the founder's primary business goal right now?
- Where does growth feel stuck?
- Bottleneck Finder results (if available)
- What has the founder already tried to fix?

## The Theory of Constraints (Simplified)

A system can only move as fast as its slowest part. In a founder-led business, the constraint is almost always the founder themselves — but the specific way they're the constraint matters.

### The 5 Types of Founder Constraints

| Type | The Constraint Is... | Looks Like |
|------|---------------------|------------|
| **Knowledge** | Information locked in the founder's head | Team can't act because they don't know what to do |
| **Authority** | Decision power concentrated in the founder | Team knows what to do but waits for permission |
| **Capacity** | Founder's time is maxed out | Pipeline of work waiting for founder's hands |
| **Process** | No system exists to handle repeating work | Same problems keep recurring, solved ad hoc each time |
| **Rhythm** | No predictable cadence for operations | Business moves in spurts — no steady momentum |

### Mapping Constraints to Framework Phases

| Constraint Type | Framework Phase | Primary Fix |
|----------------|----------------|-------------|
| Knowledge | EXTRACT | Document and transfer knowledge |
| Authority | ASSIGN | Define decision boundaries and delegate |
| Capacity | EXTRACT then ASSIGN | Extract tasks, then assign ownership |
| Process | EXTRACT | Build systems and SOPs |
| Rhythm | SCALE | Install operating cadence |

## The 5 Focusing Steps

Once the constraint is identified, follow this sequence:

### 1. Identify
Name the single constraint that limits throughput the most. Be specific — not "I'm the bottleneck" but "I'm the only person who can approve proposals, and proposals wait an average of 3 days for my review."

### 2. Exploit
Get maximum output from the constraint without changing anything else. If the founder is the constraint, this means protecting their time on the constraint work and removing distractions.

### 3. Subordinate
Align everything else to support the constraint. Other processes should feed the constraint smoothly, not pile up. If founder approval is the constraint, make approvals the first thing they do each day.

### 4. Elevate
Invest in removing the constraint permanently. This usually means: document it, delegate it, or build a system for it.

### 5. Repeat
Once the constraint is resolved, a new one emerges. Go back to Step 1 with the next constraint.

## Process

1. Understand the founder's primary growth goal
2. Ask: "What's the one thing that, if fixed, would unlock the most progress?"
3. If unclear, use the 5 Types to narrow down (Knowledge, Authority, Capacity, Process, Rhythm)
4. Validate the constraint: Is this truly the bottleneck, or a symptom of something deeper?
5. Name the constraint specifically (not generally)
6. Apply the 5 Focusing Steps
7. Map to the correct framework phase
8. Produce a focused action plan

## Output Format

```
# Constraint Analysis — [Founder Name]

## The One Constraint
**[Specific constraint statement]**

- Type: [Knowledge / Authority / Capacity / Process / Rhythm]
- Framework Phase: [EXTRACT / ASSIGN / SCALE]
- Impact: [What this constraint is costing — time, revenue, growth, sanity]

## The 5-Step Plan

### 1. Identify (Confirmed)
[The specific constraint, stated clearly]

### 2. Exploit (This Week)
[What to do immediately to get more from the constraint without changing it]

### 3. Subordinate (Next 2 Weeks)
[How to reorganize other work to support the constraint]

### 4. Elevate (Next 30 Days)
[The permanent fix — document, delegate, or systematize]
- Use skill: `[recommended skill]`

### 5. Repeat
Once resolved, the next likely constraint is: [prediction based on analysis]

## Recommended Next Step
[Specific skill to use for the Elevate step]
```

## Quality Checklist

- [ ] Single constraint identified — not a list of three
- [ ] Constraint is specific, not vague ("proposal approvals take 3 days" not "I'm too busy")
- [ ] Constraint type accurately classified
- [ ] 5 Focusing Steps are practical, not theoretical
- [ ] Elevate step includes a specific skill recommendation
- [ ] Framework phase mapping is accurate
- [ ] Tone is focused and encouraging — this is about clarity, not overwhelm

## Example

**Input:** "I want to grow from 5 to 10 clients but every time I try, things fall apart. I can't seem to scale past where I am."

**Output (excerpt):**
```
## The One Constraint
Your client onboarding process requires 6+ hours of your personal time per new client, and nothing is documented. Adding clients doesn't just add revenue — it adds founder hours at a 1:1 ratio.

- Type: Process
- Framework Phase: EXTRACT
- Impact: Capacity ceiling — you literally cannot serve more than 5 clients at your current involvement level

### 2. Exploit (This Week)
Block onboarding into two dedicated half-days. Don't let it bleed into other work. Batch the next 2 onboardings together.

### 4. Elevate (Next 30 Days)
Document the onboarding process using `process-mapper`, then create an SOP with `sop-generator`. Goal: reduce your onboarding time from 6 hours to 1 hour by having your team handle Steps 2-8.
```

## Related Skills

- `bottleneck-finder` -> this skill (for deeper single-constraint focus)
- Routes to: `sop-generator` (Process), `authority-ladder` (Authority), `weekly-rhythm` (Rhythm), `brain-dump` (Knowledge)
- After resolving, rerun to find the next constraint
- **Entry point:** `_router` — Start here if unsure which skill you need
