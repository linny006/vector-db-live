<!--
SEO: vector db live tracker
-->

<div align="center">

# Vector DB Live Tracker

Live-updating landscape of vector database projects, integrations, and benchmarks — refreshed every 15 minutes

[![Stars](https://img.shields.io/github/stars/linny006/vector-db-live?style=for-the-badge&logo=github)](https://github.com/linny006/vector-db-live/stargazers)
[![Last Commit](https://img.shields.io/github/last-commit/linny006/vector-db-live?style=for-the-badge)](https://github.com/linny006/vector-db-live/commits)
[![Items](https://img.shields.io/badge/Tracked_Items-16-brightgreen?style=for-the-badge)](#)
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

> ⏰ Last updated: 2026-10-26 12:45 UTC
>
> Data source: `GitHub Search API`
>
> The table below is rewritten on every cron tick. Star the repo to bookmark.

<!-- TRACKER_TABLE_START -->
| # | Name | ⭐ | Lang | Updated | Description |
|---|------|---|------|---------|-------------|
| 1 | [robcox2910/pyvecdb](https://github.com/robcox2910/pyvecdb) | 0 | Python | 2026-10-26 | Build your own vector database in Python: distance metrics, nearest-neighbour search and metadata filtering, explained f |
| 2 | [giuliano0s/ifrs-canoas-rag](https://github.com/giuliano0s/ifrs-canoas-rag) | 0 | Python | 2026-10-26 |  |
| 3 | [t0rresmarcus/FanVault-AI](https://github.com/t0rresmarcus/FanVault-AI) | 0 | TypeScript | 2026-10-26 | FanVault AI is a RAG chatbot works as an intelligent sports knowledge assistant that helps fans instantly discover playe |
| 4 | [MariaDB/server](https://github.com/MariaDB/server) | 8452 | C++ | 2026-10-26 | MariaDB server is a community developed fork of MySQL server. Started by core members of the original MySQL team, MariaD |
| 5 | [hufengjuexue/zhongji](https://github.com/hufengjuexue/zhongji) | 2 | Kotlin | 2026-10-26 | 终极 RP (ZhongJi RP) - 专为现代大语言模型打造的轻量沉浸式端侧安卓客户端 / Next-gen Mobile Roleplay & Chat Client |
| 6 | [albaozhen-eng/coremem](https://github.com/albaozhen-eng/coremem) | 1 | Python | 2026-10-26 | Git-diffable memory for AI agents — six-layer architecture, plain-text source of truth, Obsidian graph projection. MIT. |
| 7 | [milvus-io/milvus](https://github.com/milvus-io/milvus) | 46485 | Go | 2026-10-26 | Milvus is a high-performance, cloud-native vector database built for scalable vector ANN search |
| 8 | [ppossanzini/Jigen](https://github.com/ppossanzini/Jigen) | 17 | C# | 2026-10-26 | Jigen DB is vector database written from scratch in c# |
| 9 | [topoteretes/cognee](https://github.com/topoteretes/cognee) | 32770 | Python | 2026-10-26 | Cognee is the open-source AI memory platform for agents. Give your AI agents persistent long-term memory with small mode |
| 10 | [GenAIwithMS/OpenGPT](https://github.com/GenAIwithMS/OpenGPT) | 5 | Python | 2026-10-26 | OpenGPT, An open AI workspace for conversations, knowledge, and productivity. |
| 11 | [langchain4j/langchain4j](https://github.com/langchain4j/langchain4j) | 13302 | Java | 2026-10-26 | LangChain4j is an idiomatic, open-source Java library for building LLM-powered applications on the JVM. It offers a unif |
| 12 | [kividbio/kividb](https://github.com/kividbio/kividb) | 658 | Rust | 2026-10-26 | A fast, multi-threaded Redis® and Valkey alternative written in Rust: drop-in compatible, with full-text and vector sear |
| 13 | [matrixorigin/matrixone](https://github.com/matrixorigin/matrixone) | 2058 | Go | 2026-10-26 | AI-native HTAP database with Git-for-Data and built-in vector search, serving as the data and memory backbone for intell |
| 14 | [VectifyAI/PageIndex](https://github.com/VectifyAI/PageIndex) | 39759 | Python | 2026-10-26 | 📑 PageIndex: Document Index for Vectorless, Reasoning-based RAG |
| 15 | [gyr0byte/Generative-AI](https://github.com/gyr0byte/Generative-AI) | 0 | Python | 2026-10-26 | Hands-on GenAI projects learning with LangChain: chatbots, RAG pipelines, and AI agents. Built while learning LLM engine |
| 16 | [taladb/taladb](https://github.com/taladb/taladb) | 24 | Rust | 2026-10-26 | TalaDB - An open-source embedded vector and document database for building local-first AI applications. |
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
