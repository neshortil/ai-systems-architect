# 📐 Diagrams

> Exported diagram images referenced across README files and documentation.

---

## What Lives Here

This folder stores all **exported diagram files** — PNG, SVG, and GIF images that visualize system architecture, data flows, and component relationships.

These are the rendered outputs of diagrams created in `architecture/diagrams/`.

---

## Folder Contents

```
assets/diagrams/
├── google-lead-generator-flow.png
├── instagram-lead-generator-flow.png
├── youtube-trending-search-flow.png
├── semantic-db-architecture.svg
└── [system-name]-[type].[ext]
```

---

## File Naming Convention

```
[system-name]-[diagram-type].[ext]

Types:
- flow       ← Data flow diagram
- arch       ← Architecture overview
- sequence   ← Sequence / interaction diagram
- overview   ← High-level summary

Extensions:
- .png   ← Standard raster (default)
- .svg   ← Scalable vector (preferred for docs)
- .gif   ← Animated flow walkthroughs
```

---

## How Diagrams Are Used

Diagrams from this folder are embedded in:

| Referenced In | Example |
|--------------|---------|
| `architecture/diagrams/README.md` | Flow and architecture overviews |
| `architecture/system-designs/*.md` | Per-system blueprints |
| `systems/*/README.md` | System-level documentation |
| Root `README.md` | Visual overview section |

---

## Related

- [Architecture Diagrams](../../architecture/diagrams/) — source diagram docs
- [Screenshots](../screenshots/) — UI and output screenshots
- [Architecture Patterns](../../architecture/patterns/) — patterns these diagrams illustrate
