# 🧩 Patterns

> Reusable design patterns for building AI automation systems — battle-tested blueprints you can apply to any project.

---

## What Lives Here

This folder contains documented **architectural patterns** — recurring structures that appear across multiple systems in this repo.

Each pattern is:
- **Named** — a clear, memorable identifier
- **Described** — what it does and why it works
- **Diagrammed** — linked to a visual representation
- **Instantiated** — shown in at least one real system

---

## Pattern Catalog

### 🔁 Trigger → Scrape → Enrich → Deliver
The core pattern for all lead generation systems.

```
[Schedule / Webhook]
        ↓
[Scraper Node — Google Maps / Instagram / YouTube]
        ↓
[Filter & Deduplicate]
        ↓
[AI Enrichment — GPT-4o classification]
        ↓
[Delivery — Google Sheets + Telegram]
```

**Used in:** Google Lead Generator, Instagram Lead Generator

---

### 🧠 Query → Embed → Search → Respond
The core RAG (Retrieval-Augmented Generation) pattern.

```
[User Query — Telegram / Webhook]
        ↓
[Embed Query — text-embedding-3-small]
        ↓
[Vector Search — Supabase pgvector]
        ↓
[Retrieve Top-K Context Chunks]
        ↓
[GPT-4o — Generate Response with Context]
        ↓
[Deliver Response — Telegram Bot]
```

**Used in:** Semantic DB + Telegram

---

### 📥 Ingest → Chunk → Embed → Store
The data ingestion pattern for building knowledge bases.

```
[Source Data — Notion / Docs / Web]
        ↓
[Split into Chunks — 500-1000 tokens]
        ↓
[Embed Each Chunk — text-embedding-3-small]
        ↓
[Store in Vector DB — Supabase pgvector]
```

**Used in:** Semantic DB ingestion pipeline

---

### 🔔 Monitor → Detect → Alert
The event-detection and notification pattern.

```
[Scheduled Check — every N minutes]
        ↓
[Fetch Latest Data — API / Scraper]
        ↓
[Compare with Previous State]
        ↓
[If Changed → Format Alert]
        ↓
[Send to Telegram / Sheets]
```

**Used in:** YouTube Trending Search

---

## How to Apply a Pattern

1. Pick the pattern closest to your use case
2. Read the linked system design for a full implementation example
3. Import the workflow JSON from `systems/` or `workflows/`
4. Adapt node configs to your specific API keys and data structure

---

## Related

- [System Designs](../system-designs/) — full systems built on these patterns
- [Decision Logic](../decision-logic/) — logic layers within each pattern
- [Diagrams](../diagrams/) — visual representations of each pattern
