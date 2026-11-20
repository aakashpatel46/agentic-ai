# Multi-Agent Systems

This section explores systems where more than one agent participates in a task.

Multi-agent systems can help when work naturally separates into roles, but they can also add cost, latency, and confusion. The goal is to understand when multiple agents are useful and how to coordinate them clearly.

## Why This Section Matters

Multiple agents sound powerful, but they are not automatically better. This section focuses on the design judgment needed to use them only when they improve clarity, specialization, review, or parallel work.

## Reading Order

1. `when-to-use-multiple-agents.md`
2. `manager-worker-pattern.md`
3. `planner-executor-pattern.md`
4. `reviewer-agents.md`
5. `handoffs.md`
6. `shared-state.md`

## Module Map

| Topic | What It Explains | Status |
|---|---|---|
| When to use multiple agents | Criteria for splitting work across agents. | Drafted |
| Manager-worker | One coordinator delegates to specialists. | Drafted |
| Planner-executor | One agent plans, another executes. | Drafted |
| Reviewer agents | Critique, validation, and quality checks. | Drafted |
| Handoffs | Passing context and responsibility between agents. | Drafted |
| Shared state | How agents coordinate without losing context. | Drafted |

## Key Questions

- What problem does each extra agent solve?
- What information must be passed during a handoff?
- How do agents avoid duplicating work?
- When does review improve quality?
- What makes multi-agent systems harder to debug?

## Checkpoint

Before moving on, I should be able to sketch a multi-agent workflow and explain why each role exists.

## Read Next

After multi-agent systems, move to `../05-evaluation-and-observability` to study reliability and debugging.
