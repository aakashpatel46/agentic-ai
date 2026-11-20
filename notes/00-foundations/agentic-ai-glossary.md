# Agentic AI Glossary

This glossary defines common terms used throughout the notes.

## Core Terms

| Term | Meaning |
|---|---|
| Agent | A system that uses a model to choose actions toward a goal. |
| Agentic | Having some ability to decide steps dynamically instead of only following fixed instructions. |
| Goal | The task or outcome the agent is trying to achieve. |
| Context | The information available to the model at a given step. |
| State | Information preserved across steps in the agent loop. |
| Tool | A function, API, file operation, search, calculator, or other action the agent can call. |
| Observation | The result returned after an action or tool call. |
| Stopping condition | A rule that tells the agent when to finish or pause. |
| Workflow | A predefined sequence of steps. |
| Orchestration | The software layer that manages prompts, tools, state, and control flow. |

## Model Terms

| Term | Meaning |
|---|---|
| LLM | Large language model. The model that reads context and generates output. |
| Token | A text unit processed by the model. |
| Context window | Maximum text the model can consider at once. |
| Prompt | Input sent to the model, including instructions and context. |
| Completion | Output produced by the model. |
| Structured output | Output constrained to a machine-readable format. |
| Hallucination | Unsupported or false model output. |

## Tool and Memory Terms

| Term | Meaning |
|---|---|
| Function calling | A model producing a structured request to call a tool. |
| Tool schema | The contract that defines tool name, inputs, outputs, and constraints. |
| RAG | Retrieval-augmented generation; retrieving external context before generating. |
| Embedding | Numeric representation of text meaning. |
| Vector search | Searching by similarity between embeddings. |
| Memory | Stored information used by the agent later. |

## Evaluation Terms

| Term | Meaning |
|---|---|
| Trace | Step-by-step record of an agent run. |
| Eval | A test or measurement of model or agent behavior. |
| Golden dataset | Curated examples with expected behavior. |
| Human-in-the-loop | A design where humans approve, review, or correct important steps. |
| Prompt injection | Malicious or conflicting instructions inserted through user or retrieved content. |

## Practical Takeaway

Good agentic AI work depends on precise vocabulary. If the terms are vague, the design will be vague too.
