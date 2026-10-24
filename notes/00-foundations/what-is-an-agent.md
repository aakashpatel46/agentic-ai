# What Is an AI Agent?

An AI agent is a system that uses a model to decide what to do next, often across multiple steps, in order to complete a goal.

A simple chatbot usually responds once. An agent can observe the current state, decide on an action, use a tool, inspect the result, and continue until the task is complete or blocked.

## A Working Definition

An AI agent combines:

- A goal or task.
- A model that reasons over the task.
- Instructions that shape behavior.
- Tools or actions it can use.
- State or memory across steps.
- A stopping condition.

The more autonomy the system has over choosing and sequencing actions, the more agentic it becomes.

## Chatbot vs Workflow vs Agent

A chatbot responds to a message.

A workflow follows predefined steps.

An agent chooses steps dynamically based on the current goal, context, and tool results.

In practice, many useful systems are hybrids. A reliable production system may use deterministic workflows around agentic parts.

## Core Agent Loop

A basic agent loop looks like this:

1. Observe the user request and current state.
2. Decide what action is useful next.
3. Act by calling a tool, writing output, asking a question, or stopping.
4. Inspect the result.
5. Repeat until done.

## Why Agents Matter

Agents matter because they let language models interact with the world beyond text generation. They can use APIs, inspect files, retrieve knowledge, run calculations, coordinate workflows, and adapt to new information.

The hard part is reliability. A useful agent must know when to act, when to stop, when to ask for help, and how to recover from mistakes.

## Common Failure Modes

- The agent calls the wrong tool.
- The agent over-plans instead of doing the simple next step.
- The agent trusts bad tool output.
- The agent loses track of the original goal.
- The agent keeps going after it should stop.
- The agent invents facts instead of retrieving or verifying them.

## My Mental Model

An agent is not magic. It is a loop around a model, plus tools, state, instructions, and evaluation.

The craft is designing that loop so the system is useful, inspectable, and hard to misuse.
