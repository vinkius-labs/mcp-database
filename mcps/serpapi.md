# SerpApi MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/serpapi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent with real-time web search capabilities across Google, Bing, Baidu, Yahoo, and DuckDuckGo.

## Description
The SerpApi MCP server acts as the ultimate eye into the live web for your AI. By connecting this integration, your agents can organically bypass CAPTCHAs, retrieve current SERP events, scrape product catalogs via Google Shopping, find news, images, and localized search results globally. This module bridges the training gap of Language Models allowing instantaneous internet connectivity.


## Available Tools (12)
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


## ❓ FAQ

**Q: Does this tool bypass Google Captchas normally encountered when scraping?**
Yes, completely. SerpApi manages all the proxy rotation securely on its backend, solving the strict bot captchas for you, thereby returning perfectly structured JSON straight to this agent.

**Q: Can I search beyond standard Google web results?**
Certainly! This MCP module allows access to Google Images, Google News, Google Videos, Google Shopping, Bing, Yandex, Yahoo, Baidu and DuckDuckGo.

**Q: How do I ensure search results reflect local or international variations?**
You can use the 'list_locations' capability first to identify valid geo-specific markers and then apply them during the standard searches to narrow down local results accurately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/serpapi](https://vinkius.com/mcp/serpapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SerpApi** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `serpapi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SerpApi** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "serpapi": {
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
