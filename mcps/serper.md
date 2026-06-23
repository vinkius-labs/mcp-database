# Serper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/serper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Fast, affordable Google Search API — get real-time SERP results, news, and images with 2,500 free searches per month.

## Description
Connect your AI agent to **Serper.dev** — the fastest and most cost-effective way to get Google Search results programmatically.

### What you can do

- **Google Search** — Get organic search results with titles, links, snippets, and positions. Supports geolocation and language parameters for localized results
- **Google News** — Search the latest news articles with headlines, sources, publication dates, and snippets
- **Google Images** — Find image results with URLs, titles, and source pages for visual research

### How it works

1. Subscribe to this server
2. Enter your Serper API key (2,500 free searches/month)
3. Your agent can now search Google in real-time

### Why Serper?

- **2,500 free searches/month** — the most generous free tier for Google SERP APIs
- **Sub-100ms latency** — fastest Google SERP API available
- **Native LangChain/CrewAI integration** — the default search tool for most AI frameworks


## Available Tools (3)
- **google_image_search**: dev to query Google Images and return structured results including image URLs, titles, and source pages. Useful for visual research, content creation, and reference gathering.

Search Google Images for visual content related to any query. Returns image URLs, titles, and sources
- **google_news_search**: dev to query Google News and return the most recent news articles matching your query. Perfect for monitoring breaking news, industry trends, and competitor announcements.

Search Google News for the latest articles on any topic. Returns headlines, sources, dates, and snippets
- **google_search**: dev to perform a real-time Google Search and return structured organic results. Supports geolocation (gl) and language (hl) parameters for localized results. Returns up to 100 results per query.

Search Google and get organic SERP results instantly. Returns titles, links, snippets, and positions for any query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Serper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Google for 'best AI agent frameworks 2026' and show me the top 5 results."

**🤖 AI Agent:**
> Found 5 results for 'best AI agent frameworks 2026':

| # | Title | Source |
|---|---|---|
| 1 | Top 10 AI Agent Frameworks | datacamp.com |
| 2 | LangGraph vs CrewAI vs AutoGen | towardsdatascience.com |
| 3 | Best Agent Tools 2026 | dev.to |
| 4 | Building AI Agents Guide | langchain.com |
| 5 | Agent Framework Comparison | medium.com |

---

**👤 You:**
> "Search the latest news about OpenAI."

**🤖 AI Agent:**
> Found 10 news articles about OpenAI:

| # | Title | Source | Date |
|---|---|---|---|
| 1 | OpenAI Launches New Agent API | techcrunch.com | 2h ago |
| 2 | GPT-5 Release Timeline | theverge.com | 5h ago |
| 3 | OpenAI Valued at $300B | bloomberg.com | 1d ago |

---

**👤 You:**
> "Search Google Images for 'neural network architecture diagram'."

**🤖 AI Agent:**
> Found 10 image results for 'neural network architecture diagram':

1. **CNN Architecture Diagram** — researchgate.net
2. **Transformer Model Architecture** — arxiv.org
3. **Deep Learning Layers Visualization** — towardsdatascience.com


## ❓ FAQ

**Q: How many free searches do I get?**
Serper offers 2,500 free searches per month — no credit card required. This includes Google Search, News, and Images queries. Paid plans start at $50/month for 50,000 searches with additional volume discounts.

**Q: Can I get results for specific countries and languages?**
Yes! Serper supports geolocation (gl parameter) and language (hl parameter) for all search types. For example, set gl='br' and hl='pt' for Brazilian Portuguese results, or gl='fr' and hl='fr' for French results. This works for Search, News, and Images endpoints.

**Q: What types of search results are available?**
Serper provides three search types: organic web results (with titles, links, snippets, and knowledge panels), Google News (with headlines, sources, dates), and Google Images (with image URLs and source pages). All results include structured metadata for easy parsing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/serper](https://vinkius.com/mcp/serper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Serper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `serper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Serper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "serper": {
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
