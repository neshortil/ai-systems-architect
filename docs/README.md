# 📚 Docs

> Technical documentation, API references, and setup guides for every system in this repo.

---

## What Lives Here

The `docs/` folder contains reference material that supports building, deploying, and maintaining systems.

- **API references** — endpoints, authentication, rate limits
- **Setup guides** — step-by-step configuration for tools and services
- **Integration notes** — how components connect to each other
- **Environment variables** — required keys and configuration values

---

## Documentation Index

### 🔑 API References

| API | Purpose | Auth Method |
|-----|---------|-------------|
| Google Maps Places API | Business data for lead gen | API Key |
| Instagram Graph API | Profile and post data | OAuth 2.0 |
| YouTube Data API v3 | Video metadata and search | API Key |
| OpenAI API | GPT-4o, embeddings | Bearer Token |
| Supabase | Vector DB + PostgreSQL | Service Role Key |
| Telegram Bot API | Notifications and responses | Bot Token |

### ⚙️ Setup Guides

| Guide | System | Description |
|-------|--------|-------------|
| n8n-cloud-setup.md | All systems | Configure n8n cloud instance |
| google-credentials.md | Lead gen systems | Google API + Sheets setup |
| openai-setup.md | AI systems | OpenAI key + model config |
| supabase-setup.md | Semantic DB | Database and vector setup |
| telegram-bot.md | Notification systems | Create and configure a Telegram bot |

### 🔗 Integration Notes

| Integration | Systems Involved | Notes |
|------------|-----------------|-------|
| n8n → Google Sheets | Lead generators | OAuth2 credential required |
| n8n → OpenAI | AI workflows | Use HTTP Request node |
| n8n → Supabase | Semantic DB | REST API or Supabase node |
| n8n → Telegram | Notification system | Telegram Trigger + Send Message |

---

## Environment Variables Reference

```env
# Google APIs
GOOGLE_MAPS_API_KEY=
GOOGLE_SHEETS_CLIENT_ID=
GOOGLE_SHEETS_CLIENT_SECRET=

# OpenAI
OPENAI_API_KEY=

# Supabase
SUPABASE_URL=
SUPABASE_SERVICE_ROLE_KEY=

# Telegram
TELEGRAM_BOT_TOKEN=
TELEGRAM_CHAT_ID=

# n8n
N8N_WEBHOOK_URL=
```

---

## Related

- [Stack](../STACK.md) — full technology stack overview
- [Systems](../systems/) — production systems that use these APIs
- [Architecture](../architecture/) — system design documents
