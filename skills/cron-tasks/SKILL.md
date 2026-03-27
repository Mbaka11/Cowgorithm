# Task Execution Reference — Cowgorithm

## Purpose

Reference for how the agent should execute tasks from the backlog
(`research/research-plan.md`). No cron schedules — all work is on-demand.

## Task Sources

Tasks come from two places:

1. **research/research-plan.md** — the master backlog with phases and sub-tasks
2. **WhatsApp / CLI commands** — ad-hoc requests from the founder

## Execution Flow

When given a task (or told to "work through the backlog"):

```
1. Read research/research-plan.md → find first "Not started" task
2. Research the topic (browser, existing docs, sources.md)
3. Write findings to the appropriate document
4. Update research-plan.md: mark task as "Done"
5. Update research/sources.md with new sources
6. Send WhatsApp summary: what was done, key findings, any questions
7. If more tasks remain in scope → go to step 1
8. If done or blocked → stop and report
```

## Completion Criteria

A task is "Done" when:
- The target document has substantive content (not just headers)
- Every factual claim has a cited source
- TAM/SAM/SOM calculations show assumptions and math
- The research-plan.md status is updated
- sources.md includes all new references

## When to Stop and Ask

- Pricing/strategy decisions (e.g., "should we price at $25 or $35/month?")
- Conflicting data that changes a previous recommendation
- A task requires information the founder has but isn't in the repo
- Score results that challenge the current segment ranking

## Adjacent Market Exploration

When asked to explore new verticals:
1. Check `research/explorations/` for what's already been covered
2. Pick a vertical NOT yet explored
3. Research Canadian market size, players, regulations
4. Score using the 5-factor framework (see `skills/research/SKILL.md`)
5. Write to `research/explorations/{topic-slug}.md`
6. Flag anything scoring ≥ 3.5/5 as "High Potential"

### Ideas backlog (pick from here or find your own)
- Wildlife management / caribou tracking
- Forestry worker safety
- Mining site vehicle tracking
- Delivery fleet management
- Elder care wandering prevention
- Indigenous community livestock programs
- Recreational vehicle tracking
- Marine vessel tracking
- Drone fleet management
- Agricultural equipment tracking
- Snow removal fleet optimization
- Ski resort safety / avalanche rescue
