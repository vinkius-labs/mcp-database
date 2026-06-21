# PaperQuotes MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/paperquotes)
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


## Available Tools (4)
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


## ❓ FAQ

**Q: How can I get a daily inspirational quote?**
You can use the `get_qod` tool. It fetches a curated Quote of the Day, and you can even specify a language preference.

**Q: Can I search for quotes by a specific author?**
Yes. First, use `search_authors` to find the correct author name, then use `list_quotes` with the `author` parameter to see their quotes.

**Q: Is it possible to filter quotes by topic or tag?**
Absolutely. Use the `list_tags` tool to see available categories, and then pass those tags into the `list_quotes` tool to filter the results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paperquotes](https://vinkius.com/mcp/paperquotes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PaperQuotes** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paperquotes` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PaperQuotes** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paperquotes": {
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
