<!--
SEO: vector db live tracker
-->

<div align="center">

# Vector DB Live Tracker

Live-updating landscape of vector database projects, integrations, and benchmarks — refreshed every 15 minutes

[![Stars](https://img.shields.io/github/stars/linny006/vector-db-live?style=for-the-badge&logo=github)](https://github.com/linny006/vector-db-live/stargazers)
[![Last Commit](https://img.shields.io/github/last-commit/linny006/vector-db-live?style=for-the-badge)](https://github.com/linny006/vector-db-live/commits)
[![Items](https://img.shields.io/badge/Tracked_Items-10-brightgreen?style=for-the-badge)](#)
[![Updated](https://img.shields.io/badge/Updates-every_15min-blue?style=for-the-badge)](#)

**⭐ Star this repo to bookmark — fresh data every 15 minutes**

[English](./README.md) · [中文](./README_CN.md) · [日本語](./README_JA.md) · [한국어](./README_KO.md) · [Español](./README_ES.md) · [Português](./README_PT.md)

</div>

---

## 💡 What is this?

Automatically tracks and compares the vector database ecosystem by pulling live data from GitHub, package registries, and release feeds. Generates a structured, always-current comparison table covering maturity, integrations, language support, and recent activity for projects like pgvector, Qdrant, Chroma, Weaviate, and Milvus.

This list is **auto-updated every 15 minutes** by a GitHub Actions cron.
Each commit reflects a real change in the upstream data source — new items added,
expired items removed — so you can rely on what you see being current.

---

## 📋 Current Items

> ⏰ Last updated: 2026-10-27 07:30 UTC
>
> Data source: `GitHub Search API`
>
> The table below is rewritten on every cron tick. Star the repo to bookmark.

<!-- TRACKER_TABLE_START -->
| # | Name | ⭐ | Lang | Updated | Description |
|---|------|---|------|---------|-------------|
| 1 | [makr-code/ThemisDB](https://github.com/makr-code/ThemisDB) | 9 | C++ | 2026-10-27 | Themis Database System - High-performance C++ hybrid-database (graph-vector-relational-file) with AQL support and MVCC.  |
| 2 | [databendlabs/databend](https://github.com/databendlabs/databend) | 9482 | Rust | 2026-10-27 | Data Agent Ready Warehouse : One for  Analytics, Search, AI, Python Sandbox.  — rebuilt from scratch. Unified architectu |
| 3 | [maximilien/weave-cli](https://github.com/maximilien/weave-cli) | 35 | Go | 2026-10-27 | A universal CLI for Weaviate, Milvus, Chroma, Qdrant, and other vector DBs to help view, list, create, delete, and searc |
| 4 | [infino-ai/infino](https://github.com/infino-ai/infino) | 138 | Rust | 2026-10-27 | Embedded retrieval library built on Parquet. Fast, efficient, and scalable. |
| 5 | [alibaba/zvec](https://github.com/alibaba/zvec) | 16153 | C++ | 2026-10-27 | A lightweight, lightning-fast, in-process vector database |
| 6 | [wickra-lib/wickra-genome](https://github.com/wickra-lib/wickra-genome) | 1 | Rust | 2026-10-27 | A vector database of the whole market: every asset as a live vector over the 495 O(1) streaming indicators the registry  |
| 7 | [VecturaDB/VecturaDB.Deploy](https://github.com/VecturaDB/VecturaDB.Deploy) | 0 | Bicep | 2026-10-27 | Deploy Chroma 1.5.9 or VecturaDB in your own cloud: an Azure VM template with HTTPS, allowed IP addresses and backups. |
| 8 | [caoergou/dify-installer](https://github.com/caoergou/dify-installer) | 2 | Shell | 2026-10-27 | One-click installer for Dify Docker deployment \| Dify 一键安装脚本，使用 Docker Compose 部署 |
| 9 | [cyberlife-coder/VelesDB](https://github.com/cyberlife-coder/VelesDB) | 100 | Rust | 2026-10-27 | The explainable, local-first memory engine for AI agents. One ~9 MB binary fuses vector + graph + columnar under VelesQL |
| 10 | [houyidb-community/houyidb-site](https://github.com/houyidb-community/houyidb-site) | 0 | HTML | 2026-10-27 | HouyiDB website (houyidb.top) |
<!-- TRACKER_TABLE_END -->

---

## 🔍 How it works

Every 15 minutes, a GitHub Action runs `tracker.py`. That script:

1. Fetches the latest state from `GitHub Search API`.
2. Diffs against `data/items.json` (the previous snapshot).
3. Rewrites the table above between the `<!-- TRACKER_TABLE_* -->` markers.
4. Commits `feat: +N added, -M removed (timestamp)` if anything changed.

No external services. No paid APIs. Just a public data source and a free GitHub Action.

---

## 🤝 Contributing

See `CONTRIBUTING.md` — usually you don't need to: the tracker keeps itself current.
If you spot a data-source bug or want to suggest a new column for the table, open
an issue.

---

## 🔗 Related live trackers

If you find this useful, you might also like these other auto-updated
trackers from the same maintainer — same mechanism, different upstream:

- [trending-claude-skills](https://github.com/linny006/trending-claude-skills) — What's shipping in Claude Skills this week (`topic:claude-skills`)
- [mcp-servers-live](https://github.com/linny006/mcp-servers-live) — Live index of newest MCP servers (`topic:mcp-server`)
- [cursor-rules-live](https://github.com/linny006/cursor-rules-live) — Newest Cursor rules and .cursorrules patterns (`topic:cursor-rules`)
- [claude-code-plugin-tracker](https://github.com/linny006/claude-code-plugin-tracker) — Claude Code plugins and hook configs (`topic:claude-code`)
- [llm-agents-radar](https://github.com/linny006/llm-agents-radar) — Newest LLM agent frameworks (`topic:llm-agent`)
- [rag-radar](https://github.com/linny006/rag-radar) — Newest RAG implementations and tools (`topic:rag`)
- [llm-eval-tracker](https://github.com/linny006/llm-eval-tracker) — Newest LLM evaluation tools and benchmarks (`topic:llm-eval`)
- [agent-framework-radar](https://github.com/linny006/agent-framework-radar) — Newest agent frameworks shipping on GitHub (`topic:agent-framework`)
- [llmops-radar](https://github.com/linny006/llmops-radar) — Newest LLMOps tooling (observability, deployment) (`topic:llmops`)
- [prompt-tools-live](https://github.com/linny006/prompt-tools-live) — Newest prompt-engineering tools and prompt repos (`topic:prompt-engineering`)
- [agent-eval-harness](https://github.com/linny006/agent-eval-harness) — Live benchmark of AI coding agents (`topic:llm-eval`)
- [skills-tracker](https://github.com/linny006/skills-tracker) — Tracking new GitHub 'skills' repos (`topic:agent-skills`)
- [awesome-agent-skills](https://github.com/linny006/awesome-agent-skills) — Curated auto-updated awesome-list of AI agent skills (`topic:agent-skills`)

---

## 📜 License

MIT — see `LICENSE`.
