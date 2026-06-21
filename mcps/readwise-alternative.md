# Readwise MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/readwise-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/readwise-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/readwise-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect your AI agents to Readwise to manage books, highlights, tags, and spaced repetition reviews directly through natural language.

## Description
Transform how your organization interacts with reading material by giving your AI agent full control over your Readwise library. With 16 tools covering full highlight CRUD, book search by source and category, tag management, and daily review access, your agents can retrieve specific passages, create annotations, and help you retain knowledge.

### What you can do
- Browse books by source or category
- Full CRUD for highlights, notes, and tags
- Access daily spaced repetition reviews
- Export all data incrementally for backup or analysis

### How it works
1. Subscribe to this server
2. Enter your Readwise API Token (found in your account settings)
3. Start managing your reading library directly from Claude, Cursor, or any MCP client

### Who is it for?
Ideal for researchers, students, and professionals needing instant, conversational access to their curated knowledge base.


## Available Tools
- **check_readwise_status**: Verify connectivity
- **create_highlight**: Create a highlight
- **delete_highlight**: Delete a highlight
- **export_highlights**: Supports incremental export with updatedAfter filter.

Export highlights
- **get_book**: Get book details
- **get_daily_review**: Get daily review
- **get_highlight**: Get highlight details
- **list_books_by_category**: List books by category
- **list_books_by_source**: List books by source
- **list_books**: List all books
- **list_highlights**: Returns text, note, location, and tags.

List highlights
- **list_reviews**: List review queue
- **list_tags**: List all tags
- **search_books**: Search books
- **search_highlights**: Search highlights
- **update_highlight**: Update a highlight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Readwise** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all my highlights related to 'stoicism' and summarize the key themes."

**🤖 AI Agent:**
> I found 14 highlights mentioning stoicism. The recurring themes focus on the dichotomy of control, the practice of negative visualization, and maintaining equanimity in the face of external adversity.

---

**👤 You:**
> "List all the books I've saved from my Kindle library."

**🤖 AI Agent:**
> I've retrieved your Kindle library. You have 22 books saved, including 'Meditations' by Marcus Aurelius, 'Atomic Habits' by James Clear, and 'Deep Work' by Cal Newport.

---

**👤 You:**
> "Create a new highlight for 'The Almanack of Naval Ravikant' with the note: 'Crucial insight on leverage'."

**🤖 AI Agent:**
> Successfully added your highlight to 'The Almanack of Naval Ravikant' with the note regarding leverage.


## Installation & Usage

To install and use the **Readwise** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/readwise-alternative](https://vinkius.com/mcp/readwise-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
