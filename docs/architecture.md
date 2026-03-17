# 🏗️ System Architecture

> How AI systems are designed in this repository.

---

## Design Philosophy

Every system follows the same architectural principles:

1. **Input layer** — Define what triggers the system and what data comes in
2. **Processing layer** — Transform, enrich, and analyze data
3. **AI layer** — Apply intelligence at the right stage
4. **Output layer** — Deliver results to the right destination
5. **Control layer** — Interface for managing and monitoring the system

---

## Core Patterns

### Pattern 1: Trigger → Collect → Enrich → Act

Used in: Google Lead Generator, Instagram Lead Generator

```
Trigger (Telegram / Schedule)
    ↓
Data Collection (API / Scraping)
    ↓
Data Enrichment (Extraction / AI)
    ↓
Action (Email / Export / Notification)
```

### Pattern 2: Monitor → Analyze → Report

Used in: YouTube Trending Search

```
Scheduled Monitor (API polling)
    ↓
Data Analysis (Metrics / Scoring)
    ↓
AI Pattern Extraction
    ↓
Report Delivery
```

### Pattern 3: Ingest → Embed → Retrieve → Answer

Used in: Semantic Database with Telegram UI

```
Data Ingestion (Documents / URLs)
    ↓
Embedding Pipeline (Chunks + Vectors)
    ↓
Vector Storage (pgvector / Pinecone)
    ↓
Semantic Retrieval (Similarity Search)
    ↓
RAG Answer Generation (GPT)
```

---

## Technology Stack Overview

```
┌─────────────────────────────────────┐
│         INTERFACE LAYER                  │
│   Telegram Bot  /  Webhooks              │
└───────────────┬─────────────────────┘
                 ↓
┌───────────────┴─────────────────────┐
│       ORCHESTRATION LAYER                │
│              n8n                         │
└───────────────┬─────────────────────┘
                 ↓
┌───────────────┴─────────────────────┐
│         AI LAYER                         │
│  OpenAI GPT  /  Claude  /  Embeddings   │
└───────────────┬─────────────────────┘
                 ↓
┌───────────────┴─────────────────────┐
│           DATA LAYER                     │
│  PostgreSQL  /  Sheets  /  Pinecone     │
└─────────────────────────────────────┘
```

---

*[Back to README](../README.md) · [System Overview](./system-overview.md)*
