# Oxylabs SERP MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/oxylabs-serp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-infrastructure](../categories/data-infrastructure.md)

Extract structured search engine results via Oxylabs — scrape Google, Bing, Yandex, Baidu, and YouTube rankings directly from your AI agent.

## Description
Bring the **Oxylabs SERP Scraper API** directly into your AI workflows. Perform high-volume, structured data extraction across all major search engines without worrying about proxy rotation, CAPTCHAs, or HTML parsing.

### What you can do

- **Google Ecosystem** — Extract parsed data from Google Search (organic, snippets), Google Images, Google News, Google Shopping, Google Scholar, and Google Travel/Hotels
- **Bing Search** — Extract organic search rankings and rich snippets from Microsoft Bing
- **Yandex Search** — Scrape the leading Russian search engine for regional SEO analysis
- **Baidu Search** — Extract search engine results pages from China's leading search provider
- **YouTube Search** — Parse video rankings, channel details, and views from YouTube search results

### How it works

1. Subscribe to this server
2. Enter your Oxylabs Username and Password
3. Start fetching structured SERP data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SEO professionals** — track keyword rankings and analyze SERP features across multiple global search engines
- **Market researchers** — monitor Google Shopping prices, hotel rates on Google Travel, or academic papers on Scholar
- **Content strategists** — analyze YouTube video rankings and news syndication across global domains


## Available Tools
- **baidu_search**: Inspect deep internal arrays mitigating specific Plan Math
- **bing_search**: Dispatch an automated validation check routing explicit Gateway history
- **google_search**: Identify bounded CRM records inside the Headless Oxylabs SERP Platform
- **google_images_search**: Perform structural extraction of properties driving active Account logic
- **google_news_search**: Provision a highly-available JSON Payload generating hard Customer bindings
- **google_scholar_search**: Irreversibly vaporize explicit validations extracting rich Churn flags
- **google_shopping_search**: Retrieve explicit Cloud logging tracing explicit Vault limits
- **google_travel_search**: Enumerate explicitly attached structured rules exporting active Billing
- **yandex_search**: Identify precise active arrays spanning native Gateway auth
- **youtube_search**: Identify precise active arrays spanning native Hold parsing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Oxylabs SERP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Google for 'best enterprise LLMs' and summarize the top organic results."

**🤖 AI Agent:**
> Found the top organic results for 'best enterprise LLMs'. 1: Gartner's Magic Quadrant noting OpenAI, Anthropic, and Cohere. 2: Forbes review of private vector RAG implementations. 3: IBM's Granite LLM documentation highlighting data governance. Want me to dive deeper into any of these articles?

---

**👤 You:**
> "Check Google Travel for hotels in Tokyo next weekend."

**🤖 AI Agent:**
> Queried google_travel_search for 'hotels in Tokyo'. Returned highly rated results including The Ritz-Carlton Tokyo ($890/night), Shinjuku Washington Hotel ($120/night), and Hotel Gracery Shinjuku ($150/night). Would you like me to filter by rating or specific amenities?

---

**👤 You:**
> "Search YouTube for 'Next.js 15 tutorials'."

**🤖 AI Agent:**
> I've pulled the youtube_search results. Top videos are: 1. 'Next.js 15 Crash Course' by Traversy Media (500K views, uploaded 1 mo ago). 2. 'What's new in Next 15?' by Vercel (1.2M views). 3. 'Next.js App Router Masterclass' by Lee Robinson. Want the direct links to these videos?


## ❓ FAQ

**Q: Are the exported results structured JSON or raw HTML?**
The API returns highly structured, pre-parsed JSON. For example, a Google Search request directly returns organized arrays of organic results, related queries, ads, and knowledge panels — there's no need to write code to parse the HTML DOM.

**Q: Do I need to manage my own residential proxies?**
No. Oxylabs handles all infrastructure on the backend, automatically rotating residential proxies, fingerprinting, and bypassing CAPTCHAs. You just provide the search query.

**Q: Can I search Google News for PR tracking?**
Yes, the google_news_search tool natively queries the News tab, returning structured articles with publishers, titles, snippets, and exact publication timestamps, making it highly effective for PR and brand tracking.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oxylabs-serp](https://vinkius.com/mcp/oxylabs-serp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Oxylabs SERP** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `oxylabs-serp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Oxylabs SERP** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oxylabs-serp": {
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
