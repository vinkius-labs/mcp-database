# TheySaidSo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/theysaidso)
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


## Available Tools (4)
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


## ❓ FAQ

**Q: How can I get a specific type of quote for today?**
You can use the `get_quote_of_the_day` tool and provide a `category` such as 'inspire', 'management', 'life', or 'funny' to get a curated quote matching that theme.

**Q: How do I know which categories are available for the Quote of the Day?**
Simply run the `list_qod_categories` tool. It will return a complete list of valid categories that you can use to filter your daily quotes.

**Q: Is it possible to search for quotes by a specific person?**
Yes! Use the `search_quotes` tool and provide the `author` name. You can also combine this with a `query` string to find specific topics mentioned by that author.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/theysaidso](https://vinkius.com/mcp/theysaidso)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TheySaidSo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `theysaidso` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TheySaidSo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "theysaidso": {
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
