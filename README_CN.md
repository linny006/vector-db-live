# vector-db-live

> 向量数据库项目、集成与基准测试的实时动态全景图 — 每 15 分钟自动刷新

[English](./README.md) · **中文** · [日本語](./README_JA.md) · [한국어](./README_KO.md) · [Español](./README_ES.md) · [Português](./README_PT.md)

[![Stars](https://img.shields.io/github/stars/linny006/vector-db-live?style=for-the-badge&logo=github)](https://github.com/linny006/vector-db-live/stargazers)
[![Last Commit](https://img.shields.io/github/last-commit/linny006/vector-db-live?style=for-the-badge)](https://github.com/linny006/vector-db-live/commits)

---

通过抓取 GitHub、包注册表和发布订阅的实时数据，自动追踪并对比向量数据库生态系统。生成结构化、始终最新的对比表，涵盖 pgvector、Qdrant、Chroma、Weaviate、Milvus 等项目的成熟度、集成情况、语言支持和近期动态。

本列表由 GitHub Actions 定时任务**每 15 分钟自动更新**一次。每次提交都对应上游数据源的真实变化 — 新增条目或移除过期条目 — 所以你看到的内容随时都是最新的。

---

每隔 15 分钟，GitHub Action 会运行 `tracker.py`，该脚本会：

1. 从 `GitHub Search API` 拉取最新状态。
2. 与 `data/items.json`（上一次快照）做差异对比。
3. 在 `<!-- TRACKER_TABLE_* -->` 标记之间重写上方的表格。
4. 如有变化，提交 `feat: +N added, -M removed (timestamp)`。

无需外部服务，无需付费 API，只用公开数据源和免费的 GitHub Action。

---

## 📋 Live data

实时数据请查看英文版 README

---

## 🔗 Related live trackers

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
