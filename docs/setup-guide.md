# 🔧 Setup Guide

> How to explore, extend, and build on this repository.

---

## For Clients and Collaborators

This repository is a portfolio and reference system. To work with any of these systems:

1. Browse the system folders in `systems/`
2. Read the README.md inside each system
3. Check the architecture in `docs/architecture.md`
4. Contact via Upwork or GitHub for custom work

---

## For Developers

### Prerequisites

- n8n (self-hosted or cloud)
- Node.js (for custom n8n nodes)
- Python 3.10+ (for FastAPI components)
- PostgreSQL with pgvector (for semantic systems)
- Telegram Bot API token
- OpenAI API key

### Getting Started with the Live System

The Google Lead Generator is fully documented in its own repository:

👉 [github.com/neshortil/google-lead-generator](https://github.com/neshortil/google-lead-generator)

Follow the setup instructions there to:
1. Import the n8n workflow
2. Configure API credentials
3. Set up the Telegram bot
4. Run your first lead generation

---

## Extending Systems

### Adding a New System

1. Create a new folder in `systems/`
2. Add a `README.md` following the existing pattern
3. Design the architecture in `architecture/system-designs/`
4. Export workflows to `workflows/n8n/`
5. Document prompts in `ai/prompts/`

### Adding New Workflows

1. Export workflow JSON from n8n
2. Place in `workflows/n8n/[system-name]/`
3. Document the flow in `workflows/` folder
4. Update the system README

### Adding AI Components

1. Document prompt templates in `ai/prompts/`
2. Save agent configs in `ai/agents/`
3. RAG designs go in `ai/rag/`
4. Embedding strategies in `ai/embeddings/`

---

## Repository Conventions

| Convention | Rule |
|-----------|------|
| Folder names | kebab-case |
| File names | kebab-case.md |
| Commit messages | Action + scope (e.g. "Add systems/new-system README") |
| Status badges | ✅ Live / 🚧 In development |
| Links | Always relative when linking within repo |

---

*[Back to README](../README.md) · [Architecture](./architecture.md) · [System Overview](./system-overview.md)*
