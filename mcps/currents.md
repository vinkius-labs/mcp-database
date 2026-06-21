# Currents MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/currents)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/currents-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/currents-mcp)
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


## Available Tools
- **check_auth**: Check API authentication status
- **list_categories**: List available news categories
- **list_languages**: List available languages
- **get_latest_news**: Do not use search keywords here.

Get latest real-time news articles
- **list_regions**: List available regions/countries
- **search_news**: Use keywords or boolean query syntax.

Search for news articles by keywords or query


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


## Installation & Usage

To install and use the **Currents** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/currents](https://vinkius.com/mcp/currents)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
