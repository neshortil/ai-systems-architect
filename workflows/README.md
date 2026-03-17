# 🔄 Workflows

> Reusable n8n workflow modules — building blocks for every system in this repo.

---

## What Lives Here

This folder contains modular n8n workflows organized by function. Each workflow is:

- **Importable** — drop the JSON into any n8n instance
- **Documented** — inline notes explain every node
- **Composable** — designed to connect with other workflows

---

## Workflow Categories

### 🔍 Scrapers
Data extraction workflows for Google Maps, Instagram, YouTube, and more.

| Workflow | Source | Output |
|----------|--------|--------|
| google-maps-scraper | Google Maps API | Business leads |
| instagram-profile-scraper | Instagram Graph API | Profile data |
| youtube-search | YouTube Data API | Video metadata |

### 📤 Enrichment
Workflows that clean, score, and enhance raw data.

| Workflow | Input | Output |
|----------|-------|--------|
| lead-scorer | Raw lead data | Scored + tagged leads |
| email-validator | Email list | Verified emails |

### 🤖 AI Processing
Workflows that use LLMs to analyze or generate content.

| Workflow | Model | Purpose |
|----------|-------|---------|
| ai-summarizer | GPT-4o | Summarize scraped content |
| semantic-embedder | text-embedding-3-small | Embed text for vector DB |

### 📨 Delivery
Workflows that send results to the right destination.

| Workflow | Destination | Trigger |
|----------|------------|---------|
| sheets-writer | Google Sheets | On data ready |
| telegram-notifier | Telegram Bot | On new lead or event |

---

## How to Use

1. Open n8n
2. Click **Import Workflow**
3. Paste or upload the `.json` file
4. Configure credentials
5. Activate

---

## Related

- [Systems](../systems/) — full systems that use these workflows
- [AI Modules](../ai/) — AI utilities used inside workflows
- [Docs](../docs/) — API references and setup guides
