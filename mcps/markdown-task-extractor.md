# Markdown Task Extractor MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/markdown-task-extractor)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/markdown-task-extractor-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/markdown-task-extractor-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Instantly scan any local folder of Markdown notes (Obsidian, Notion, Logseq) and aggregate every scattered '- [ ]' to-do item into a single, structured list for your AI.

## Description
If you use Obsidian, Logseq, or Notion, your tasks are probably scattered across dozens of different daily notes and project files. When you ask your AI, 'What are my pending tasks today?', it has no idea because it can't read your local vault effectively.

This MCP uses a hyper-fast glob pattern to scan hundreds of local `.md` files in milliseconds. It extracts every `- [ ]` (pending) and `- [x]` (completed) task, along with the specific file it came from, and feeds it directly into your AI chat context. It transforms your local vault into a centralized AI task dashboard.

### The Superpowers

- **Vault-Wide Aggregation:** Turns your scattered notes into a centralized task dashboard.
- **Zero Config:** Just give the AI the absolute path to your notes folder.
- **Lightning Fast:** Uses `fast-glob` to scan 1,000+ files in under 50ms.
- **Status Aware:** Perfectly distinguishes between open and completed tasks.


## Available Tools
- **extract_markdown_todos**: Provide the absolute directory path to scan.

Scan a local directory of Markdown files (Obsidian, Notion, Logseq) and extract all open and completed tasks (- [ ] and - [x])


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Markdown Task Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan my Obsidian vault at C:/Notes and list all my pending tasks grouped by file."

**🤖 AI Agent:**
> I found 12 pending tasks across 4 different files. Here is the grouped breakdown:

---

**👤 You:**
> "Look through my Notion exports folder and tell me how many tasks I completed this week."

**🤖 AI Agent:**
> Based on the `- [x]` markers, you have completed exactly 24 tasks.

---

**👤 You:**
> "Find all tasks in my project folder that contain the hashtag '#urgent'."

**🤖 AI Agent:**
> I found 3 open tasks marked with #urgent:
1. Fix database deployment (backend.md)
2. Call investor (meetings.md)


## Installation & Usage

To install and use the **Markdown Task Extractor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/markdown-task-extractor](https://vinkius.com/mcp/markdown-task-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
