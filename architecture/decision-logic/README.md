# 🧭 Decision Logic

> Decision trees, routing rules, and conditional logic that drive system behavior.

---

## What Lives Here

This folder documents the **"why"** behind system decisions — how systems choose what to do next based on data, conditions, and context.

Each file maps a specific decision point in a system to the rules that govern it.

---

## What Is Decision Logic?

Decision logic defines:

- **Routing** — which path a workflow takes based on input
- **Filtering** — what data gets processed or discarded
- **Scoring** — how leads, content, or records are ranked
- **Fallbacks** — what happens when conditions aren't met
- **Branching** — conditional flows based on API responses or data values

---

## Decision Logic Index

### 🎯 Lead Qualification Logic
Rules for deciding if a lead is worth processing.

| Rule | Condition | Outcome |
|------|-----------|---------|
| Has phone | Phone field not empty | Include in output |
| Has email | Email field not empty | Priority lead |
| Has website | Website field not empty | Business verified |
| Rating filter | Rating ≥ 4.0 | High-quality lead |
| Review count | Reviews ≥ 10 | Established business |

### 🔀 Routing Logic
Rules for directing data to different outputs.

| Condition | Route |
|-----------|-------|
| Lead has email | → Email outreach queue |
| Lead has phone only | → Call list sheet |
| Lead is duplicate | → Skip / discard |
| Lead score ≥ 8 | → Priority Telegram alert |

### 🤖 AI Decision Points
Where AI models make decisions in workflows.

| Step | Model | Decision |
|------|-------|---------|
| Content relevance check | GPT-4o | Is this content worth summarizing? |
| Lead classification | GPT-4o | B2B or B2C? Industry category? |
| Query routing | GPT-4o | Which knowledge base to query? |

---

## How to Read Decision Logic Docs

Each decision logic file follows this structure:

```
# Decision: [Name]
System: [Which system uses this]
Trigger: [What initiates the decision]
Input: [What data is evaluated]
Rules: [List of conditions and outcomes]
Fallback: [Default if no condition matches]
```

---

## Related

- [System Designs](../system-designs/) — systems that implement this logic
- [Diagrams](../diagrams/) — visual representations of decision flows
- [Patterns](../patterns/) — reusable patterns built on this logic
