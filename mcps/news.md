# News MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/news)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search millions of articles and track breaking headlines from over 150,000 global news sources in real-time.

## Description
Connect your AI agent to the world's most comprehensive news database. This server provides instant access to live headlines and historical articles from thousands of publishers worldwide, ranging from major news outlets to niche blogs.

### What you can do

- **Global Search** — Search through millions of articles using advanced keywords, date filters, and domain restrictions.
- **Breaking Headlines** — Get the latest top stories filtered by country, category (business, tech, sports, etc.), or specific publishers.
- **Source Discovery** — Find and filter valid news sources and publishers to fine-tune your monitoring.
- **Market Intelligence** — Track mentions of companies, products, or trends across the global media landscape.

### How it works

1. Subscribe to this server
2. Enter your NewsAPI Key
3. Start querying live news from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Market Researchers** — monitor industry trends and competitor mentions across thousands of domains.
- **Content Creators** — find the latest stories and verified sources for newsletters or social media updates.
- **Data Analysts** — aggregate news sentiment and volume for specific topics over time.


## Available Tools (3)
- **search_everything**: Supports advanced operators (+, -, AND, OR, NOT) in the query.

Search through millions of articles from over 150,000 news sources
- **list_sources**: Returns a list of publishers available for top headlines
- **get_top_headlines**: Do not mix country/category with sources.

Returns live top and breaking headlines


## 💬 Prompt Examples

Here are some examples of how you can interact with the **News** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the latest news about 'Quantum Computing' from the last 7 days."

**🤖 AI Agent:**
> I've found several articles regarding Quantum Computing. Highlights include a breakthrough in error correction from Google and a new partnership between IBM and several research universities. Would you like the full summaries?

---

**👤 You:**
> "What are the top technology headlines in the US right now?"

**🤖 AI Agent:**
> The top tech stories in the US currently feature new AI regulations being debated in Congress, the launch of a new flagship smartphone, and a major cybersecurity update from Microsoft. I can provide the links to any of these.

---

**👤 You:**
> "List all available news sources for sports in France."

**🤖 AI Agent:**
> I've identified several sports news sources in France, including L'Equipe and various regional publishers. You can use these identifiers to filter your future searches for more targeted results.


## ❓ FAQ

**Q: Can I search for news articles from a specific date range?**
Yes! Use the `search_everything` tool and provide the `from` and `to` parameters in ISO 8601 format (e.g., 2023-12-01) to restrict your search to a specific timeframe.

**Q: How do I find the top business headlines in a specific country like the UK?**
You can use the `get_top_headlines` tool. Set the `country` parameter to 'gb' and the `category` parameter to 'business' to get the latest relevant news.

**Q: Is it possible to see which news sources are available for a specific language?**
Absolutely. Use the `list_sources` tool and specify the `language` parameter (e.g., 'en', 'pt', 'fr') to retrieve a list of all supported publishers for that language.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/news](https://vinkius.com/mcp/news)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **News** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `news` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **News** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "news": {
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
