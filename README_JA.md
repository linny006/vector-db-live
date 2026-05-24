# vector-db-live

> ベクターデータベースのプロジェクト・インテグレーション・ベンチマークをリアルタイムで追跡 — 15 分ごとに自動更新

[English](./README.md) · [中文](./README_CN.md) · **日本語** · [한국어](./README_KO.md) · [Español](./README_ES.md) · [Português](./README_PT.md)

[![Stars](https://img.shields.io/github/stars/linny006/vector-db-live?style=for-the-badge&logo=github)](https://github.com/linny006/vector-db-live/stargazers)
[![Last Commit](https://img.shields.io/github/last-commit/linny006/vector-db-live?style=for-the-badge)](https://github.com/linny006/vector-db-live/commits)

---

GitHub、パッケージレジストリ、リリースフィードからライブデータを取得し、ベクターデータベースのエコシステムを自動で追跡・比較します。pgvector、Qdrant、Chroma、Weaviate、Milvus などのプロジェクトについて、成熟度・インテグレーション・言語サポート・最近のアクティビティを網羅した、常に最新の構造化比較テーブルを生成します。

このリストは GitHub Actions の cron によって**15 分ごとに自動更新**されます。各コミットはアップストリームデータソースの実際の変化（新規追加・期限切れ削除）を反映しているので、表示内容が常に最新であることを信頼できます。

---

15 分ごとに GitHub Action が `tracker.py` を実行します。このスクリプトは以下を行います：

1. `GitHub Search API` から最新の状態を取得する。
2. `data/items.json`（前回のスナップショット）と差分を比較する。
3. `<!-- TRACKER_TABLE_* -->` マーカー間のテーブルを書き換える。
4. 変更があれば `feat: +N added, -M removed (timestamp)` としてコミットする。

外部サービス不要。有料 API 不要。公開データソースと無料の GitHub Action だけで動きます。

---

## 📋 Live data

ライブデータは英語版 README をご覧ください

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
