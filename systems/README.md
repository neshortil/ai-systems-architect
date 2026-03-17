# ⚙️ Systems

> Production-ready automation systems built on n8n, AI APIs, and modern data pipelines.

---

## What Lives Here

Each subfolder is a standalone, deployable system with:

- Complete n8n workflow JSON
- Environment variable reference
- Setup and deployment guide
- Architecture diagram link

---

## Live Systems

| System | Status | Category | Design Doc |
|--------|--------|----------|------------|
| Google Lead Generator | ✅ Live | Lead Gen | [Design](../architecture/system-designs/) |
| Instagram Lead Generator | ✅ Live | Lead Gen | [Design](../architecture/system-designs/) |
| YouTube Trending Search | ✅ Live | Research | [Design](../architecture/system-designs/) |
| Semantic DB + Telegram | ✅ Live | AI Memory | [Design](../architecture/system-designs/) |

---

## System Categories

### 🎯 Lead Generation
Systems that find, qualify, and deliver leads automatically.
- Input: platform, keywords, filters
- Output: enriched contact data → Google Sheets / Telegram

### 🤖 AI Agents
Systems that reason, retrieve, and respond autonomously.
- Input: user query or trigger
- Output: structured response, action, or stored memory

### 📊 Data Pipelines
Systems that collect, transform, and store structured data.
- Input: API / scraper sources
- Output: clean database records or spreadsheets

---

## How to Deploy Any System

1. Read the system's own `README.md`
2. Import the `.json` workflow into n8n
3. Set required environment variables
4. Activate and test

---

## Related

- [Architecture Designs](../architecture/system-designs/)
- [Workflows](../workflows/)
- [AI Modules](../ai/)
