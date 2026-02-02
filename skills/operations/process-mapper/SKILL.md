---
name: process-mapper
description: Map workflows step-by-step. Use when hearing "map process," "workflow," "how does this work," "document the steps," or "walk me through the process."
---

# Process Mapper

## What This Does

Converts a verbal description of how something works into a clear, step-by-step workflow map with triggers, actions, decision points, and outputs. This is the bridge between "it's in my head" and "anyone can follow this."

## Framework Phase

**EXTRACT** — Process mapping is how tribal knowledge becomes transferable documentation. It's the precursor to SOP creation.

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context:

- Which process to map (name and general purpose)
- Who currently performs it (usually the founder)
- How often it runs
- What triggers it (what starts the process)
- What the end result looks like

## Process Mapping Elements

Every workflow map needs these components:

### 1. Trigger
What initiates this process? Examples:
- New client signs contract
- Team member submits a request
- Calendar reminder fires
- Client sends a message
- End of month arrives

### 2. Steps
Sequential actions taken. For each step:
- **Who** does it
- **What** they do (specific action)
- **Where** (which tool, platform, or location)
- **How long** it typically takes

### 3. Decision Points
Where the process branches based on conditions:
- If [condition], then [path A]
- If [not condition], then [path B]
- Mark which decisions require founder judgment vs. rules-based

### 4. Handoffs
Where responsibility transfers between people:
- From whom to whom
- What information passes with the handoff
- How the next person knows it's their turn

### 5. Output
What the process produces when complete:
- Deliverable or result
- Where it goes next
- How success is measured

## Process

1. Name the process and state its purpose in one sentence
2. Identify the trigger — what starts it
3. Walk through each step chronologically
4. At each step, capture: Who, What, Where, How Long
5. Identify decision points — where does the path branch?
6. Mark handoffs — where does responsibility change?
7. Define the output — what does "done" look like?
8. Review for missing steps (ask: "What could go wrong between step X and Y?")
9. Produce the workflow map

## Output Format

```
# Process Map: [Process Name]

## Purpose
[One sentence: what this process achieves]

## Trigger
[What starts this process]

## Owner
[Primary person responsible]

## Frequency
[How often this runs]

## Steps

### Step 1: [Action Name]
- **Who:** [Person/Role]
- **What:** [Specific action]
- **Where:** [Tool/Platform]
- **Time:** [Estimated duration]

### Step 2: [Action Name]
- **Who:** [Person/Role]
- **What:** [Specific action]
- **Where:** [Tool/Platform]
- **Time:** [Estimated duration]

### Decision Point: [Question]
- If [yes/condition A]: Go to Step [X]
- If [no/condition B]: Go to Step [Y]
- **Requires founder judgment?** [Yes/No]

### Step 3: [Action Name]
...

## Handoffs
| From | To | What Passes | Signal |
|------|-----|-------------|--------|
| [Role] | [Role] | [Info/deliverable] | [How they know] |

## Output
- **Deliverable:** [What is produced]
- **Destination:** [Where it goes]
- **Success criteria:** [How you know it worked]

## Estimated Total Time: [X minutes/hours]

## Recommended Next Step
Use `sop-generator` to turn this map into a full Standard Operating Procedure.
```

## Quality Checklist

- [ ] Process has a clear trigger — not "whenever I feel like it"
- [ ] Every step has Who, What, Where, and Time
- [ ] Decision points are identified — not hidden inside steps
- [ ] Handoffs are explicit — nothing falls through the cracks
- [ ] Output is defined — the process has a clear "done"
- [ ] Missing steps checked — "what could go wrong?" asked at each stage
- [ ] Language is simple enough for someone new to follow

## Example

**Input:** "Walk me through how we onboard a new client at my design agency."

**Output (excerpt):**
```
# Process Map: New Client Onboarding

## Trigger: Client signs contract and pays deposit

### Step 1: Send Welcome Email
- **Who:** Founder (currently)
- **What:** Send personalized welcome email with next steps
- **Where:** Gmail
- **Time:** 15 minutes

### Step 2: Create Project Folder
- **Who:** VA
- **What:** Set up Google Drive folder from template, share with client
- **Where:** Google Drive
- **Time:** 10 minutes

### Decision Point: Is this a rush project?
- If yes: Skip Step 3, go directly to Step 4 (Kickoff Call)
- If no: Proceed to Step 3 (Questionnaire)
- **Requires founder judgment?** No — defined by contract terms
```

## Related Skills

- `brain-dump` -> this skill -> `sop-generator`
- Process maps feed into `handoff-script` when transferring to team
- Complex processes may reveal bottlenecks for `bottleneck-finder`
- **Entry point:** `_router` — Start here if unsure which skill you need
