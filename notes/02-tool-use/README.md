# Tool Use

This section focuses on how agents interact with the outside world through tools.

Tools are what make an agent more than a text generator. A tool-using agent can call functions, query APIs, inspect files, run calculations, search knowledge, or trigger workflows.

## Why This Section Matters

Tool use is where agent design becomes practical. It is also where risk increases, because the agent can affect systems outside the model.

## Reading Order

1. `what-is-a-tool.md`
2. `function-calling.md`
3. `tool-schemas.md`
4. `tool-selection.md`
5. `tool-safety.md`
6. `error-handling.md`

## Module Map

| Topic | What It Should Explain | Status |
|---|---|---|
| What is a tool? | How tools extend the model's abilities. | Planned |
| Function calling | How models request structured actions. | Planned |
| Tool schemas | How inputs, outputs, and constraints are described. | Planned |
| Tool selection | How agents decide which tool to use. | Planned |
| Tool safety | How permissions and approvals reduce risk. | Planned |
| Error handling | How agents recover when tools fail or return bad output. | Planned |

## Key Questions

- What should be a tool and what should stay in the prompt?
- How should tool inputs be validated?
- When should a human approve an action?
- How does an agent recover from tool failure?
- How do logs make tool use inspectable?

## Checkpoint

Before moving on, I should be able to design a simple tool schema and explain how an agent would call it safely.

## Read Next

After tool use, move to `../03-memory-and-rag` to study how agents use external knowledge.
