# Bear MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bear)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bear-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bear-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Bear notes via AI — search, create, and organize your markdown knowledge base autonomously.

## Description
Connect your **Bear App** database to any AI agent and manage your entire localized knowledge base through natural conversation.

### O que você pode fazer

- **Note Operations** — Search globally, read explicit full-markdown note content, and orchestrate the creation of rich hierarchical docs
- **Content Mutation** — Inject new blocks into existing resources (`add_text`), avoiding constant manual copy-pasting
- **Lifecycle Control** — Move outdated research aggressively to the Archive or permanently isolate abandoned drafts in the Trash
- **Taxonomy & Tags** — List tags, explore bounded nested hierarchies, or completely rename structural tags across thousands of items

### Como funciona

1. Subscribe to this server
2. Enter your Bear API Token (interfacing directly with your private local instance)
3. Take absolute control of your linked-thinking graph via Claude or Cursor natively

Say goodbye to breaking focus. Your autonomous agent fetches the precise code snippets or creative writing you saved months ago without breaking context.

### Para quem é?

- **Developers** — inject raw saved configuration blocks directly into your active coding environment
- **Writers & Researchers** — let the AI read your fragmented thoughts, organize your nested active tags, and assemble pristine drafts
- **Productivity Enthusiasts** — search the "@todo" tag instantly summarizing all pending personal action items


## Available Tools
- **search_notes**: g. @todo @today).

Search across all Bear app notes
- **open_note**: Retrieve explicit complete Markdown content of a Bear note
- **create_note**: Create a new native Bear note
- **add_text**: Append or prepend Markdown chunks to a Bear note
- **trash_note**: Move an explicit Bear Note to the Trash
- **archive_note**: Archive an explicit Bear Note
- **list_tags**: g. parent/child).

Retrieve the exact Tags taxonomy nesting globally
- **open_tag**: List all explicit Bear notes matching a specific tag
- **rename_tag**: Rename globally an entire tag across all mapped Notes
- **delete_tag**: Destroy entirely a Tag constraint globally


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bear** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my Bear notes for anything mentioning 'Database Migration 2026'."

**🤖 AI Agent:**
> The query returned 3 explicit note UUIDs. The highly relevant document is titled 'Q1 Migration Plan' (UUID: FE12...). Should I open this full exact note fetching its entire underlying Markdown syntax?

---

**👤 You:**
> "Rename the tag '#project/legacy' to '#archive/legacy_projects' across all my notes."

**🤖 AI Agent:**
> Globally executed target mutation. The tag '#project/legacy' has been fully reconstructed into '#archive/legacy_projects'. Bear natively propagated changes eliminating any obsolete string traces successfully.

---

**👤 You:**
> "Create a new note with the title 'Meeting Notes - App V2' and tag it 'work/meetings/vurb'."

**🤖 AI Agent:**
> The note 'Meeting Notes - App V2' has been initialized via API injection and synced instantly. Its explicitly nested taxonomy tag 'work/meetings/vurb' binds correctly inside the local knowledge cache.


## Installation & Usage

To install and use the **Bear** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bear](https://vinkius.com/mcp/bear)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
