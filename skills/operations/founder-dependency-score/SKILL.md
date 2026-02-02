---
name: founder-dependency-score
description: Calculate reliance on founder (0-100). Use when hearing "founder dependency," "bus factor," "what if I left," "how dependent is the business on me," or "could my business run without me."
---

# Founder Dependency Score

## What This Does

Calculates a 0-100 score quantifying how dependent the business is on the founder, places the business into one of four segments, and provides a phase-specific recommendation for reducing dependency.

## Framework Phase

**EXTRACT** — The Founder Dependency Score is the key diagnostic metric of the Extract phase. It quantifies the problem and tracks progress over time.

**Context:** `/context/operations-reset-framework.md`

**Code source of truth:** `src/lib/ops-inventory/scoring.ts` — `calculateFounderScore()`, `getSegment()`, `SEGMENT_INFO`

## Before Starting

Gather this context:

- Honest assessment of current business operations
- Willingness to answer candidly — this score only helps if it's truthful
- Understanding that a high score isn't failure — it's the starting point

## The 10 Chaos Questions

Each question uses a traffic light scoring system:

- **Green (0 points):** Healthy — this isn't a problem
- **Yellow (5 points):** Caution — some dependency exists
- **Red (10 points):** Critical — heavy founder dependency

### The Questions

1. **If you were unreachable for a week, how much of the business would keep running normally?**
   - Green: Most things would continue fine
   - Yellow: Some things would stall, but nothing critical
   - Red: Major parts of the business would stop

2. **How many decisions require your direct approval before the team can act?**
   - Green: Very few — team handles most decisions
   - Yellow: Several daily decisions need my input
   - Red: Almost everything needs my approval

3. **If a new team member started tomorrow, how quickly could they get up to speed?**
   - Green: Clear documentation and onboarding exists
   - Yellow: Some documentation, but mostly learned from me
   - Red: They'd shadow me for weeks — nothing is written down

4. **How often does your team come to you with questions they could answer themselves?**
   - Green: Rarely — they know where to find answers
   - Yellow: A few times a week
   - Red: Multiple times daily

5. **What percentage of client relationships depend on your personal involvement?**
   - Green: Under 20% — team handles most client contact
   - Yellow: 20-60% require some founder involvement
   - Red: Over 60% depend on me personally

6. **How much of your business knowledge exists only in your head?**
   - Green: Most things are documented or shared
   - Yellow: Key processes are documented but details are in my head
   - Red: Almost everything — I am the documentation

7. **When something goes wrong, who fixes it?**
   - Green: Team has clear escalation paths and can resolve most issues
   - Yellow: Team tries but usually needs my help
   - Red: Everything escalates to me

8. **How predictable is your weekly schedule?**
   - Green: I have a consistent rhythm with protected strategic time
   - Yellow: Somewhat predictable but frequently disrupted
   - Red: Every week is different — I'm constantly reacting

9. **Could your team run the business for a month without you?**
   - Green: Yes — they'd handle it well
   - Yellow: They'd manage but some things would slip
   - Red: No — things would fall apart within days

10. **How often do you do work that someone on your team could do at 70% of your quality?**
    - Green: Rarely — I've delegated most of that
    - Yellow: Weekly — some tasks I should let go of
    - Red: Daily — I do things my team could handle

## The Four Segments (must match code)

| Score | Segment | Description |
|-------|---------|-------------|
| **0-25** | **Operational CEO** | You've built solid systems. Your team operates with real autonomy, and you're mostly working ON the business, not IN it. |
| **26-50** | **Bottleneck Builder** | You've got some systems in place, but you're still the approval layer for too many decisions. Your team is capable, but they're waiting on you more than they should. |
| **51-75** | **Single Point of Failure** | Your business has a serious dependency problem — you. Critical knowledge lives in your head, and most decisions require your input. Growth is limited by your capacity. |
| **76-100** | **The Business IS You** | Right now, you don't have a business — you have a job you can't quit. Everything runs through you, and stepping away means everything stops. |

## Segment Recommendations (must match code)

| Segment | Recommendation |
|---------|---------------|
| Operational CEO | Focus on optimizing and scaling what's working. The Ops Inventory can help you identify the remaining 20% that still needs attention. |
| Bottleneck Builder | Time to define clear decision authority. Focus on the ASSIGN phase — give your team explicit permission to act. |
| Single Point of Failure | Start with EXTRACT. Get the systems out of your head and onto paper. Your Brain Dump list is your roadmap. |
| The Business IS You | This is fixable, but it starts with acknowledging the depth of the problem. Your first step is documentation — every process, every decision, everything in your head. |

## Process

1. Present the 10 Chaos Questions one at a time
2. Record Green/Yellow/Red for each (0/5/10 points)
3. Calculate total score (sum of all answers, 0-100)
4. Determine segment based on score range
5. Present the score, segment, and recommendation
6. Identify the highest-scoring questions as priority areas

## Output Format

```
# Founder Dependency Score — [Founder Name]

## Your Score: [X]/100
## Segment: [Segment Name]

[Segment description from SEGMENT_INFO]

## Score Breakdown
| # | Question Area | Answer | Score |
|---|--------------|--------|-------|
| 1 | Unreachable for a week | [G/Y/R] | [0/5/10] |
| 2 | Approval dependency | [G/Y/R] | [0/5/10] |
...
| **Total** | | | **[X]/100** |

## Priority Areas (Highest Scores)
1. [Question area] — scored Red/10 — [specific observation]
2. [Question area] — scored Red/10 — [specific observation]
3. [Question area] — scored Yellow/5 — [specific observation]

## Recommendation
[Phase-specific recommendation from SEGMENT_INFO]

## Recommended Next Step
[Based on segment: EXTRACT skills for 51+, ASSIGN skills for 26-50, SCALE skills for 0-25]
```

## Quality Checklist

- [ ] All 10 questions answered — no skipping
- [ ] Scoring matches code exactly: Green=0, Yellow=5, Red=10
- [ ] Segment ranges match code: 0-25, 26-50, 51-75, 76-100
- [ ] Segment descriptions match SEGMENT_INFO from code
- [ ] Recommendations match code recommendations
- [ ] Tone is encouraging — a high score isn't a judgment, it's a map
- [ ] Priority areas identified from highest-scoring questions

## Example

**Input:** Founder answers 10 questions: 2 Green, 3 Yellow, 5 Red

**Output (excerpt):**
```
## Your Score: 65/100
## Segment: Single Point of Failure

Your business has a serious dependency problem — you. Critical knowledge lives in your head, and most decisions require your input. Growth is limited by your capacity.

## Priority Areas
1. Business knowledge in your head — scored Red/10 — Almost nothing is documented
2. Team escalation patterns — scored Red/10 — Everything comes to you
3. Client relationship dependency — scored Red/10 — Over 60% need you personally

## Recommendation
Start with EXTRACT. Get the systems out of your head and onto paper. Your Brain Dump list is your roadmap.
```

## Related Skills

- `brain-dump` -> `bottleneck-finder` -> this skill
- Score informs which phase to start: EXTRACT (51+), ASSIGN (26-50), SCALE (0-25)
- Rerun after implementing changes to track progress
- **Entry point:** `_router` — Start here if unsure which skill you need
