# Memory and RAG

This section studies how agents use knowledge beyond the immediate prompt.

Retrieval and memory help agents work with documents, prior interactions, and domain-specific information. They also introduce design problems around what to store, what to retrieve, and what to trust.

## Why This Section Matters

Most useful agents need information that is not inside the model's current context. Retrieval and memory provide that information, but they must be designed carefully or the agent will retrieve the wrong thing with confidence.

## Reading Order

1. `rag-basics.md`
2. `embeddings.md`
3. `chunking.md`
4. `vector-search.md`
5. `agent-memory.md`
6. `retrieval-evaluation.md`

## Module Map

| Topic | What It Should Explain | Status |
|---|---|---|
| RAG basics | How retrieval augments generation. | Planned |
| Embeddings | How text becomes searchable as vectors. | Planned |
| Chunking | How splitting documents changes retrieval quality. | Planned |
| Vector search | How similar meaning is found. | Planned |
| Agent memory | Short-term, long-term, episodic, and semantic memory. | Planned |
| Retrieval evaluation | How to test whether the right context is retrieved. | Planned |

## Key Questions

- When is RAG useful?
- What should be embedded?
- How large should chunks be?
- What is the difference between retrieval and memory?
- How do we test if retrieval is good?

## Checkpoint

Before moving on, I should be able to explain a basic RAG pipeline from document ingestion to final answer.

## Read Next

After memory and RAG, move to `../04-multi-agent-systems` to study coordination between agents.
