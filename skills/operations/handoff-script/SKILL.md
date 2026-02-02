---
name: handoff-script
description: Generate delegation scripts for tasks. Use when hearing "hand off," "delegate this," "transfer task," "give this to my team," or "how do I explain this to them."
---

# Handoff Script

## What This Does

Creates a structured delegation conversation script that clearly communicates what's being handed off, why, the authority boundaries, success criteria, and check-in cadence. This removes ambiguity from delegation.

## Framework Phase

**ASSIGN** — The Handoff Script is the execution step of the Assign phase. It turns authority decisions into actual conversations with team members.

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context:

- What task or responsibility is being delegated
- Who is receiving it (name, role, current capabilities)
- Authority level assigned (from `authority-ladder`)
- The SOP if one exists (from `sop-generator`)
- What support the team member will have during transition

## The Handoff Framework

Every delegation conversation covers seven elements:

### 1. The What
Clearly describe the task or responsibility being transferred. Be specific — not "handle client communication" but "respond to all routine client emails within the same business day using the approved templates."

### 2. The Why
Explain why this is being delegated and why to this person. This builds ownership and motivation.
- Why the business needs this: [business reason]
- Why you specifically: [what makes them right for this]

### 3. The Authority Level
State explicitly what they can decide on their own:
- Level 1: Research and present options to me
- Level 2: Recommend a path, I'll approve
- Level 3: Decide and let me know what you chose
- Level 4: Decide, no need to tell me
- Level 5: Own it and teach others

### 4. The Boundaries
Define the edges — what's in scope and what's not:
- You CAN: [specific actions within authority]
- You CANNOT: [specific actions that still need founder]
- Escalate if: [specific conditions that require checking in]

### 5. The Success Criteria
What "done well" looks like — measurable when possible:
- [Metric or observable outcome]
- [Quality standard]
- [Timeline expectation]

### 6. The Support
What resources and support are available:
- SOP or documentation location
- Who to ask if stuck (besides the founder)
- Tools or templates available

### 7. The Check-In
How and when you'll review progress:
- First check-in: [when — usually within first week]
- Ongoing cadence: [weekly, biweekly, or on-demand]
- What to bring to check-ins: [status, blockers, decisions made]

## Process

1. Identify the task and the delegate
2. Determine the authority level (from `authority-ladder`)
3. Draft the handoff script using the 7 elements
4. Review for clarity — could the team member repeat it back accurately?
5. Schedule the handoff conversation
6. Deliver the script in conversation (not just email)
7. Set up the first check-in

## Output Format

```
# Handoff Script: [Task Name]

## For: [Team Member Name] ([Role])

---

### "Here's what I'd like you to take over..."

**The What:**
"I'm handing off [specific task/responsibility]. This means you'll be responsible for [specific actions]."

**The Why:**
"This matters because [business reason]. And I'm giving this to you because [personal reason — capability, growth, fit]."

**Your Authority:**
"For this, you're at Level [X] — [level name]. That means [plain-language explanation of what they can decide]."

**The Boundaries:**
- You CAN: [list specific authorized actions]
- Escalate to me if: [list specific escalation triggers]
- You do NOT need to ask me about: [list things they might think need approval but don't]

**What Success Looks Like:**
- [Measurable outcome 1]
- [Measurable outcome 2]
- [Timeline expectation]

**Support Available:**
- SOP: [location or link]
- Questions go to: [person or resource]
- Tools: [relevant tools/templates]

**Our Check-In Plan:**
- First review: [date/timeframe]
- Ongoing: [cadence]
- Bring to check-ins: [what to prepare]

---

### Conversation Notes
- Deliver this in person or on a call — not just email
- Ask them to repeat back what they understood
- Ask: "What questions do you have?" (not "Do you have questions?")
- Reassure: "The first few times won't be perfect, and that's fine."
```

## Quality Checklist

- [ ] All 7 elements covered — nothing left ambiguous
- [ ] Authority level is explicit (from `authority-ladder`)
- [ ] Boundaries include "you do NOT need to ask me about" — this prevents unnecessary escalation
- [ ] Success criteria are measurable, not vague
- [ ] Check-in plan is realistic — not too frequent (micromanaging) or too infrequent (abandonment)
- [ ] Script is conversational — not a corporate memo
- [ ] Includes emotional reassurance — delegation is vulnerable for both sides

## Example

**Input:** "Hand off weekly client status emails to my project manager Sarah. She's at Authority Level 3."

**Output (excerpt):**
```
### "Here's what I'd like you to take over..."

**The What:**
"I'm handing off weekly client status emails. This means every Friday by 3pm, you'll send each active client a status update covering what was completed, what's in progress, and any blockers."

**The Why:**
"Clients need consistent communication, and right now it only happens when I remember. You already know the project status better than I do — you're closer to the work."

**Your Authority:**
"You're at Level 3 — Decide & Inform. Send the emails yourself. You don't need my review. Just let me know if a client raises a concern you're not sure how to handle."

**The Boundaries:**
- You CAN: Write, customize, and send all routine status emails
- Escalate to me if: A client expresses frustration or requests a call with me
- You do NOT need to ask me about: Tone adjustments, minor timeline updates, or adding project details

**What Success Looks Like:**
- Every active client gets a status email by Friday 3pm
- Zero client follow-ups saying "what's the status?"
- You feel confident sending without reviewing with me by Week 3
```

## Related Skills

- `authority-ladder` -> `70-percent-rule` -> `decision-filter` -> this skill
- Requires SOP from `sop-generator` for complex handoffs
- Feeds into `team-autonomy-score` tracking
- **Entry point:** `_router` — Start here if unsure which skill you need
