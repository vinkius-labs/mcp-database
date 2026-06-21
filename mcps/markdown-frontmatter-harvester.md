# Markdown Frontmatter Harvester MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/markdown-frontmatter-harvester)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/markdown-frontmatter-harvester-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/markdown-frontmatter-harvester-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Scan local Obsidian or Hugo vaults and extract all YAML frontmatter (tags, dates, status) into a single structured JSON. Let your AI query your scattered notes metadata instantly.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Markdown Frontmatter Harvester** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan my Obsidian vault at C:/Notes and list all files that have the tag 'urgent'."

**🤖 AI Agent:**
> I found 5 notes with the tag 'urgent'. Here are their filenames: ProjectX.md, MeetingNotes.md...

---

**👤 You:**
> "Harvest the frontmatter from my blog repo and tell me which posts are still marked as 'status: draft'."

**🤖 AI Agent:**
> Based on the frontmatter, you have 12 posts still marked as 'draft'. Would you like the list?

---

**👤 You:**
> "Count how many notes I created in the year 2023 based on the YAML 'date' field."

**🤖 AI Agent:**
> According to the metadata, you created exactly 142 notes in 2023.


## Installation & Usage

To install and use the **Markdown Frontmatter Harvester** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/markdown-frontmatter-harvester](https://vinkius.com/mcp/markdown-frontmatter-harvester)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
