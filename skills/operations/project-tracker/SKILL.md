---
name: project-tracker
description: Set up project status and milestone tracking. Use when hearing "project tracking," "milestones," "project status," "where are we on this," or "what's the status."
---

# Project Tracker

## What This Does

Creates a simple, visual project tracking system with clear status indicators, milestones, and blockers. Gives the founder and team a shared view of what's on track, what's behind, and what needs attention — without requiring the founder to check every project personally.

## Framework Phase

**Cross-Phase** — Project tracking supports all phases: makes work visible (EXTRACT), enables team ownership (ASSIGN), and provides the rhythm data (SCALE).

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context:

- Current projects or clients being managed
- How the founder currently tracks progress (spreadsheet, memory, tool)
- What milestones matter for each project type
- Who needs visibility into project status
- Common project failure points (where things go off track)

## Project Tracking Elements

### Status Levels

Every project gets a simple status using the traffic light system:

| Status | Meaning | Action Required |
|--------|---------|----------------|
| **Green** | On track — hitting milestones on schedule | None — keep going |
| **Yellow** | At risk — behind schedule or blocker emerging | Needs attention this week |
| **Red** | Off track — missed milestones or blocked | Needs immediate intervention |
| **Complete** | Delivered and closed | Archive and review |

### Milestones

Break each project into 3-5 key milestones. Each milestone has:

- **Name:** What this stage accomplishes
- **Due date:** When it should be complete
- **Owner:** Who is responsible for delivering it
- **Deliverable:** What's produced when this milestone is hit
- **Status:** Green / Yellow / Red / Complete

### Blockers

When a project is Yellow or Red, document:

- **What's blocked:** Specific description
- **Blocked by:** Person, resource, decision, or external factor
- **Since when:** How long it's been blocked
- **Resolution path:** What needs to happen to unblock

## Process

1. List all active projects or clients
2. Define 3-5 milestones for each project type (can be templated)
3. Assign status (Green/Yellow/Red) to each project
4. Assign an owner for each project and milestone
5. Identify current blockers for Yellow/Red projects
6. Set up a weekly review cadence (integrate with `weekly-rhythm`)
7. Create the tracker

## Output Format

```
# Project Tracker — [Business Name]

## Active Projects Summary
| Project | Client | Owner | Status | Next Milestone | Due |
|---------|--------|-------|--------|---------------|-----|
| [Project] | [Client] | [Name] | [G/Y/R] | [Milestone] | [Date] |

## Detailed Project Status

### [Project Name]
- **Client:** [Name]
- **Owner:** [Name]
- **Status:** [Green/Yellow/Red]
- **Start Date:** [Date]
- **Target Completion:** [Date]

**Milestones:**
| # | Milestone | Due | Owner | Status |
|---|-----------|-----|-------|--------|
| 1 | [Name] | [Date] | [Name] | [Complete/Green/Yellow/Red] |
| 2 | [Name] | [Date] | [Name] | [Status] |
| 3 | [Name] | [Date] | [Name] | [Status] |

**Blockers:**
| Blocker | Blocked By | Since | Resolution |
|---------|-----------|-------|------------|
| [Description] | [Person/thing] | [Date] | [What needs to happen] |

## Weekly Review Template
Review each project during Friday Wrap:
1. Is the status accurate? (Update Green/Yellow/Red)
2. Any new blockers? (Document them)
3. Any milestones hit this week? (Celebrate and mark complete)
4. What's the #1 thing that needs to happen next week for each project?

## Recommended Next Step
Integrate this tracker into `weekly-rhythm` Friday Wrap and Monday Alignment. Use `scorecard-builder` for aggregate project metrics.
```

## Quality Checklist

- [ ] Every active project has a clear status (Green/Yellow/Red)
- [ ] Milestones are specific and date-bound — not vague phases
- [ ] Every project has a single owner
- [ ] Blockers documented with resolution paths
- [ ] Weekly review cadence set up (connects to `weekly-rhythm`)
- [ ] Tracker is simple enough to update in 5 minutes
- [ ] Founder can see status without attending every project meeting

## Example

**Input:** "I have 5 active web design clients. I check in with each one myself to know the status. It takes me 2-3 hours a week just to figure out where we are."

**Output (excerpt):**
```
## Active Projects Summary
| Project | Client | Owner | Status | Next Milestone | Due |
|---------|--------|-------|--------|---------------|-----|
| Website Redesign | Acme Co | Sarah | Green | Design Mockups | Feb 3 |
| Brand Package | Summit LLC | Sarah | Yellow | Logo Options | Jan 28 (2 days late) |
| Landing Page | Nova Inc | Marcus | Green | Copy Draft | Feb 1 |

### Brand Package — Summit LLC
- **Status:** Yellow
- **Blocker:** Waiting on client feedback since Jan 22 (3 days)
- **Resolution:** Sarah to send follow-up email today; escalate to founder if no response by Friday
```

## Related Skills

- This skill integrates into `weekly-rhythm` (Monday Alignment + Friday Wrap)
- Project metrics feed into `scorecard-builder`
- Blocked projects may surface issues for `bottleneck-finder`
- New project setup uses `client-onboarding` workflow
- **Entry point:** `_router` — Start here if unsure which skill you need
