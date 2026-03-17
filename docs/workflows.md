# ⚡ Workflows

> How automation logic is structured in this repository.

---

## Workflow Design Principles

1. **Single responsibility** — Each workflow does one thing well
2. **Error handling** — Every step has failure logic
3. **Observability** — Logging and notifications built in
4. **Modularity** — Workflows can be connected as building blocks
5. **Testability** — Each step can be tested independently

---

## Workflow Types

### 🟢 Trigger-Based Workflows
Activated by external events (Telegram commands, webhooks, form submissions).

```
External Trigger
    ↓
Input Validation
    ↓
Core Processing
    ↓
Output + Notification
```

### 🟡 Scheduled Workflows
Run on a defined schedule (hourly, daily, weekly).

```
Cron Trigger
    ↓
Data Fetch
    ↓
Processing
    ↓
Report Delivery
```

### 🔵 Pipeline Workflows
Multi-step data processing with enrichment and AI.

```
Data Input
    ↓
Step 1: Collection
    ↓
Step 2: Enrichment
    ↓
Step 3: AI Processing
    ↓
Step 4: Output
```

---

## n8n Workflow Patterns

### Error Handling
All workflows include:
- Try/catch logic at each critical node
- Fallback paths for API failures
- Error notifications via Telegram

### Data Flow
- Data passed as JSON between nodes
- Consistent field naming conventions
- Structured output format for every system

---

## Workflow Index

| Workflow | System | Status |
|----------|--------|--------|
| Google Maps Lead Scraper | google-lead-generator | ✅ Live |
| Lead Enrichment Pipeline | google-lead-generator | ✅ Live |
| AI Email Generator | google-lead-generator | ✅ Live |
| Instagram Profile Collector | instagram-lead-generator | 🚧 Planned |
| YouTube Trend Detector | youtube-trending-search | 🚧 Planned |
| Semantic Indexing Pipeline | semantic-database-telegram | 🚧 Planned |

---

*[Back to README](../README.md) · [Architecture](./architecture.md)*
