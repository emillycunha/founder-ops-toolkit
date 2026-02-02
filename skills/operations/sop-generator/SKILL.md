---
name: sop-generator
description: Create standard operating procedures. Use when hearing "SOP," "document process," "write procedure," "standard operating procedure," or "how do I document this."
---

# SOP Generator

## What This Does

Creates a complete, ready-to-use Standard Operating Procedure from a process description or process map. The SOP is written so that someone with no prior knowledge of the task can follow it successfully.

## Framework Phase

**EXTRACT** — SOPs are the primary deliverable of the Extract phase. They transform tribal knowledge into transferable documentation that enables delegation.

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context:

- Process map (ideally from `process-mapper` skill) or verbal description
- Who will be following this SOP (role, skill level)
- What tools or systems are involved
- What "done well" looks like for this process
- Common mistakes or edge cases

## SOP Structure

Every SOP follows this standard template:

### 1. Header
- SOP Title (action-oriented: "How to [Do X]")
- Version number and date
- Owner (who maintains this SOP)
- Last reviewed date

### 2. Purpose
One sentence explaining why this process exists and what business outcome it supports.

### 3. Scope
Who uses this SOP and when. Includes:
- Roles that follow this procedure
- When/triggers for this procedure
- What this SOP does NOT cover

### 4. Steps
Numbered, sequential actions. Each step includes:
- Clear action verb (Send, Create, Check, Update, etc.)
- Specific details (which tool, which template, which field)
- Expected outcome of the step
- Screenshots or links where helpful

### 5. Decision Points
Where the process branches:
- Clear if/then logic
- Criteria for each path
- Who decides (if judgment is needed)

### 6. Quality Check
How to verify the output is correct:
- Checklist of what "done right" looks like
- Common mistakes to avoid
- What to double-check before marking complete

### 7. Escalation Path
When and how to escalate:
- What situations require escalation
- Who to escalate to
- What information to include when escalating

### 8. Related Resources
Links to templates, tools, examples, and related SOPs.

## SOP Writing Rules

- **Write for the newest team member.** If they can follow it, anyone can.
- **One action per step.** Don't combine "Open the spreadsheet and update column B" — make those two steps.
- **Be specific.** Not "send the email" but "send the Welcome Email using the template in Google Drive > Templates > Client Welcome."
- **Include the why.** Brief context helps people make judgment calls when edge cases arise.
- **Use active voice.** "Send the invoice" not "The invoice should be sent."
- **Number everything.** Steps, sub-steps, decision paths. No ambiguity about order.

## Process

1. Gather process information (from `process-mapper` output or founder description)
2. Write the Header (title, owner, version)
3. Write the Purpose (one sentence)
4. Define the Scope (who, when, boundaries)
5. Write each Step with specific actions, tools, and expected outcomes
6. Add Decision Points with clear criteria
7. Create the Quality Check (what "done right" looks like)
8. Define the Escalation Path
9. List Related Resources
10. Review: Could the newest team member follow this without asking questions?

## Output Format

```
# SOP: [How to Do X]

**Version:** 1.0
**Owner:** [Name/Role]
**Created:** [Date]
**Last Reviewed:** [Date]

---

## Purpose
[One sentence: why this process exists and what outcome it serves]

## Scope
- **Who follows this:** [Roles]
- **When to use:** [Trigger/condition]
- **Not covered:** [What this SOP doesn't include]

---

## Steps

### Step 1: [Action Verb + What]
[Specific instructions with tool/platform details]
- Expected outcome: [What should happen after this step]

### Step 2: [Action Verb + What]
[Specific instructions]
- Expected outcome: [Result]

### Decision Point: [Question]
- **If [condition A]:** [Go to Step X / Do Y]
- **If [condition B]:** [Go to Step X / Do Y]
- **Who decides:** [Role or criteria]

### Step 3: [Action Verb + What]
...

---

## Quality Check
Before marking this complete, verify:
- [ ] [Check 1]
- [ ] [Check 2]
- [ ] [Check 3]

## Common Mistakes
- [Mistake 1] — [How to avoid it]
- [Mistake 2] — [How to avoid it]

## Escalation
- **When to escalate:** [Conditions]
- **Who to contact:** [Name/Role]
- **Include:** [What info to provide]

## Related Resources
- [Template/Tool link]
- [Related SOP link]
```

## Quality Checklist

- [ ] A new team member could follow this without asking questions
- [ ] Every step has a clear action verb
- [ ] Tools and platforms are named specifically (not "the system")
- [ ] Decision points have explicit criteria, not "use your judgment"
- [ ] Quality check covers the most common failure modes
- [ ] Escalation path is defined — people know when to ask for help
- [ ] Language is warm and clear — not corporate or robotic
- [ ] SOP is concise — long enough to be complete, short enough to actually use

## Example

**Input:** Process map for "New Client Welcome Email" from a consulting firm

**Output (excerpt):**
```
# SOP: How to Send the New Client Welcome Email

**Version:** 1.0 | **Owner:** Client Success Lead | **Created:** 2026-01-24

## Purpose
Send a personalized welcome email within 24 hours of contract signing to set expectations and begin the onboarding relationship.

## Scope
- **Who follows this:** Anyone on the client success team
- **When to use:** Within 24 hours of receiving a signed contract notification
- **Not covered:** Follow-up emails after the welcome (see SOP: Client Onboarding Sequence)

## Steps

### Step 1: Open the Welcome Email Template
Go to Google Drive > Templates > Client Emails > "Welcome Email Template v3"
- Expected outcome: Template is open and ready to customize

### Step 2: Personalize the Email
Replace the following fields:
- [CLIENT NAME] — Use the name from the contract
- [PROJECT TYPE] — Match to the service package purchased
- [START DATE] — Use the date from the kickoff calendar invite
- Expected outcome: All brackets replaced with client-specific info

### Step 3: Review Before Sending
Read the full email once. Check:
- Client name spelled correctly
- Project type matches the contract
- Start date is accurate
- No template brackets remaining
- Expected outcome: Email is error-free and ready to send
```

## Related Skills

- `brain-dump` -> `process-mapper` -> this skill
- SOPs enable `handoff-script` — you can't delegate what isn't documented
- SOP targets come from `waterline-audit` top 5 list
- **Entry point:** `_router` — Start here if unsure which skill you need
