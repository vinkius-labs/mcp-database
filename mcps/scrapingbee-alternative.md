# ScrapingBee MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scrapingbee-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Powerful web scraping with JS rendering, premium proxies, and AI-powered data extraction directly from your AI agent.

## Description
Connect **ScrapingBee** to your AI agent to bypass blocks and extract clean data from any website. Handle headless browsers and rotating proxies automatically.

### What you can do

- **Advanced Scraping** — Use `scrape_html` to fetch content with full JavaScript rendering, custom wait times, and ad blocking.
- **AI Data Extraction** — Leverage `ai_query` to transform messy HTML into structured data using natural language instructions.
- **Search Engine Intelligence** — Use `search_google` to retrieve structured JSON results from web, news, maps, or images.
- **E-commerce Monitoring** — Extract precise product details from Amazon using the `get_amazon_product` tool and ASIN codes.
- **Flexible Formats** — Return content as raw HTML, clean Markdown, or plain text to suit your agent's context window.

### How it works

1. Subscribe to this server
2. Enter your ScrapingBee API Key
3. Start scraping complex sites from Claude, Cursor, or any MCP-compatible client

No more getting blocked by Cloudflare or struggling with complex regex. Your AI handles the selectors while ScrapingBee handles the infrastructure.

### Who is this for?

- **Data Scientists** — gather datasets from JS-heavy SPAs without writing complex crawler logic.
- **Market Researchers** — monitor competitor pricing and search engine rankings automatically.
- **Developers** — integrate live web data into AI workflows without worrying about proxy rotation or browser management.


## Available Tools (7)
- **get_amazon_product**: Scrape Amazon product details
- **ask_chatgpt**: Query the ChatGPT API via ScrapingBee
- **fast_search**: Perform a fast SERP search
- **search_google**: Scrape Google Search results
- **scrape_html**: Supports JS rendering, proxies, and data extraction.

Scrape HTML content from any web page
- **search_walmart**: Scrape Walmart search results
- **search_youtube**: Scrape YouTube search results


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ScrapingBee** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scrape https://news.ycombinator.com and return the content as clean Markdown."

**🤖 AI Agent:**
> I've scraped Hacker News for you. Here is the content converted to Markdown: [Markdown content follows...]

---

**👤 You:**
> "Search Google for 'best MCP servers 2024' and give me the top 3 results."

**🤖 AI Agent:**
> I found the top 3 results for your search: 1. Introduction to MCP... 2. Top MCP Servers List... 3. GitHub MCP Awesome...

---

**👤 You:**
> "Get the price and rating for Amazon product B08N5WRWNW."

**🤖 AI Agent:**
> For the Amazon product (ASIN: B08N5WRWNW), the current price is $999.00 with a rating of 4.8 stars based on 12,450 reviews.


## ❓ FAQ

**Q: Can I extract specific data from a page using natural language instead of CSS selectors?**
Yes! Use the `scrape_html` tool and provide your request in the `ai_query` parameter. The server will use ScrapingBee's AI capabilities to parse the HTML and return exactly what you asked for.

**Q: How do I handle websites that require JavaScript to load content?**
The `scrape_html` tool has `render_js` enabled by default. You can also use `wait` or `wait_for` parameters to ensure the page is fully loaded before the data is captured.

**Q: Can I get structured results from Google Search directly?**
Absolutely. Use the `search_google` tool with your query. It returns structured JSON containing organic results, ads, and related searches, saving you from parsing search result pages manually.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scrapingbee-alternative](https://vinkius.com/mcp/scrapingbee-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ScrapingBee** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scrapingbee-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ScrapingBee** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scrapingbee-alternative": {
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
