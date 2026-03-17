# 🧠 AI

> Prompts, agents, RAG pipelines, and embedding strategies powering every system in this repo.

---

## What Lives Here

The `ai/` folder is the intelligence layer of this repository. It contains:

- **Prompts** — engineered templates for lead gen, classification, summarization
- **Agents** — autonomous AI agent configurations and logic flows
- **RAG** — Retrieval-Augmented Generation pipeline designs
- **Embeddings** — vector embedding strategies and search configs

---

## Folder Structure

```
ai/
├── prompts/       ← Prompt templates and engineering patterns
├── agents/        ← AI agent configurations and logic
├── rag/           ← RAG pipeline designs
└── embeddings/    ← Embedding strategies and vector search configs
```

---

## AI Modules in Use

### 🗣️ Prompts
Carefully engineered prompts used across systems.

| Prompt | Use Case | Model |
|--------|----------|-------|
| lead-qualifier | Score and classify incoming leads | GPT-4o |
| email-writer | Generate personalized outreach emails | GPT-4o |
| content-summarizer | Summarize YouTube / web content | GPT-4o mini |
| intent-detector | Detect user intent from messages | GPT-4o |

### 🤖 Agents
Autonomous agents that execute multi-step tasks.

| Agent | Capability | Trigger |
|-------|-----------|---------|
| lead-research-agent | Research company + contact info | On new lead |
| content-agent | Find + summarize trending content | On schedule |
| qa-agent | Answer questions from knowledge base | On message |

### 🔍 RAG Pipelines
Systems that retrieve context before generating responses.

| Pipeline | Data Source | Vector DB |
|---------|------------|-----------|
| knowledge-base-rag | Notion / docs | Supabase pgvector |
| lead-context-rag | CRM + history | Supabase pgvector |

### 📐 Embeddings
Strategies for turning text into searchable vectors.

| Strategy | Model | Purpose |
|---------|-------|---------|
| semantic-search | text-embedding-3-small | Find similar leads |
| content-indexing | text-embedding-3-small | Index scraped content |

---

## Related

- [Systems](../systems/) — systems powered by these AI modules
- [Workflows](../workflows/) — n8n workflows that call these AI modules
- [Architecture](../architecture/) — system design documents
