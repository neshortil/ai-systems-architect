# 💬 Prompts

> Prompt templates and engineering patterns used across all AI systems.

---

## What's Here

This folder contains all prompt templates used in production systems — structured, versioned, and ready to reuse.

Good prompts are not random text. They are engineered instructions with clear input/output contracts.

---

## 📂 Structure

```
prompts/
├── lead-generation/     ← Prompts for email generation and lead qualification
├── classification/      ← Category and intent classification prompts
├── extraction/          ← Structured data extraction from unstructured text
└── summarization/       ← Content and report summarization templates
```

---

## ⚙️ Prompt Engineering Principles

1. **Role definition** — Always define who the AI is and what context it operates in
2. **Clear input format** — Specify exactly what data the prompt receives
3. **Strict output format** — Define the expected JSON or text structure
4. **Few-shot examples** — Include 1–3 examples for complex tasks
5. **Edge case handling** — Instruct what to do when data is missing or ambiguous

---

## 📝 Prompt Template Format

Every prompt in this folder follows this structure:

```
## Purpose
What this prompt does

## Input
What data is passed in

## Output
Expected format of the result

## Prompt
[The actual prompt text]

## Notes
Edge cases, known limitations, version history
```

---

## 🌍 Used In

| System | Prompt Type |
|--------|-------------|
| Google Lead Generator | Email generation, lead qualification |
| Instagram Lead Generator | Profile scoring, DM personalization |
| YouTube Trending Search | Topic extraction, trend summarization |
| Semantic DB + Telegram | RAG answer generation |

---

*[Back to AI](../README.md) · [Back to Root](../../README.md)*
