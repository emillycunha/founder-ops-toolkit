---
name: bottleneck-finder
description: Identify where the founder is the constraint. Use when hearing "I'm the bottleneck," "everything goes through me," "my team waits on me," or "I can't take time off."
---

# Bottleneck Finder

## What This Does

Diagnoses the specific operational bottlenecks where the founder is the constraint, ranks them by severity, and routes to the correct Operations Reset Framework phase for resolution.

## Framework Phase

**EXTRACT** — Bottleneck identification is a diagnostic step that reveals where extraction is most urgent. Results often span all three phases.

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context (ask if not provided):

- Brain Dump Inventory (if available from `brain-dump` skill)
- Team size and structure
- What happened last time the founder was unavailable for a week
- Where the founder feels most "stuck"

## The 5 Bottleneck Questions

Ask each question and capture specific examples, not generalizations:

### 1. What breaks when you leave?

What literally stops functioning if you're unreachable for 3 days? Not "things slow down" — what actually breaks?

- Client deliverables stall?
- Team can't make decisions?
- Revenue-generating activities stop?
- Emergencies have no resolution path?

### 2. What has the longest queue?

Where do things pile up waiting on you?

- Approval backlogs (designs, proposals, invoices)
- Decision queues (hiring, pricing, scope changes)
- Communication bottlenecks (only you talk to certain clients)
- Review cycles (everything needs your eyes before it ships)

### 3. Where do people wait on you?

Different from queues — this is about team idle time:

- Team members blocked until you respond
- Projects paused mid-stream for your input
- Meetings that can't happen without you
- Information that only lives in your head

### 4. What do you do that nobody else can?

Challenge every answer here. "Nobody else can" usually means:

- Nobody else has been trained (fixable)
- Nobody else has been given permission (fixable)
- It genuinely requires your judgment (keep — but fewer than you think)

### 5. What fires recur monthly?

Recurring fires reveal systemic bottlenecks:

- Same client issue that keeps coming back
- Same team mistake that keeps happening
- Same process that keeps breaking
- Same emergency that keeps pulling you in

## Severity Scoring

Rate each bottleneck on three dimensions:

| Dimension | Low (1) | Medium (2) | High (3) |
|-----------|---------|------------|----------|
| **Frequency** | Monthly or less | Weekly | Daily |
| **Impact** | Inconvenience | Delays revenue | Stops revenue |
| **Dependency** | Others can partially cover | Others struggle without me | Only I can do this |

**Total Score (3-9):**
- 3-4: Minor bottleneck — address in normal workflow
- 5-6: Moderate bottleneck — prioritize within current quarter
- 7-9: Critical bottleneck — address immediately

## Phase Routing

Based on bottleneck type, route to the correct framework phase:

| Bottleneck Type | Route To | Why |
|----------------|----------|-----|
| "It's not documented" | EXTRACT | Need to get it out of founder's head |
| "Nobody has permission" | ASSIGN | Need to transfer authority |
| "No system to catch it" | SCALE | Need to install rhythm and monitoring |
| "Nobody is trained" | EXTRACT then ASSIGN | Document first, then delegate |

## Process

1. Ask the 5 Bottleneck Questions — capture specific examples
2. List all identified bottlenecks
3. Score each on Frequency, Impact, and Dependency (3-9)
4. Rank by total severity score
5. Classify each bottleneck type
6. Route to the appropriate framework phase
7. Identify the #1 bottleneck to fix first

## Output Format

```
# Bottleneck Diagnosis — [Founder Name]

## Top Bottleneck
[Name]: [One-sentence description]
- Severity: [Score]/9
- Type: [Not documented / No permission / No system / Not trained]
- Phase: [EXTRACT / ASSIGN / SCALE]
- Fix starts with: [Specific first action]

## All Bottlenecks Ranked
| # | Bottleneck | Freq | Impact | Depend | Score | Phase |
|---|------------|------|--------|--------|-------|-------|
| 1 | [Name] | [1-3] | [1-3] | [1-3] | [3-9] | [Phase] |

## Recommended Action Sequence
1. [First bottleneck] — [specific action] — use `[skill-name]`
2. [Second bottleneck] — [specific action] — use `[skill-name]`
3. [Third bottleneck] — [specific action] — use `[skill-name]`
```

## Quality Checklist

- [ ] All 5 questions asked with specific examples, not generalizations
- [ ] "Only I can do this" challenged at least once
- [ ] Severity scores reflect actual business impact, not founder anxiety
- [ ] Phase routing matches the bottleneck type accurately
- [ ] Single #1 bottleneck identified — not a tie
- [ ] Tone is calm and constructive — bottleneck findings can feel heavy

## Example

**Input:** "I run a coaching practice with 2 VAs. I handle all client communication, session prep, and billing. My VAs do admin but always need to check with me."

**Output (excerpt):**
```
## Top Bottleneck
Client communication dependency: All client emails, scheduling changes, and session follow-ups go through you personally.
- Severity: 8/9 (Daily + Delays revenue + Only me)
- Type: Not documented + No permission
- Phase: EXTRACT then ASSIGN
- Fix starts with: Document your client communication templates and give your VA authority to handle routine responses.
```

## Related Skills

- `brain-dump` -> this skill -> `founder-dependency-score`
- Use `constraint-finder` for deeper single-constraint analysis
- Route to `sop-generator` (Extract), `authority-ladder` (Assign), or `weekly-rhythm` (Scale) based on findings
- **Entry point:** `_router` — Start here if unsure which skill you need
