# LLM Basics for Agents

A language model is the reasoning and language engine inside many modern agents. It reads context and produces text or structured output. In an agentic system, that output may become a final answer, a tool call, a plan, a critique, or a request for more information.

## Why It Matters

Agent design becomes clearer when the model is understood as one component, not the whole system. The model predicts useful next text from context. The agent loop around it decides how that text is used.

## Mental Model

Think of an LLM as a powerful pattern engine with limited working memory. It can reason over the context you provide, but it does not automatically know your private files, current database state, or whether its answer is true.

```mermaid
flowchart LR
    Prompt[Prompt and Context] --> Model[LLM]
    Model --> Output[Text or Structured Output]
    Output --> App[Agent Runtime]
    App --> Tool[Tool Call or Final Answer]
```

## Core Terms

| Term | Meaning |
|---|---|
| Token | A chunk of text processed by the model. |
| Context window | The maximum amount of text the model can consider at once. |
| Prompt | The instructions and information sent to the model. |
| Completion | The model output. |
| System instruction | High-priority behavior guidance. |
| Structured output | Output constrained to a schema such as JSON. |
| Hallucination | A confident answer that is unsupported or false. |

## Context Window

The context window is the model's working space. It can include instructions, user input, retrieved documents, tool results, and conversation history.

A larger context window helps, but it does not remove the need for good retrieval and clear instructions. Too much irrelevant context can make the model less focused.

## Prompts and Instructions

Agent prompts usually include:

- Role and behavior instructions.
- The user's goal.
- Available tools.
- Rules for when to use tools.
- Output format requirements.
- Safety and refusal rules.

The prompt is not just a message. It is part of the control system.

## Structured Outputs

Agents often need structured output so software can parse the model's decision.

Example:

```json
{
  "action": "search_notes",
  "query": "agent loop stopping condition"
}
```

Structured outputs reduce ambiguity. They make it easier to validate decisions and route the next step.

## Common Failure Modes

- The model invents facts when it should ask or retrieve.
- The model follows irrelevant context too strongly.
- The model produces output that software cannot parse.
- The prompt gives unclear tool-use rules.
- The model appears certain even when evidence is weak.

## Practical Takeaways

- Give the model only the context it needs.
- Use tools for facts, calculations, files, APIs, and current information.
- Use structured outputs when software must act on model decisions.
- Treat model output as a proposal that the agent runtime can validate.
- Design prompts and tools together, not separately.

## My Notes

For agentic systems, the LLM is the brain-like part, but the runtime is the nervous system. The system becomes useful when the model, tools, state, and checks work together.
