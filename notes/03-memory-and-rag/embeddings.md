# Embeddings

Embeddings are numeric representations of text meaning.

They allow systems to compare pieces of text by semantic similarity instead of exact keyword match.

## Why It Matters

Embeddings are the foundation of many RAG systems. They help an agent find relevant information even when the user's words do not exactly match the document text.

## Mental Model

```mermaid
flowchart LR
    A[Text Chunk] --> B[Embedding Model]
    B --> C[Vector]
    C --> D[Similarity Search]
```

## Simple Example

The phrases "fix login bug" and "resolve authentication failure" may not share many words, but their embeddings may be close because the meaning is similar.

## How Embeddings Are Used

1. Convert documents into vectors.
2. Convert the user's query into a vector.
3. Compare query vector to document vectors.
4. Return the closest matches.

## Similarity

Similarity is usually measured with cosine similarity or related distance metrics. The system looks for vectors that are close in meaning.

## Common Failure Modes

- Similar text is not actually useful for the task.
- Important exact keywords are missed.
- Short chunks lack enough meaning.
- Long chunks mix unrelated concepts.
- Embedding model does not fit the domain well.

## Practical Takeaways

- Embeddings are for semantic search, not truth.
- Inspect search results manually during development.
- Combine keyword and vector search when exact terms matter.
- Use retrieval evaluation to test whether embeddings help.
