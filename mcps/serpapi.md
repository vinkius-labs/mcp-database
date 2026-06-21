# SerpApi MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/serpapi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/serpapi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/serpapi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent with real-time web search capabilities across Google, Bing, Baidu, Yahoo, and DuckDuckGo.

## Description
The SerpApi MCP server acts as the ultimate eye into the live web for your AI. By connecting this integration, your agents can organically bypass CAPTCHAs, retrieve current SERP events, scrape product catalogs via Google Shopping, find news, images, and localized search results globally. This module bridges the training gap of Language Models allowing instantaneous internet connectivity.


## Available Tools
- **baidu_search**: Performs a search on Baidu
- **bing_search**: Performs a search on Bing
- **duckduckgo_search**: Performs a search on DuckDuckGo
- **get_account_info**: Retrieves SerpApi account information
- **google_images**: Returns thumbnails and full-size image links.

Searches for images on Google
- **google_news**: Searches for news on Google
- **google_search**: Specify parameters like "location" or "hl" (language) for localized results.

Performs a search on Google
- **google_shopping**: Searches for products on Google Shopping
- **google_videos**: Searches for videos on Google
- **list_locations**: Lists supported locations for search engines
- **yahoo_search**: Performs a search on Yahoo
- **yandex_search**: Performs a search on Yandex


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SerpApi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search DuckDuckGo to find the latest developer sentiment trends regarding Node.js version 22."

**🤖 AI Agent:**
> I executed duckduckgo_search targeting 'Node.js version 22 developer sentiment'. Many forums are highlighting the native require() support for synchronous ES module loads.

---

**👤 You:**
> "Use Google Shopping search capabilities to retrieve structured prices for an 'ergonomic mesh chair'."

**🤖 AI Agent:**
> I've searched Google Shopping arrays. The paramount cost-effective benchmark is around $650 for the listed items. Would you like to target this filtering to a specific ZIP code?

---

**👤 You:**
> "Verify how many organic searches my SerpApi vault can still execute before I hit quota limits."

**🤖 AI Agent:**
> According to the account info tools, you have precisely 1,240 execution quotas remaining for your current billing month.


## Installation & Usage

To install and use the **SerpApi** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/serpapi](https://vinkius.com/mcp/serpapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
