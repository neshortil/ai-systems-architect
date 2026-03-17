# 🔍 RAG

> Retrieval-Augmented Generation pipeline designs and configurations.

---

## What's Here

RAG (Retrieval-Augmented Generation) is a pattern where an AI model answers questions using retrieved context from a knowledge base — not just its training data.

This folder documents RAG pipeline architectures used in the Semantic Database system and other knowledge-intensive flows.

---

## 📂 Structure

```
rag/
├── pipelines/       ← Full RAG pipeline configurations
├── chunking/        ← Text splitting strategies and configs
└── retrieval/       ← Similarity search and ranking logic
```

---

## ⚙️ How RAG Works

```
┌────────────────────┐
│   User Question       │
└────────┬───────────┘
         ↓
┌────────┴───────────┐
│  Question Embedding   │  ← Convert to vector
└────────┬───────────┘
         ↓
┌────────┴───────────┐
│  Vector Search        │  ← Find top-K similar chunks
└────────┬───────────┘
         ↓
┌────────┴───────────┐
│  Context Assembly     │  ← Build prompt with retrieved context
└────────┬───────────┘
         ↓
┌────────┴───────────┐
│  LLM Answer           │  ← GPT generates grounded answer
└────────┬───────────┘
         ↓
┌────────┴───────────┐
│  Answer + Sources     │  ← Delivered to user
└───────────────────┘
```

---

## 🧩 Stack

| Component | Tool |
|-----------|------|
| Embeddings | OpenAI text-embedding-3-small |
| Vector DB | pgvector or Pinecone |
| LLM | OpenAI GPT-4o |
| Orchestration | n8n |

---

## 🧠 Chunking Strategies

| Strategy | Best For |
|----------|----------|
| Fixed-size (512 tokens) | General documents |
| Sentence-based | FAQs, short answers |
| Paragraph-based | Long-form content |
| Semantic chunking | Complex technical docs |

---

*[Back to AI](../README.md) · [Back to Root](../../README.md)*
