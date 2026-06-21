# NewsCatcher MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/newscatcher)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Search millions of news articles in real-time with AI clustering and topic tracking.

## Description
Connect **NewsCatcher** to any AI agent and access a massive, real-time news feed aggregator with powerful clustering and filtering capabilities.

### What you can do
- **Real-Time Search** — Search millions of articles instantly with keyword, language, country, and source filters
- **Latest News Feed** — Get the most recent articles for any topic or publisher
- **News Clustering** — Group similar stories to see how different outlets cover the same event
- **Source Discovery** — List available news sources by country, topic, or language
- **Global Coverage** — Access news from over 100,000 sources worldwide

### How it works
1. Subscribe to this server
2. Enter your NewsCatcher API Key
3. Start tracking global news trends from Claude, Cursor, or any MCP-compatible client

NewsCatcher uses AI to normalize and cluster news from diverse sources, making it easy to track narratives.

### Who is this for?
- **Media Analysts** — Monitor how narratives evolve across different outlets using clustering
- **Researchers** — Find niche articles with precise filtering options
- **Brand Managers** — Track mentions across global media in real-time


## Available Tools
- **get_news_clusters**: Get grouped news stories (clusters)
- **get_latest_news**: Use "q" for keywords, "topic" (e.g., "sports"), "countries" (e.g., "US"), or "sources" (e.g., "cnn.com").

Get the latest news articles for a topic or source
- **search_news**: Use "q" for keywords, "lang" for language (e.g., "en"), "countries" for country codes (e.g., "US"), and "sort_by" (relevancy, date).

Search for news articles using keywords and filters
- **list_sources**: Filter by "topic", "countries", or "lang".

List available news sources


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NewsCatcher** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find latest news about 'Artificial Intelligence' in the US."

**🤖 AI Agent:**
> Found 542 articles: 1. New AI Regulations Proposed in Senate. 2. Tech Giants Invest Billions in AI Research. 3. AI Breakthrough in Medical Diagnostics Announced.

---

**👤 You:**
> "Show me clusters for the topic 'Elections'."

**🤖 AI Agent:**
> Top Clusters: 1. 'Global Election Trends' (150 articles). 2. 'Voting Technology Updates' (45 articles). 3. 'Campaign Finance Reform' (30 articles).

---

**👤 You:**
> "List all English news sources available for Sports."

**🤖 AI Agent:**
> Available Sports Sources: ESPN, BBC Sport, Sky Sports, Bleacher Report, The Athletic, and 45 others.


## ❓ FAQ

**Q: How does NewsCatcher differ from other news APIs?**
NewsCatcher uses AI to cluster similar stories and normalize data from diverse sources, making it easier to track narratives and avoid duplicates.

**Q: Can I filter news by country and language?**
Yes! You can filter by 'lang' (e.g., 'en', 'pt') and 'countries' (e.g., 'US', 'BR', 'FR') to get highly localized content.

**Q: What are 'News Clusters'?**
News Clusters group articles that cover the same event or topic, allowing you to see diverse perspectives and coverage from different publishers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/newscatcher](https://vinkius.com/mcp/newscatcher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NewsCatcher** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `newscatcher` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NewsCatcher** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "newscatcher": {
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
