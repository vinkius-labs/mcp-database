# Mediastack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mediastack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Access real-time and historical news articles from over 7,500 sources worldwide directly through your AI agent.

## Description
Connect **Mediastack** to your AI agent to search, filter, and retrieve global news data using natural language.

### What you can do

- **Live News** — Fetch the latest headlines and articles as they break across the globe from thousands of publishers.
- **Historical Archives** — Query past news events by specifying exact dates or date ranges to track the evolution of a story.
- **Source Discovery** — List and filter thousands of supported news outlets by country, category, or language to find specific perspectives.
- **Advanced Filtering** — Narrow down results using keywords, specific sources, or geographic regions to get exactly the information you need.

### How it works

1. Subscribe to this server
2. Enter your Mediastack Access Key
3. Start querying global news from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Market Analysts** — track industry trends and competitor news in real-time without leaving your research environment.
- **Content Creators** — find relevant articles and historical context for newsletters, blogs, or social media posts.
- **Journalists & Researchers** — quickly aggregate sources and verify timelines of events across multiple global outlets.


## Available Tools (2)
- **list_sources**: Retrieve a list of all supported news sources
- **get_news**: Use the date parameter for historical news.

Retrieve live or historical news articles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mediastack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the latest technology news from the US in English."

**🤖 AI Agent:**
> I've found 10 recent technology articles from the US. Headlines include 'New AI Breakthrough' and 'Silicon Valley Trends'. Would you like a summary of any of these?

---

**👤 You:**
> "List all news sources available in the sports category for the UK."

**🤖 AI Agent:**
> I've retrieved the sports sources for the UK. Available publishers include 'BBC Sport', 'Sky Sports', and 'The Guardian Sports'. Which one should I query for articles?

---

**👤 You:**
> "Search for news articles about 'SpaceX' published on 2024-01-15."

**🤖 AI Agent:**
> Searching archives... I found 5 articles about SpaceX from January 15th, 2024. The top headline is 'Starship Flight Test Update'. Shall I provide the full details?


## ❓ FAQ

**Q: Can I filter news by specific countries or languages?**
Yes! Use the `get_news` tool and specify the `countries` (e.g., 'us') or `languages` (e.g., 'en') parameters to narrow down your search results.

**Q: How do I find which news sources are available?**
Simply use the `list_sources` tool. You can optionally filter the list by category, country, or language to find the exact publishers supported by Mediastack.

**Q: Can I search for news from a specific date in the past?**
Absolutely. The `get_news` tool accepts a `date` parameter. You can provide a single date (YYYY-MM-DD) or a date range to retrieve historical articles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mediastack](https://vinkius.com/mcp/mediastack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mediastack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mediastack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mediastack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mediastack": {
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
