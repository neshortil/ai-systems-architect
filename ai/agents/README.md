# 🤖 Agents

> AI agent configurations, logic flows, and autonomous decision systems.

---

## What's Here

AI agents are systems that take a goal, break it into steps, and execute them autonomously — making decisions along the way without human input at each stage.

This folder documents how agents are structured and configured in each system.

---

## 📂 Structure

```
agents/
├── lead-agent/          ← Lead generation and outreach agent
├── research-agent/      ← Data research and enrichment agent
└── qa-agent/            ← Quality assurance and validation agent
```

---

## ⚙️ Agent Design Pattern

Every agent in this repository follows the same structure:

```
┌─────────────────────┐
│    Goal Definition     │  ← What the agent must achieve
└────────┬───────────┘
         ↓
┌────────┴───────────┐
│    Tool Selection     │  ← Which tools/APIs are available
└────────┬───────────┘
         ↓
┌────────┴───────────┐
│   Step Execution     │  ← Sequential or parallel actions
└────────┬───────────┘
         ↓
┌────────┴───────────┐
│  Output + Handoff    │  ← Structured result passed downstream
└───────────────────┘
```

---

## 🧠 AI Stack for Agents

| Component | Tool |
|-----------|------|
| Reasoning | OpenAI GPT-4o |
| Orchestration | n8n workflow engine |
| Memory | Context window + structured state |
| Tools | REST APIs, scraping, databases |

---

## 🌍 Used In

| System | Agent Role |
|--------|------------|
| Google Lead Generator | Lead discovery + outreach agent |
| Instagram Lead Generator | Profile qualification agent |
| Semantic DB + Telegram | RAG retrieval + answer agent |

---

*[Back to AI](../README.md) · [Back to Root](../../README.md)*
