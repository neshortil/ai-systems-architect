# 💫 Embeddings

> Vector embedding strategies and configurations for semantic search systems.

---

## What's Here

Embeddings convert text into dense numerical vectors — enabling similarity search, clustering, and semantic retrieval.

This folder documents the embedding strategies used across all systems that require semantic understanding.

---

## 📂 Structure

```
embeddings/
├── models/          ← Model selection and comparison
├── indexing/        ← Vector database indexing configs
└── search/          ← Similarity search strategies
```

---

## ⚙️ How Embeddings Work

```
  Plain Text
      ↓
  Tokenization
      ↓
  Embedding Model (OpenAI / local)
      ↓
  Dense Vector [0.23, -0.87, 0.41, ...]
      ↓
  Stored in Vector Database
      ↓
  Similarity Search (cosine / dot product)
      ↓
  Top-K Most Relevant Results
```

---

## 🧠 Model Comparison

| Model | Dimensions | Best For |
|-------|------------|----------|
| text-embedding-3-small | 1536 | Speed + cost efficiency |
| text-embedding-3-large | 3072 | Maximum accuracy |
| text-embedding-ada-002 | 1536 | Legacy systems |

---

## 🗄️ Vector Database Options

| DB | Type | Best For |
|----|------|----------|
| pgvector | PostgreSQL extension | Self-hosted, SQL-friendly |
| Pinecone | Managed cloud | Scale, production-ready |
| Qdrant | Open source | Self-hosted, high performance |
| Chroma | In-memory / local | Prototyping and dev |

---

## 📊 Similarity Metrics

| Metric | Use Case |
|--------|----------|
| Cosine similarity | Text similarity (most common) |
| Dot product | When vectors are normalized |
| Euclidean distance | Spatial clustering |

---

*[Back to AI](../README.md) · [Back to Root](../../README.md)*
