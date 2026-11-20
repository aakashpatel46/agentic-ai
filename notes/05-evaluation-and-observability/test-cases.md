# Test Cases

Test cases are example tasks used to check whether an agent behaves correctly.

## Why It Matters

Agents are probabilistic and multi-step. Good test cases help detect regressions when prompts, tools, models, or retrieval settings change.

## Test Case Structure

A useful agent test case includes:

- User input.
- Available context.
- Expected behavior.
- Expected tool calls, if any.
- Expected final answer qualities.
- Things the agent must not do.

## Example

```yaml
name: retrieve_policy_answer
input: "What is the refund window?"
expected:
  should_retrieve: true
  source: "refund-policy.md"
  must_not: "invent policy details"
```

## Types of Test Cases

- Happy path.
- Missing information.
- Ambiguous request.
- Tool failure.
- No-answer retrieval case.
- Prompt injection attempt.
- Risky action requiring approval.

## Common Failure Modes

- Tests are too broad.
- Expected behavior is unclear.
- Only final text is checked.
- Tool behavior is not verified.
- Tests are not updated when requirements change.

## Practical Takeaways

- Start with a small, high-quality test set.
- Include failure and refusal cases.
- Keep expected behavior specific.
- Use traces to debug failed tests.
