# Agent Patterns

This section studies the recurring patterns used to make agents reason, plan, choose actions, and recover from imperfect intermediate results.

Patterns are useful because they give structure to model behavior. They do not make a system reliable by themselves, but they help define how decisions are made and how work moves forward.

## Why This Section Matters

An agent is not just a model call. It is a decision process. Patterns help describe that process so it can be designed, debugged, and improved.

## Reading Order

1. `react-pattern.md`
2. `planning-vs-workflows.md`
3. `routing.md`
4. `reflection.md`
5. `structured-outputs.md`

## Module Map

| Topic | What It Should Explain | Status |
|---|---|---|
| ReAct | How reasoning and acting are interleaved. | Planned |
| Planning vs workflows | When to let the model plan and when to predefine steps. | Planned |
| Routing | How requests move to the right prompt, tool, or agent. | Planned |
| Reflection | How self-checking can improve or degrade results. | Planned |
| Structured outputs | Why schemas make behavior easier to parse and control. | Planned |

## Key Questions

- When should an agent plan dynamically?
- When is a fixed workflow more reliable?
- How does ReAct help with tool use?
- What is the risk of too much reflection?
- Why do structured outputs matter?

## Checkpoint

Before moving on, I should be able to choose a pattern for a simple agent task and explain why that pattern fits.

## Read Next

After patterns, move to `../02-tool-use` to study how agents take action through tools.
