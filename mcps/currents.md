# Currents MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/currents)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access real-time global news and search millions of articles directly from your AI agent using the Currents API.

## Description
Connect your **Currents** account to any AI agent to monitor global media, track specific topics, and retrieve real-time news streams through natural language.

### What you can do

- **Real-time News** — Stream the latest international news articles as they happen without complex search queries.
- **Advanced Search** — Query a database of tens of millions of articles using keywords or boolean logic (AND, OR, NOT).
- **Granular Filtering** — Filter results by language, country, category, or specific domains like reuters.com.
- **Metadata Discovery** — List all supported categories, regions, and languages to refine your news monitoring.
- **Deep Pagination** — Access historical data and large result sets using page numbers or cursor-based navigation.

### How it works

1. Subscribe to this server
2. Enter your Currents API Key
3. Start querying global news from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Market Analysts** — track industry trends and competitor mentions in real-time.
- **Content Creators** — find inspiration and verify facts across global news sources.
- **Researchers** — perform deep searches across millions of archived articles for specific data points.


## Available Tools (6)
- **get_latest_news**: Do not use search keywords here.

Get latest real-time news articles
- **list_regions**: List available regions/countries
- **search_news**: Use keywords or boolean query syntax.

Search for news articles by keywords or query
- **check_auth**: Check API authentication status
- **list_categories**: List available news categories
- **list_languages**: List available languages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Currents** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the latest news in technology from the US."

**🤖 AI Agent:**
> I've fetched the latest technology news from the United States. Key headlines include updates on new AI regulations and recent semiconductor breakthroughs. Would you like me to summarize any specific article?

---

**👤 You:**
> "Search for articles about 'SpaceX' AND 'Mars' from the last 30 days."

**🤖 AI Agent:**
> Searching the archives... I found several articles regarding SpaceX's Mars mission plans and recent Starship tests. I can provide the links and descriptions for the top 5 results.

---

**👤 You:**
> "What are the available news categories I can filter by?"

**🤖 AI Agent:**
> I've retrieved the list of supported categories. You can filter news by: business, entertainment, general, health, science, sports, and technology. Which one interests you?


## ❓ FAQ

**Q: How do I find the latest news without specific keywords?**
Use the `get_latest_news` tool. It provides a real-time stream of international news. You can optionally filter by `language`, `country`, or `category` to narrow down the stream.

**Q: Can I search for articles using complex logic like AND/OR?**
Yes! Use the `search_news` tool and provide your logic in the `query` parameter. This allows you to use boolean syntax to find exactly what you need across millions of articles.

**Q: How do I know which country codes or categories are supported?**
You can use the `list_regions` tool to see all supported 2-letter country codes and the `list_categories` tool to see the canonical list of news categories available for filtering.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/currents](https://vinkius.com/mcp/currents)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Currents** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `currents` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Currents** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "currents": {
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
