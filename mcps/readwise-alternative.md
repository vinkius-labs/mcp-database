# Readwise MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/readwise-alternative)
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


## Available Tools (16)
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


## ❓ FAQ

**Q: What can I do with the Readwise connector?**
You can list, search, create, update, and delete highlights, browse books by source or category, manage tags, access your daily spaced repetition review, and export all data incrementally for analysis or backup.

**Q: How does the daily review feature work?**
The daily review tool retrieves highlights selected by Readwise's spaced repetition algorithm, helping your AI agent surface the most important passages at the optimal retention interval.

**Q: Can I filter books by where they came from?**
Yes, you can filter by source (Kindle, Instapaper, Pocket, web, Apple Books) or by category (books, articles, tweets, podcasts) to quickly find the content you need.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/readwise-alternative](https://vinkius.com/mcp/readwise-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Readwise** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `readwise-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Readwise** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "readwise-alternative": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
