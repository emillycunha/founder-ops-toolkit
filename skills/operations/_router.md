---
name: operations-router
description: Intelligent entry point for all operations skills. Routes founder problems to the right tool. Use when hearing any operations-related problem, question, or request.
---

# Operations Router

## What This Does

The intelligent entry point for all 24 operations skills. When a founder describes a problem, question, or goal, this router identifies the right skill and executes it.

**You don't need to know which skill to use.** Just describe what's happening.

## How to Use

Simply state your problem or question:
- "I'm the bottleneck in my business"
- "Everything's in my head"
- "My team can't make decisions without me"
- "I need to build a dashboard"
- "Where do I start?"

The router will:
1. Match your input to the right skill
2. Ask ONE clarifying question if needed
3. Execute the skill with context

---

## Quick Reference: What to Say

| If you're experiencing... | Say something like... | Routes to |
|---------------------------|----------------------|-----------|
| Don't know where to start | "Where should I focus?" "Operations audit" | `ops-health-check` |
| Everything goes through you | "I'm the bottleneck" | `bottleneck-finder` |
| Knowledge stuck in your head | "Everything's in my head" | `brain-dump` |
| Team can't decide without you | "They always check with me" | `authority-ladder` |
| Ready to delegate something | "How do I hand this off?" | `handoff-script` |
| Need to document a process | "Write an SOP for this" | `sop-generator` |
| Calendar is chaos | "Too many meetings" | `meeting-audit` |
| Need metrics/KPIs | "Build me a dashboard" | `scorecard-builder` |
| Week feels unpredictable | "Design my ideal week" | `weekly-rhythm` |
| Unsure if ready to delegate | "Can someone else do this?" | `70-percent-rule` |

---

## Cluster Routing

### DIAGNOSE — "What's wrong? Where am I?"

**Trigger phrases:**
- "bottleneck," "constraint," "what's slowing us"
- "where should I focus," "operations audit," "health check"
- "where's my time going," "always busy but nothing done"
- "could this run without me," "bus factor," "founder dependency"
- "above the line," "waterline," "what should I keep"
- "capacity," "bandwidth," "overloaded"

**Skills:**
| Skill | Use when |
|-------|----------|
| `ops-health-check` | Don't know where to start |
| `bottleneck-finder` | Know you're the problem, need specifics |
| `constraint-finder` | Need to identify THE one thing holding you back |
| `founder-dependency-score` | Want to measure how dependent on you the business is |
| `time-audit` | Need to see where your hours actually go |
| `waterline-audit` | Need to separate CEO work from systemizable work |
| `capacity-planner` | Need to understand team bandwidth |

---

### EXTRACT — "Get it out of my head"

**Trigger phrases:**
- "brain dump," "everything in my head," "I'm the only one who knows"
- "document this," "map this process," "workflow"
- "SOP," "procedure," "standard operating procedure"

**Skills:**
| Skill | Use when |
|-------|----------|
| `brain-dump` | Starting from scratch, need to inventory everything |
| `process-mapper` | Have a specific process to document step-by-step |
| `sop-generator` | Ready to create a formal, reusable procedure |

---

### ASSIGN — "Hand it off to the team"

**Trigger phrases:**
- "delegate," "hand off," "give this to someone"
- "who owns this," "accountability," "RACI"
- "authority," "decision levels," "how much can they decide"
- "what needs my approval," "reversible," "one-way door"
- "should I hire," "hire vs systemize," "build a system"
- "team independence," "autonomy," "can they run things"
- "is this ready to delegate," "70%," "good enough"

**Skills:**
| Skill | Use when |
|-------|----------|
| `authority-ladder` | Need to define decision-making levels |
| `70-percent-rule` | Evaluating if a specific task is ready to delegate |
| `decision-filter` | Categorizing which decisions need your approval |
| `handoff-script` | Ready to actually hand something off, need the script |
| `accountability-matrix` | Clarifying ownership across functions |
| `team-autonomy-score` | Measuring how independent your team currently is |
| `hire-vs-systemize` | Deciding whether to hire or build a system |

---

### BUILD — "Create something"

**Trigger phrases:**
- "build a dashboard," "scorecard," "KPIs," "metrics"
- "weekly rhythm," "ideal week," "operating cadence"
- "project tracker," "milestones," "project status"
- "onboarding," "new client process," "kickoff"

**Skills:**
| Skill | Use when |
|-------|----------|
| `weekly-rhythm` | Designing your operating cadence |
| `scorecard-builder` | Creating a KPI dashboard |
| `project-tracker` | Setting up project status tracking |
| `client-onboarding` | Building client onboarding workflow |

---

### OPTIMIZE — "Make it better"

**Trigger phrases:**
- "too many meetings," "calendar review," "meeting audit"
- "results not tasks," "outcomes," "measure what matters"
- "prioritize," "4-box map," "what should I delegate"

**Skills:**
| Skill | Use when |
|-------|----------|
| `task-categorizer` | Sorting tasks to find what to delegate/eliminate |
| `outcome-shifter` | Converting task-thinking to outcome-thinking |
| `meeting-audit` | Reviewing and cutting unnecessary meetings |

---

## Clarifying Questions

When input is ambiguous, ask ONE of these:

| Ambiguous Input | Clarifying Question |
|-----------------|---------------------|
| "Help with my team" | "Is this about giving them more authority to decide, or measuring how independently they work?" |
| "I need a system" | "Are you documenting something you already do, or creating something new?" |
| "My week is chaos" | "Do you want to understand where your time goes, or design a better week?" |
| "I'm overwhelmed" | "Do you want to see where you're stuck, or are you ready to start handing things off?" |
| "Things keep falling through" | "Is this about clarifying who owns what, or about how you're handing things off?" |
| "Need more structure" | "Structure for your week, your team's decisions, or your processes?" |

---

## Routing Process

1. **Receive input** — Listen for the problem/question
2. **Scan for triggers** — Match against phrases above
3. **Identify cluster** — Which of the 5 clusters does this fall into?
4. **Single match?** → Announce and execute
5. **Multiple matches?** → Ask ONE clarifying question
6. **Execute** — Run the selected skill with gathered context

### Announcement Format

When routing, announce:

```
Running [skill-name]...
[One-line description of what it does]
```

Example:
```
Running bottleneck-finder...
Identifying where you're the constraint and ranking by severity.
```

---

## Common Journeys

### "I don't know where to start"
1. `ops-health-check` → Assess all 3 phases
2. Routes to weakest phase pipeline

### "I'm drowning"
1. `time-audit` → See where hours go
2. `task-categorizer` → Sort into delegate/keep/eliminate
3. `70-percent-rule` → Evaluate what's ready to hand off

### "My team is too dependent on me"
1. `founder-dependency-score` → Measure the problem
2. `brain-dump` → Get knowledge visible
3. `authority-ladder` → Define decision levels

### "I need to scale"
1. `ops-health-check` → Identify gaps
2. `weekly-rhythm` → Build operating cadence
3. `scorecard-builder` → Create tracking system

---

## Related Skills

- See `_cluster-map.md` for full cluster organization
- See `README.md` for framework overview
- Individual skills link back to this router

---

**Entry Point:** This IS the entry point. Start here.

**Last Updated:** 2026-02-02
