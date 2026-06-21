# Markdown Task Extractor MCP Server

Instantly scan any local folder of Markdown notes (Obsidian, Notion, Logseq) and aggregate every scattered '- [ ]' to-do item into a single, structured list for your AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/markdown-task-extractor)

## Overview
**Category:** productivity
**Tools Count:** 1

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


## Installation & Usage

To install and use the **Markdown Task Extractor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/markdown-task-extractor](https://vinkius.com/mcp/markdown-task-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
