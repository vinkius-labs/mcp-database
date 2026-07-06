# Zenserp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zenserp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Scrape live search engine results (SERP) from Google, Bing, Yandex, and DuckDuckGo using Zenserp's high-speed API.

## Description
Connect your **Zenserp** account to any AI agent and harness the power of real-time search intelligence through natural conversation.

### What you can do

- **Organic Search** — Retrieve structured organic results from Google, Bing, Yandex, and DuckDuckGo including titles, URLs, and snippets
- **Image Discovery** — Find high-quality images and retrieve direct source or thumbnail URLs across the major search engines
- **Local Intelligence** — Search Google Maps for business listings, physical addresses, ratings, and reviews for any location
- **News Monitoring** — Retrieve breaking stories and current articles from Google News with precise timestamps and source metadata
- **E-commerce Auditing** — Compare product prices and availability by scraping Google Shopping results into structured JSON
- **Video Search** — Find indexed videos across various platforms through Google Video and YouTube search tools
- **Geographic Precision** — Execute searches with specific location parameters (e.g., 'New York, NY') to see localized results

### How it works

1. Subscribe to this server
2. Enter your Zenserp API Key
3. Start querying global search data through Claude, Cursor, or any MCP-compatible client

No more manual search scraping or proxy management. Your AI agent becomes your global search analyst.

### Who is this for?

- **SEO Specialists** — monitor keyword rankings and analyze search snippets from multiple engines and regions via chat
- **Market Researchers** — collect competitive pricing data from Google Shopping and local business info from Maps
- **Data Scientists** — collect massive search datasets for trend analysis and sentiment feedback monitoring
- **Content Marketers** — find relevant images, videos, and news stories to inform content strategy and distribution


## Available Tools (10)
- **search_duckduckgo**: Retrieves organic search results from DuckDuckGo
- **search_images**: Retrieves image search results from Google
- **search_maps**: Retrieves local business listings and reviews from Google Maps
- **search_news**: Returns articles with titles, snippets, and timestamps.

Retrieves current news articles from Google News
- **search_google**: Provide a query string and optional location (e.g. "New York,NY").

Retrieves organic search results from Google
- **search_shopping**: Retrieves product prices and availability from Google Shopping
- **search_yandex**: Retrieves search results from the Yandex search engine
- **search_youtube**: Retrieves search results directly from the YouTube platform
- **search_bing**: Retrieves organic search results from Microsoft Bing
- **search_videos**: Retrieves video search results from Google Video search


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zenserp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Google for 'best CRM software for small business' and show me the top 5 organic results."

**🤖 AI Agent:**
> I found the top 5 organic results for your query. 1. HubSpot CRM (https://...), 2. Zoho CRM (https://...), 3. Salesforce Essentials (https://...). Would you like me to pull the snippets for any of these?

---

**👤 You:**
> "Find restaurants in 'Austin, TX' using Google Maps and show their ratings."

**🤖 AI Agent:**
> I found several highly-rated restaurants in Austin: 1. Franklin Barbecue (Rating: 4.8, 15k reviews), 2. Uchi (Rating: 4.7, 3k reviews), and 3. Terry Black's BBQ (Rating: 4.8, 12k reviews). Would you like the addresses for any of these?

---

**👤 You:**
> "What are the current news headlines for 'generative AI'?"

**🤖 AI Agent:**
> Retrieving news for 'generative AI'... 1. 'New advancements in LLM reasoning' (Source: TechCrunch, 2h ago), 2. 'AI ethics board releases new guidelines' (Source: Reuters, 5h ago). Would you like to read the snippets for these articles?


## ❓ FAQ

**Q: Can I search for local businesses in a specific city through the agent?**
Yes. The `search_google_maps` tool allows your AI agent to retrieve local business listings, including their ratings, physical addresses, and contact info, helping you perform local market research through chat.

**Q: How do I get product prices from Google Shopping via conversation?**
You can use the `search_google_shopping` tool. Simply provide the product name, and Zenserp will return a structured list of vendor prices and availability to help you audit the e-commerce landscape.

**Q: Is it possible to search on Bing or DuckDuckGo using this server?**
Absolutely. This server includes specialized tools like `search_bing_organic` and `search_duckduckgo_organic`, allowing your agent to retrieve results from multiple search engines for broader data coverage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zenserp](https://vinkius.com/mcp/zenserp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zenserp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zenserp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zenserp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zenserp": {
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
