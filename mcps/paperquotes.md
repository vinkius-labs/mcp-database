# PaperQuotes MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/paperquotes)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/paperquotes-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/paperquotes-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Access a vast library of quotes, search by author or tags, and get the quote of the day directly in your AI agent.

## Description
Connect to the **PaperQuotes** API to enrich your conversations with inspiration and wisdom. This MCP server allows your AI agent to browse thousands of quotes, find specific authors, and retrieve curated daily content.

### What you can do

- **Browse Quotes** — List quotes with advanced filters for authors, tags, and languages using the `list_quotes` tool.
- **Quote of the Day** — Fetch a curated daily quote to start your day or spark inspiration with `get_qod`.
- **Author Search** — Find specific authors within the extensive PaperQuotes database using `search_authors`.
- **Tag Discovery** — Explore available categories and tags to find the perfect quote for any context with `list_tags`.

### How it works

1. Subscribe to this server
2. Enter your PaperQuotes API Token
3. Start querying quotes from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Find the perfect quote for social media posts or articles.
- **Developers** — Integrate inspirational content into applications or daily standups.
- **Writers & Researchers** — Quickly verify quotes and find relevant authors for their work.


## Available Tools
- **search_authors**: Search for authors in the database
- **get_qod**: Get a curated Quote of the Day
- **list_quotes**: Retrieve quotes from the PaperQuotes database
- **list_tags**: Retrieve available tags used to categorize quotes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PaperQuotes** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the Quote of the Day in English."

**🤖 AI Agent:**
> I've retrieved today's quote: 'The only way to do great work is to love what you do.' — Steve Jobs. Would you like to see more quotes from Steve Jobs?

---

**👤 You:**
> "Search for authors named 'Marcus Aurelius'."

**🤖 AI Agent:**
> I found 'Marcus Aurelius' in the database. I can now list his quotes for you using the list_quotes tool. Should I proceed?

---

**👤 You:**
> "List 5 quotes about 'wisdom' and 'courage'."

**🤖 AI Agent:**
> I've found several quotes matching those tags. Here are 5 selections including insights from ancient philosophers and modern thinkers. Would you like the full metadata for any of these?


## Installation & Usage

To install and use the **PaperQuotes** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paperquotes](https://vinkius.com/mcp/paperquotes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
