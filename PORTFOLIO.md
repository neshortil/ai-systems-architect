# 📂 Portfolio

> Systems I have designed and built. Each one is a product, not a project.

---

## 1. 🌍 Google Lead Generation System

**Status:** ✅ Live

👉 **[github.com/neshortil/google-lead-generator](https://github.com/neshortil/google-lead-generator)**

### Problem
Businesses spend hours manually searching for leads, copying data, writing outreach emails — a completely manual, unscalable process.

### Solution
A fully automated system that finds businesses on Google Maps, enriches contact data, generates personalized AI emails, and sends outreach — all triggered from a Telegram bot.

### Architecture
```
Telegram Bot (Input)
    ↓
n8n Workflow Engine
    ↓
Google Maps API → Lead Extraction
    ↓
Data Enrichment Layer
    ↓
OpenAI → Email Generation
    ↓
Email Delivery Module
    ↓
Telegram Bot (Results)
```

### Stack
- **Automation:** n8n
- **Data Source:** Google Maps API
- **AI:** OpenAI GPT
- **Interface:** Telegram Bot API
- **Delivery:** SMTP / Email API

### Value Delivered
- ⏱️ Reduces lead gen time from hours to minutes
- 🤖 Fully automated — zero manual work after setup
- 📈 Scalable to any niche or location
- 🎯 Personalized outreach at scale

---

## 2. 📸 Instagram Lead Generator

**Status:** 🚧 System in development

### Problem
Manually finding and qualifying Instagram profiles for B2C outreach is time-consuming and inconsistent.

### Solution
Automated Instagram profile discovery, enrichment, and structured outreach pipeline.

### Architecture (Designed)
```
Search Parameters (Input)
    ↓
Instagram Data Layer
    ↓
Profile Enrichment
    ↓
Qualification Filter (AI)
    ↓
Structured Output / CRM Export
```

### Stack (Planned)
- **Automation:** n8n
- **Data Layer:** Instagram scraping API
- **AI:** OpenAI for qualification
- **Output:** Google Sheets / Airtable

> Architecture designed. Implementation coming soon.

---

## 3. 📈 YouTube Trending Search System

**Status:** 🚧 System in development

### Problem
Content creators and marketers struggle to identify trending topics before they peak. Manual research is slow and inconsistent.

### Solution
Automated system that monitors YouTube for trending signals, extracts keyword patterns, and surfaces actionable content opportunities.

### Architecture (Designed)
```
Search Parameters (Input)
    ↓
YouTube Data API v3
    ↓
Trend Analysis Engine
    ↓
AI Pattern Extraction
    ↓
Structured Report Output
    ↓
Delivery (Telegram / Email)
```

### Stack (Planned)
- **Automation:** n8n
- **Data Source:** YouTube Data API v3
- **AI:** OpenAI for pattern analysis
- **Output:** Telegram report / Google Sheets

> Architecture designed. Implementation coming soon.

---

## 4. 🧠 Semantic Database with Telegram UI

**Status:** 🚧 System in development

### Problem
Teams accumulate unstructured data across docs, notes, and chats. Retrieval is manual, slow, and keyword-dependent.

### Solution
A semantic knowledge base with vector search, accessible through a conversational Telegram interface. Ask questions in natural language — get precise answers from your own data.

### Architecture (Designed)
```
Data Ingestion (docs / text / URLs)
    ↓
Chunking + Embedding Layer
    ↓
Vector Database (pgvector / Pinecone)
    ↓
Semantic Retrieval Engine
    ↓
AI Answer Generation
    ↓
Telegram Bot Interface
```

### Stack (Planned)
- **Automation:** n8n
- **Embeddings:** OpenAI text-embedding
- **Vector DB:** pgvector or Pinecone
- **AI:** OpenAI GPT (RAG)
- **Interface:** Telegram Bot API

> Architecture designed. Implementation coming soon.

---

## 📊 Summary

| System | Status | Core Tech |
|--------|--------|-----------|
| 🌍 Google Lead Generator | ✅ Live | n8n + Google Maps + OpenAI |
| 📸 Instagram Lead Generator | 🚧 Dev | n8n + Scraping + OpenAI |
| 📈 YouTube Trending Search | 🚧 Dev | n8n + YouTube API + OpenAI |
| 🧠 Semantic DB + Telegram | 🚧 Dev | n8n + pgvector + OpenAI |

---

*[Back to README](./README.md) · [Services](./SERVICES.md) · [Stack](./STACK.md)*
