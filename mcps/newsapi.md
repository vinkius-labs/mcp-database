# NewsAPI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/newsapi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/newsapi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/newsapi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Search breaking news and historical articles from 150,000+ sources via NewsAPI.org.

## Description
Connect **NewsAPI** to any AI agent and access real-time breaking news, top headlines, and 5 years of historical articles from over 150,000 news sources worldwide.

### What you can do
- **Top Headlines** — Get live breaking news for any country or category
- **Full-Text Search** — Search every article ever published with keyword, date, and language filters
- **Source Discovery** — List all available news publishers indexed by the API
- **Multi-Language** — Access news in English, Portuguese, Spanish, French, and more
- **Historical Research** — Query articles from the last 5 years for trend analysis
- **Domain Filtering** — Restrict searches to specific domains or sources

### How it works
1. Subscribe to this server
2. Enter your NewsAPI API Key
3. Start searching global news from Claude, Cursor, or any MCP-compatible client

NewsAPI.org aggregates content from major publishers like BBC, CNN, Reuters, Bloomberg, TechCrunch, and thousands more.

### Who is this for?
- **Journalists & Researchers** — Quickly find relevant articles, track breaking news, and analyze media coverage across time
- **Brand Monitors** — Track mentions of companies or products across global news sources
- **Financial Analysts** — Monitor market-moving news and sentiment for specific sectors


## Available Tools
- **get_headlines_by_category**: Get top headlines by category
- **get_headlines_by_country**: g., "us", "br", "gb").

Get top headlines by country
- **get_articles_from_domains**: Search articles from specific domains
- **get_articles_by_language**: g., "en", "pt", "es").

Search articles by language
- **get_popular_articles**: Search most popular articles
- **get_recent_articles**: Search most recent articles
- **get_headlines_by_source**: g., "bbc-news", "cnn").

Get headlines from specific sources
- **list_sources**: List available news sources
- **search_articles**: Search all articles (Everything)
- **search_headlines**: Search headlines by query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NewsAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me top business headlines in the US."

**🤖 AI Agent:**
> Top US Business Headlines: 1. Fed Holds Rates Steady Amid Inflation Concerns (Reuters). 2. Tech Stocks Rally as Earnings Beat Expectations (Bloomberg). 3. Oil Prices Surge on Supply Disruptions (CNBC).

---

**👤 You:**
> "Search for articles about 'Artificial Intelligence regulation' from the last 30 days."

**🤖 AI Agent:**
> Found 1,245 articles: 1. EU AI Act Enters Final Review Phase (TechCrunch). 2. US Senate Debates New AI Safety Framework (The Verge). 3. UK Proposes Light-Touch AI Regulation (Financial Times).

---

**👤 You:**
> "What are the main news sources in Brazil?"

**🤖 AI Agent:**
> Top Brazil Sources: Globo, Folha de S.Paulo, O Estado de S. Paulo, UOL, CNN Brasil, Metrópoles, and Valor Econômico. Total: 35+ active Brazilian sources indexed.


## Installation & Usage

To install and use the **NewsAPI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/newsapi](https://vinkius.com/mcp/newsapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
