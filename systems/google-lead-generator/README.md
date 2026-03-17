# 🌍 Google Lead Generation System

**Status:** ✅ Live

👉 **[View Full Repository](https://github.com/neshortil/google-lead-generator)**

---

## Overview

An AI-powered lead generation system that automatically discovers, enriches, and reaches out to business leads using Google Maps — fully automated and controlled via Telegram.

This is not a script. It's a system.

---

## 🎯 Problem It Solves

Manual lead generation is:
- Time-consuming — hours per day per person
- Inconsistent — data quality depends on the human
- Unscalable — limited by available work hours
- Expensive — requires dedicated staff

This system replaces the entire manual process with an automated pipeline.

---

## ⚙️ System Architecture

```
┌────────────────────────┐
│   Telegram Bot (Input)   │  ← User sends: niche + location
└───────────┬───────────┘
                ↓
┌───────────┴───────────┐
│   n8n Workflow Engine    │  ← Orchestrates all steps
└───────────┬───────────┘
                ↓
┌───────────┴───────────┐
│  Google Maps API        │  ← Business discovery
└───────────┬───────────┘
                ↓
┌───────────┴───────────┐
│  Data Enrichment Layer  │  ← Contact extraction
└───────────┬───────────┘
                ↓
┌───────────┴───────────┐
│  OpenAI GPT             │  ← Email generation
└───────────┬───────────┘
                ↓
┌───────────┴───────────┐
│  Email Delivery         │  ← Automated outreach
└───────────┬───────────┘
                ↓
┌───────────┴───────────┐
│  Telegram Bot (Output)  │  ← Results delivered
└───────────────────────┘
```

---

## 🔄 System Flow

1. **Input** — User sends target niche and city to Telegram bot
2. **Discovery** — System queries Google Maps API for matching businesses
3. **Extraction** — Business names, addresses, phones, websites collected
4. **Enrichment** — Website scraping for email addresses and contact info
5. **AI Generation** — OpenAI generates personalized outreach email per lead
6. **Delivery** — Emails sent via configured SMTP or email API
7. **Report** — Results and stats delivered back to Telegram

---

## 📊 Value Delivered

| Metric | Before | After |
|--------|--------|-------|
| Time per 100 leads | 4–6 hours | 5–10 minutes |
| Manual work | 100% | 0% |
| Email personalization | Generic | AI-personalized |
| Scalability | Limited by time | On-demand |
| Cost per lead | High | Near zero |

---

## 🧩 Stack

| Component | Technology |
|-----------|------------|
| Workflow Engine | n8n |
| Business Data | Google Maps API |
| AI / Email Generation | OpenAI GPT |
| User Interface | Telegram Bot API |
| Email Delivery | SMTP / Email API |

---

## 🔗 Links

- **Full Repository:** [github.com/neshortil/google-lead-generator](https://github.com/neshortil/google-lead-generator)
- **Portfolio:** [../../PORTFOLIO.md](../../PORTFOLIO.md)
- **Stack:** [../../STACK.md](../../STACK.md)

---

*Part of the [AI Systems Architect](https://github.com/neshortil/ai-systems-architect) portfolio*
