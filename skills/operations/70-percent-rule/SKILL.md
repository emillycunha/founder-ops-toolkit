---
name: 70-percent-rule
description: Evaluate if a task is ready to delegate using the 70% Rule. Use when hearing "70%," "good enough," "can they do this," "should I delegate," or "ready to hand off."
---

# 70% Rule

## What This Does

Evaluates whether a specific task or responsibility is ready to delegate by applying the 70% Rule: if someone can do the task at 70% of the founder's quality, delegate it. The time the founder saves is worth more than the 30% quality gap.

## Framework Phase

**ASSIGN** — The 70% Rule is the second mini-framework in the Assign phase. It breaks through the perfectionism that keeps founders doing everything themselves.

**Context:** `/context/operations-reset-framework.md`

**Code source of truth:** `src/lib/authority-transfer/types.ts` — `Readiness` type (ready, developing, not-ready)

## Before Starting

Gather this context:

- The specific task being evaluated for delegation
- Who would receive it (team member name and role)
- The founder's current time investment in this task
- What "quality" means for this task — what does good look like?

## The 70% Rule Explained

**The Math of Delegation:**

A founder doing a task at 100% quality but spending 5 hours/week on it is LESS valuable than a team member doing it at 70% quality while the founder spends those 5 hours on strategic work.

```
Founder doing it:     100% quality x 0 hrs freed = 0 strategic hours gained
Team member doing it: 70% quality  x 5 hrs freed = 5 strategic hours gained
```

The 30% quality gap almost always closes over time as the team member improves. The strategic hours are recovered immediately.

**When the 70% Rule Does NOT Apply:**
- Irreversible decisions with high financial stakes
- Tasks where "70%" means client harm or legal risk
- Relationship-dependent work where the founder IS the value
- One-time strategic decisions (no point delegating what won't recur)

## The Evaluation Questions

For each task, assess these five dimensions:

### 1. Can they produce an acceptable result?
Not perfect — acceptable. Could a reasonable client/customer tell the difference?
- **Yes:** Delegation candidate
- **With training:** Delegation candidate after SOP creation
- **No:** Keep for now

### 2. What's the cost of imperfection?
If the team member does it at 70%, what's the actual consequence?
- **Nothing meaningful:** Delegate immediately
- **Minor rework needed:** Delegate with review period
- **Significant business impact:** Keep or delegate at Level 2 (Recommend)

### 3. Will quality improve with practice?
Most tasks improve with repetition. The first attempt is the worst it'll ever be.
- **Yes, naturally:** Delegate and let them learn
- **Yes, with feedback:** Delegate with structured check-ins
- **No, it requires founder instinct:** Keep — this is CEO Zone work

### 4. What's the founder's time worth?
Calculate the opportunity cost:
- Hours/week currently spent on this task
- What the founder could do instead (revenue-generating, strategic, growth)
- Is the founder's time better used elsewhere?

### 5. Is the blocker skill or permission?
- **Skill gap:** Create an SOP, provide training (fixable)
- **Permission gap:** Grant explicit authority (fixable immediately)
- **Trust gap:** Start with smaller scope, build confidence (fixable over time)

## Readiness Assessment (must match code)

Based on the evaluation, classify readiness:

| Readiness | Criteria | Action |
|-----------|----------|--------|
| **Ready** | Can do it at 70%+ now, consequences of imperfection are manageable | Delegate immediately |
| **Developing** | Could reach 70% with training or SOP support | Create SOP, then delegate |
| **Not Ready** | Significant gap exists, high stakes, or task is genuinely CEO-level | Keep — reassess in 30 days |

## Process

1. Name the specific task being evaluated
2. Identify the potential delegate (team member)
3. Ask the 5 Evaluation Questions
4. Assess readiness: Ready, Developing, or Not Ready
5. If Developing, identify the specific gap and fix
6. Calculate the time reclaimed if delegated
7. Make the delegation recommendation

## Output Format

```
# 70% Rule Evaluation — [Task Name]

## Assessment
- **Task:** [Specific task]
- **Current Owner:** [Founder]
- **Proposed Delegate:** [Team Member]
- **Current Time Investment:** [X hrs/week]

## Evaluation
| Question | Assessment |
|----------|-----------|
| Can they produce acceptable results? | [Yes/With training/No] |
| Cost of imperfection? | [Nothing/Minor rework/Significant] |
| Will quality improve? | [Yes naturally/Yes with feedback/No] |
| Founder's time worth more elsewhere? | [Yes/No] |
| Blocker type? | [Skill/Permission/Trust/None] |

## Readiness: [Ready / Developing / Not Ready]

## Recommendation
[Specific recommendation: delegate now, delegate after [action], or keep]

## Time Reclaimed: [X hrs/week]

## If Developing — Gap Closure Plan
- Gap: [What's missing]
- Fix: [Specific action — SOP, training, smaller scope]
- Timeline: [When they'll be ready]
- Use skill: `[recommended skill]`
```

## Quality Checklist

- [ ] All 5 evaluation questions answered honestly
- [ ] "Not Ready" isn't founder perfectionism disguised as standards
- [ ] Time reclaimed calculation is realistic
- [ ] If Developing, gap closure plan is specific and actionable
- [ ] Readiness states match code: ready, developing, not-ready
- [ ] Tone acknowledges that letting go is hard — 70% feels uncomfortable at first

## Example

**Input:** "Should I delegate client proposal writing to my project manager? I spend about 4 hours a week on proposals."

**Output (excerpt):**
```
## Evaluation
| Question | Assessment |
|----------|-----------|
| Can they produce acceptable results? | With training — needs proposal template and pricing guidelines |
| Cost of imperfection? | Minor rework — founder reviews before sending (30 min) |
| Will quality improve? | Yes with feedback — after 5 proposals, quality will be 85%+ |
| Founder's time worth more elsewhere? | Yes — 4 hrs/week could be 2 new client conversations |
| Blocker type? | Skill — no proposal SOP exists |

## Readiness: Developing

## Recommendation
Delegate after creating a proposal SOP and pricing guide. First 5 proposals get founder review before sending. After 5 successful proposals, move to Decide & Inform (Level 3).

## Time Reclaimed: 3.5 hrs/week (4 hrs minus 30 min review)
```

## Related Skills

- `authority-ladder` -> this skill -> `decision-filter`
- Gap closure often requires `sop-generator`
- Delegation execution uses `handoff-script`
- **Entry point:** `_router` — Start here if unsure which skill you need
