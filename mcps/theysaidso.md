# TheySaidSo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/theysaidso)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/theysaidso-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/theysaidso-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Access the world's largest quote API — retrieve the Quote of the Day, search by author, and fetch random inspiration directly via AI.

## Description
Connect the **TheySaidSo** API to your AI agent to enrich your conversations with curated wisdom, motivational content, and famous sayings from thousands of authors.

### What you can do

- **Quote of the Day** — Fetch the daily curated quote, optionally filtered by categories like 'inspire', 'management', or 'life'.
- **Category Discovery** — List all available categories to find the perfect theme for your content or mood.
- **Random Inspiration** — Retrieve one or more random quotes based on specific authors, tags, or character length.
- **Advanced Search** — Deep search the database using text queries, specific authors, or length constraints to find the exact words you need.

### How it works

1. Subscribe to this server
2. Enter your TheySaidSo API Key (optional for basic use, required for higher limits)
3. Start requesting quotes in Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — instantly find relevant quotes for social media posts or articles without manual searching
- **Developers** — integrate motivational features or daily wisdom into applications directly from the prompt
- **Writers & Editors** — verify famous sayings and find attribution for specific themes or authors


## Available Tools
- **list_qod_categories**: List all available categories for the Quote of the Day
- **get_quote_of_the_day**: The same quote is returned for the full calendar day.

Retrieve the curated quote of the day
- **get_random_quotes**: Can be filtered by author, tag, or length. Limit depends on API plan.

Retrieve one or more random quotes from the database
- **search_quotes**: Search for quotes based on specific criteria


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TheySaidSo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the quote of the day for inspiration?"

**🤖 AI Agent:**
> The inspirational quote of the day is: 'Believe you can and you're halfway there.' — Theodore Roosevelt.

---

**👤 You:**
> "List all available categories for the quote of the day."

**🤖 AI Agent:**
> I've retrieved the categories for you. You can choose from: inspire, management, sports, life, funny, love, art, and students.

---

**👤 You:**
> "Search for quotes about 'success' by 'Steve Jobs'."

**🤖 AI Agent:**
> I found a relevant quote by Steve Jobs: 'If you really look closely, most overnight successes took a long time.' Would you like to see more from him?


## Installation & Usage

To install and use the **TheySaidSo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/theysaidso](https://vinkius.com/mcp/theysaidso)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
