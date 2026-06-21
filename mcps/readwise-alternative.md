# Readwise MCP Server

Connect your AI agents to Readwise to manage books, highlights, tags, and spaced repetition reviews directly through natural language.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/readwise-alternative)

## Overview
**Category:** productivity
**Tools Count:** 16

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


## Installation & Usage

To install and use the **Readwise** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/readwise-alternative](https://vinkius.com/mcp/readwise-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
