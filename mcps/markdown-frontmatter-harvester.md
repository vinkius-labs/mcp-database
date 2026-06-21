# Markdown Frontmatter Harvester MCP Server

Scan local Obsidian or Hugo vaults and extract all YAML frontmatter (tags, dates, status) into a single structured JSON. Let your AI query your scattered notes metadata instantly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/markdown-frontmatter-harvester)

## Overview
**Category:** developer-tools
**Tools Count:** 1

## Description
If you use a Knowledge Management system like Obsidian, Logseq, or Hugo, you likely use YAML 'frontmatter' at the top of your markdown files to track metadata like `status: draft`, `tags: [idea, research]`, or `date: 2024-01-01`.

When you ask Claude, 'Which of my notes are marked as drafts and never published?', it fails because it can't read thousands of local files quickly. This MCP solves that by acting as a hyper-fast metadata librarian. It recursively scans your local folder, rips out only the YAML frontmatter from every file, and aggregates it into a clean JSON index. The AI can then instantly filter, sort, and query your entire knowledge base.

### The Superpowers

- **Vault-Wide Indexing:** Turns scattered local markdown metadata into a unified database.
- **Lightning Fast:** Uses `fast-glob` and `gray-matter` to scan 1,000+ files in milliseconds.
- **Zero Config:** Just give the AI the absolute path to your notes folder.
- **100% Air-Gapped Privacy:** Your private journal entries and business notes never leave your machine.


## Available Tools
- **harvest_markdown_frontmatter**: Provide the absolute directory path.

Scan a local directory of Markdown files (Obsidian/Hugo) and extract all YAML frontmatter tags, dates, and metadata


## Installation & Usage

To install and use the **Markdown Frontmatter Harvester** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/markdown-frontmatter-harvester](https://vinkius.com/mcp/markdown-frontmatter-harvester)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
