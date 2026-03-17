# 📊 Diagrams

> Flow diagrams, architecture maps, and visual representations of every system in this repo.

---

## What Lives Here

This folder contains all visual diagrams that explain how systems are structured and how data flows through them.

Each diagram corresponds to a system or component documented in `system-designs/`.

---

## Diagram Types

### 🔄 Data Flow Diagrams
Show how data moves from source to destination through each system.

- Input → Processing → Output
- API calls, transformations, and storage steps
- Error paths and fallback flows

### 🏛️ Architecture Diagrams
High-level structural view of how components connect.

- n8n nodes and connections
- External APIs and services
- Databases and storage layers

### 🔁 Sequence Diagrams
Step-by-step interaction between system components.

- Trigger → Action → Response chains
- Multi-service coordination flows
- Async and parallel execution paths

---

## Naming Convention

```
[system-name]-[diagram-type].[ext]

Examples:
google-lead-generator-flow.png
semantic-db-architecture.svg
youtube-search-sequence.png
```

---

## Tools Used

- **draw.io** — architecture and flow diagrams
- **Mermaid** — embedded diagrams in markdown
- **Lucidchart** — complex multi-system diagrams
- **Excalidraw** — quick sketches and wireframes

---

## Diagrams Index

| Diagram | System | Type | Format |
|---------|--------|------|--------|
| google-lead-generator-flow | Google Lead Generator | Data Flow | PNG |
| instagram-lead-generator-flow | Instagram Lead Generator | Data Flow | PNG |
| youtube-trending-search-flow | YouTube Trending Search | Data Flow | PNG |
| semantic-db-architecture | Semantic DB + Telegram | Architecture | SVG |

---

## Related

- [System Designs](../system-designs/) — blueprints these diagrams illustrate
- [Decision Logic](../decision-logic/) — logic trees referenced in diagrams
- [Assets/Diagrams](../../assets/diagrams/) — exported diagram images
