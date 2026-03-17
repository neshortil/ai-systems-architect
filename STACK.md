# ⚙️ Stack

> Every tool in this stack is here for a reason. No bloat. No trends for the sake of it.

---

## ⚙️ Automation Layer

### n8n
**Why:** Visual workflow engine that connects any API, handles branching logic, and runs 24/7 without custom infrastructure.

n8n is the backbone of every system I build. It provides:
- Visual pipeline design — fast to build, easy to audit
- Native integrations with 400+ services
- Webhook-based triggers for real-time automation
- Self-hostable — full data control
- Extensible with custom JavaScript nodes

```
Use cases: lead pipelines, data enrichment, AI orchestration,
notification systems, scheduled jobs, API bridges
```

---

## 🧠 AI Layer

### OpenAI (GPT-4 / GPT-4o)
**Why:** Best-in-class language model for generation, classification, extraction, and structured output.

- Email generation with context-aware personalization
- Data classification and qualification scoring
- Structured JSON extraction from unstructured text
- Prompt chaining for multi-step reasoning

### Anthropic Claude
**Why:** Superior performance on long-context tasks, document analysis, and complex instruction-following.

- Large document processing
- Complex multi-step agent logic
- High-quality summarization pipelines

### OpenAI Embeddings (text-embedding-3)
**Why:** Converts text to dense vectors for semantic search and similarity matching.

- Semantic knowledge base indexing
- Similarity-based lead matching
- RAG (Retrieval-Augmented Generation) pipelines

---

## 🔗 API & Integration Layer

### REST APIs
**Why:** Universal interface for connecting any modern service.
- Google Maps API — business discovery and data
- YouTube Data API v3 — content and trending analysis
- Telegram Bot API — user interfaces and notifications
- Any CRM, email, or data platform

### Webhooks
**Why:** Event-driven triggers that start workflows instantly without polling.
- Real-time pipeline activation
- Cross-system event propagation
- Form submissions, payment events, user actions

---

## 🗄️ Data Layer

### PostgreSQL + pgvector
**Why:** Relational data storage with native vector extension for semantic search.
- Structured lead and contact storage
- Vector embeddings for RAG systems
- Query performance at scale

### Google Sheets
**Why:** Accessible, shareable output layer for non-technical stakeholders.
- Lead delivery and review
- Lightweight data pipelines
- Client-facing outputs

### Airtable
**Why:** Structured database with CRM-like interface for more complex data management.
- Lead management pipelines
- Content calendars
- Project tracking

### Pinecone
**Why:** Managed vector database optimized for high-performance semantic search at scale.
- Production RAG systems
- Large-scale similarity search

---

## 🚀 Backend Layer

### FastAPI (Python)
**Why:** Lightweight, fast API framework for custom endpoints and system extensions.
- Custom webhook receivers
- Data preprocessing pipelines
- API bridges between systems

### n8n Cloud / Self-hosted
**Why:** Managed infrastructure for workflow execution without DevOps overhead.
- Always-on automation execution
- Scalable worker capacity
- Built-in monitoring and error logging

---

## 💬 Interfaces

### Telegram Bot API
**Why:** Universal control interface that works on any device, requires no frontend development, and is familiar to most users.

- System control (start/stop/configure)
- Result delivery
- Status notifications
- Human-in-the-loop approval flows

---

## 📊 Stack Summary

| Layer | Tool | Role |
|-------|------|------|
| Automation | n8n | Workflow orchestration |
| AI | OpenAI / Claude | Generation, extraction, reasoning |
| Embeddings | OpenAI text-embedding | Semantic search |
| APIs | REST / Webhooks | Service integration |
| Data | PostgreSQL / Sheets | Storage and output |
| Vector DB | pgvector / Pinecone | Semantic retrieval |
| Backend | FastAPI | Custom logic |
| Interface | Telegram Bot | User control layer |

---

*[Back to README](./README.md) · [Portfolio](./PORTFOLIO.md)*
