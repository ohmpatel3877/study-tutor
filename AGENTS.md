# study-tutor — Agent Instructions

Adaptive exam prep PWA with SM-2 spaced repetition and AcademyGraph knowledge graph. Built as a single-page app (no build step — pure HTML/JS/CSS).

> **This file is for OpenCode agents.** Every line answers: "Would an agent likely miss this without help?"

---

## What It Is

- **PWA** — installable, works offline via service worker (`service-worker.js`)
- **SM-2 spaced repetition** — algorithm from SuperMemo-2, implemented in `tutor.html`
- **AcademyGraph** — interactive knowledge graph visualization (`academy-graph.js` + `academy-data.js`) showing topic interconnections
- **Zero build step** — no bundler, no framework, no npm. Directly openable in browser.

## Key Files

| File | Purpose |
|------|---------|
| `tutor.html` | Main SM-2 flashcard tutor UI |
| `tutor-academy.html` | AcademyGraph explorer UI |
| `academy-graph.js` | Knowledge graph rendering engine |
| `academy-data.js` | Graph nodes/edges data |
| `histo-cytology-exam-prep.html` | Subject-specific prep module |
| `index.html` | Landing / entry page |
| `manifest.json` | PWA manifest (icons, theme, display) |
| `service-worker.js` | Offline cache worker |

## Deployment

- **GitHub Pages**: https://ohmpatel3877.github.io/study-tutor/
- Served from `docs/` or root — confirm current GH Pages source config.
- To deploy: push to `main` branch, GH Pages auto-deploys from configured source.

## Related Repositories

| Repo | Description | URL |
|------|-------------|-----|
| StudySpace | Tauri 2 + React 19 desktop study workspace | github.com/ohmpatel3877/StudySpace |
| ai-memory-core | Python 68-tool MCP server (BM25 memory, skill router, trace system) | github.com/ohmpatel3877/ai-memory-core |
| agent-memory-mcp | TypeScript MCP memory server (LanceDB, cortical architecture, KG) | github.com/ohmpatel3877/agent-memory-mcp |
| wshobson-agents | Multi-harness agentic plugin marketplace | github.com/ohmpatel3877/wshobson-agents |
| opencad | CAD collaboration pnpm monorepo | github.com/ohmpatel3877/opencad |
