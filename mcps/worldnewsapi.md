# WorldNewsAPI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/worldnewsapi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Search world news — audit articles, top stories, and sources via AI.

## Description
Empower your AI agent to orchestrate your entire media research and news auditing workflow with **WorldNewsAPI**, the comprehensive source for global journalism. By connecting WorldNewsAPI to your agent, you transform complex keyword searches into a natural conversation. Your agent can instantly retrieve real-time articles, audit top stories by country, and extract metadata from specific news URLs without you ever touching a news portal. Whether you are conducting market analysis or monitoring regional geopolitical shifts, your agent acts as a real-time news analyst, ensuring your intelligence is always verified and precise.

### What you can do

- **News Auditing** — Search for thousands of real-time news articles by keyword or phrase and maintain a clear view of global media distribution.
- **Headline Oversight** — Audit the top stories for specific countries and languages to understand the current industry lead in information flow instantly.
- **URL Intelligence** — Extract high-resolution content and metadata from specific news links to assist in deep-dive media classification.
- **Source Discovery** — Retrieve detailed metadata for news articles to identify relevant stylistic markers for your research.
- **Operational Monitoring** — Check API status to ensure your media research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your WorldNewsAPI Key
3. Start managing your news intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Media Analysts & Journalists** — monitor global trends and retrieve official metadata straight from your workflow.
- **Market Researchers** — verify industry news and audit information patterns without manual searching.
- **Policy Leads** — perform rapid audits of regional stories and identify relevant geopolitical markers through natural language.
- **Operations Leads** — automate news data querying to orchestrate cross-functional research teams smoothly.


## Available Tools
- **check_api_status**: Check if the WorldNews service is operational
- **extract_news_from_url**: Extract article content and metadata from a specific news URL
- **get_top_world_news**: Get top news headlines for a specific country and language
- **search_world_news**: Search for world news articles by keyword or phrase


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WorldNewsAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for news about 'artificial intelligence' using WorldNewsAPI."

**🤖 AI Agent:**
> I've retrieved several articles about artificial intelligence! Notable headlines include updates on new model releases and industry regulations. Would you like the full text or the source metadata for any of these stories?

---

**👤 You:**
> "Show the top stories in 'United Kingdom' in 'English'."

**🤖 AI Agent:**
> I've identified the top stories for the UK in English! They cover current events from major British publishers. I can provide the summary and direct links for each of these articles if you'd like.

---

**👤 You:**
> "Extract the news content from 'https://www.bbc.com/news/example-article'."

**🤖 AI Agent:**
> I've retrieved the article content! The text covers [Summary]. I can also assist you with the publication date and author metadata for this specific link.


## ❓ FAQ

**Q: How do I find my WorldNewsAPI Key?**
Sign up for an account at [**worldnewsapi.com**](https://worldnewsapi.com/), and you will find your API Key in your dashboard. Copy and paste it below.

**Q: Can I filter news by country?**
Yes. Use the `get_top_world_news` tool and provide the 2-letter country code (e.g., 'us' or 'br'). Your agent will return matching top stories instantly.

**Q: Does it support article extraction?**
Yes. The `extract_news_from_url` tool retrieves the full text and metadata for a news article from any specified URL in the database.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/worldnewsapi](https://vinkius.com/mcp/worldnewsapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WorldNewsAPI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `worldnewsapi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WorldNewsAPI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "worldnewsapi": {
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
