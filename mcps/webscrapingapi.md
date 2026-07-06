# WebScrapingAPI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/webscrapingapi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Scrape HTML, render JavaScript, and retrieve structured SERP data using WebScrapingAPI's high-proxy network.

## Description
Connect your **WebScrapingAPI** account to any AI agent and harness the power of industrial-grade web scraping through natural conversation.

### What you can do

- **Universal Scraping** — Retrieve raw HTML from any website using a massive network of datacenter and residential proxies to avoid blocks
- **JavaScript Rendering** — Scrape complex SPAs and dynamic pages by using a headless browser to capture the full rendered state
- **SERP Discovery** — Retrieve structured search engine results (organic, ads, snippets) from Google, Bing, and Yandex
- **E-commerce Extraction** — Scrape product details like price, reviews, and titles from major stores like Amazon and Walmart into structured JSON
- **Anonymity & Bypass** — Use residential or mobile proxies for high-anonymity scraping and to bypass even the most aggressive bot detections
- **Auto-Parsing** — Automatically extract structured data from news articles or product pages without manual selectors
- **Custom Parameters** — Execute scrapes with advanced options like geo-targeting, sessions, and custom headers

### How it works

1. Subscribe to this server
2. Enter your WebScrapingAPI Key
3. Start extracting web data through Claude, Cursor, or any MCP-compatible client

No more manual selector debugging or proxy management. Your AI agent becomes your web data architect.

### Who is this for?

- **Data Scientists** — collect massive datasets for ML training and market research through simple chat commands
- **Developers** — test scraping logic and verify JavaScript rendering without building custom scrapers
- **E-commerce Managers** — monitor competitor pricing and product availability across different marketplaces
- **SEO Specialists** — track SERP rankings and analyze search snippets from multiple engines and regions


## Available Tools (10)
- **custom_api_scrape**: g. country, session, wait_for).

Execute a scrape using advanced custom parameters
- **search_bing_serp**: Retrieve structured search engine results from Bing
- **scrape_and_auto_extract**: g. for news or product pages).

Scrape with automatic structured data extraction
- **scrape_ecommerce_product**: Returns price, title, and reviews as structured JSON.

Scrape product details from Amazon, Walmart, or other supported stores
- **scrape_static_html**: Pass the full target URL.

Scrape raw HTML from any URL using WebScrapingAPI datacenter proxies
- **scrape_js_rendered**: Slower but captures the full rendered state.

Scrape JS-rendered HTML using WebScrapingAPI headless browser
- **scrape_as_mobile**: Scrape as a mobile device using WebScrapingAPI device emulation
- **scrape_via_residential_proxy**: Scrape using residential proxies for high anonymity and bypass
- **search_google_serp**: Provide a query string.

Retrieve structured search engine results from Google
- **search_yandex_serp**: Retrieve structured search engine results from Yandex


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WebScrapingAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scrape the rendered HTML of 'https://example.com/dynamic-dashboard'."

**🤖 AI Agent:**
> I've scraped the dynamic page using a headless browser. Here is the rendered content, including all JavaScript-generated elements and data points from the dashboard.

---

**👤 You:**
> "Search Google for 'best wireless noise cancelling headphones' and return structured results."

**🤖 AI Agent:**
> I found the top Google SERP results for your query. 1. 'Sony WH-1000XM5 review' (https://...), 2. 'Bose QuietComfort Ultra' (https://...), 3. 'Apple AirPods Max' (https://...). Would you like to see the snippets or ads associated with these?

---

**👤 You:**
> "Get the price and rating for the product at 'https://amazon.com/dp/B09XXX'."

**🤖 AI Agent:**
> Successfully extracted product data from Amazon: Name: 'AcousticPro Wireless', Price: '$299.00', Rating: '4.8/5 stars (1,250 reviews)'. Would you like the full JSON extract?


## ❓ FAQ

**Q: Can I scrape websites that heavily use JavaScript?**
Yes. Use the `scrape_js_rendered` tool. It utilizes a headless browser to execute the JavaScript on the target page and returns the full rendered HTML, making it ideal for SPAs built with React, Vue, or Angular.

**Q: How do I get structured data from Google search results?**
You can use the `search_google_serp` tool. Simply provide your search query, and WebScrapingAPI will return a structured JSON object containing organic results, titles, URLs, snippets, and even ads.

**Q: What if a website blocks standard scraping attempts?**
Use the `scrape_via_residential_proxy` tool. This routes your request through real residential IP addresses, providing maximum anonymity and allowing you to bypass aggressive bot protection systems.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/webscrapingapi](https://vinkius.com/mcp/webscrapingapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WebScrapingAPI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `webscrapingapi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WebScrapingAPI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "webscrapingapi": {
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
