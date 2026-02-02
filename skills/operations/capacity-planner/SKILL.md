---
name: capacity-planner
description: Calculate bandwidth and workload limits. Use when hearing "capacity," "bandwidth," "can we take more," "are we overloaded," or "how many clients can we handle."
---

# Capacity Planner

## What This Does

Calculates how much work the founder and team can realistically handle, identifies where capacity is maxed out, and determines whether the business can take on more without breaking.

## Framework Phase

**Cross-Phase** — Capacity planning spans all phases. It informs extraction priorities (EXTRACT), hiring decisions (ASSIGN), and sustainable rhythm (SCALE).

**Context:** `/context/operations-reset-framework.md`

## Before Starting

Gather this context:

- Team members and their roles
- Working hours per week for each person
- Current client count and project load
- How much time each type of client or project requires
- Any known capacity issues or overload symptoms

## Capacity Calculation

### Step 1: Available Hours

For each team member:

```
Gross Hours = Working days/week x Hours/day
Overhead = Meetings + Admin + Communication (typically 20-30%)
Available Hours = Gross Hours - Overhead
```

### Step 2: Utilization Targets

Not all available hours should be client work. Healthy targets:

| Role | Billable/Productive Target | Why Not 100% |
|------|---------------------------|--------------|
| Founder | 40-50% | Strategic work, business development, management |
| Senior team | 65-75% | Some oversight, mentoring, improvement work |
| Junior team | 75-85% | Mostly execution with some learning time |

### Step 3: Client/Project Cost

For each client type or project type:

```
Hours per client/project = (Delivery hours + Communication + Admin + Buffer)
```

Always add a 15-20% buffer for scope creep, revisions, and unexpected needs.

### Step 4: Capacity Math

```
Max clients = Total available productive hours / Hours per client
Current utilization = Current client hours / Total available productive hours
Remaining capacity = Max clients - Current clients
```

## Capacity Health Indicators

| Utilization | Status | Meaning |
|-------------|--------|---------|
| Under 60% | **Under-utilized** | Room for growth — take on more work or reduce team |
| 60-80% | **Healthy** | Sustainable pace with room for surprises |
| 80-90% | **Near capacity** | Can handle current load but no room for error |
| Over 90% | **Overloaded** | Quality will drop, burnout is likely, no buffer for problems |

## Process

1. List all team members with their weekly hours
2. Calculate overhead and available hours for each
3. Apply utilization targets by role
4. Calculate hours required per client/project type
5. Determine maximum capacity (clients or projects)
6. Compare current load to maximum
7. Identify bottleneck person (who hits capacity first)
8. Produce the capacity analysis

## Output Format

```
# Capacity Plan — [Business Name]

## Team Capacity
| Person | Role | Gross Hrs | Overhead | Available | Target Util | Productive Hrs |
|--------|------|-----------|----------|-----------|-------------|----------------|
| [Name] | [Role] | [X] | [X] | [X] | [X]% | [X] |

## Client/Project Cost
| Type | Delivery | Comms | Admin | Buffer | Total Hrs |
|------|----------|-------|-------|--------|-----------|
| [Type] | [X] | [X] | [X] | [X] | [X] |

## Capacity Summary
- Maximum clients at healthy utilization: [X]
- Current clients: [X]
- Current utilization: [X]%
- Remaining capacity: [X] clients / [X] hours
- Status: [Under-utilized / Healthy / Near Capacity / Overloaded]

## Bottleneck Person: [Name]
[Who hits capacity first and why — this person limits growth]

## Recommendations
1. [Specific recommendation based on status]
2. [Action to increase capacity if needed]
```

## Quality Checklist

- [ ] Overhead calculated realistically (20-30%, not 5%)
- [ ] Buffer included in client hours (15-20%)
- [ ] Utilization targets are sustainable, not aspirational
- [ ] Bottleneck person identified — this is where to focus
- [ ] Founder's strategic time protected — not all productive hours assigned to clients
- [ ] Recommendations are actionable

## Example

**Input:** "I have myself and 2 team members. We serve 8 clients, each needs about 10 hours/month of work. Am I at capacity?"

**Output (excerpt):**
```
## Capacity Summary
- Maximum clients at healthy utilization: 12
- Current clients: 8
- Current utilization: 67%
- Remaining capacity: 4 clients / 40 hours per month
- Status: Healthy

## Bottleneck Person: Founder
You're spending 15 hrs/month on client delivery + 10 hrs/month on each client's strategic oversight. At 8 clients, you're at 80% utilization with no room for business development. Your team has capacity; you don't.
```

## Related Skills

- `time-audit` -> this skill
- Informs `hire-vs-systemize` decisions
- Connects to `weekly-rhythm` for Strategic Margin
- **Entry point:** `_router` — Start here if unsure which skill you need
