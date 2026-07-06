# ScrapingAnt MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scrapingant)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Extract web data reliably with rotating proxies, headless Chrome rendering, and CAPTCHA solving built into every request.

## Description
Connect your **ScrapingAnt** account to any AI agent and take full control of your web data extraction and scraping orchestration through natural conversation. ScrapingAnt provides a high-performance scraping API with rotating proxies and headless browser rendering, and this integration allows you to retrieve raw HTML, convert pages to Markdown, and use AI-driven data extraction directly from your chat interface.

### What you can do

- **Stealth Scraper Orchestration** — Retrieve raw HTML or extended page metadata while bypassing anti-bot systems and CAPTCHAs programmatically.
- **Markdown Intelligence** — Extract web page content and automatically transform it into clean Markdown format directly from the AI interface.
- **AI-Driven Data Extraction** — Use AI models to extract structured data from any website by providing a simple prompt or schema via natural language.
- **Browser & Proxy Control** — Configure headless browser settings and proxy types (datacenter or residential) to optimize your scraping success rate.
- **Operational Monitoring** — Track API credit usage and monitor system statistics using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your ScrapingAnt API Key from your dashboard
3. Start extracting web data from Claude, Cursor, or any MCP-compatible client

No more wrestling with IP blocks or complex browser configurations. Your AI acts as a dedicated data engineer or web researcher.

### Who is this for?

- **Data Scientists & Researchers** — quickly retrieve structured data from the web without managing proxy pools.
- **Content Engineers** — automate the conversion of web pages to Markdown for knowledge base synchronization.
- **Growth Hackers** — streamline the extraction of competitor metadata and monitor website changes directly within the chat.


## Available Tools (5)
- **scrape_extended_data**: Scrape webpage with network logs and cookies
- **extract_structured_data**: Extract JSON data using AI
- **scrape_to_markdown**: Ideal for RAG and LLMs.

Scrape webpage directly to Markdown
- **get_api_usage**: Check API credit usage
- **scrape_webpage**: Handles JavaScript, anti-bot, and proxies automatically.

Scrape a webpage with browser rendering


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ScrapingAnt** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the latest product prices from 'https://example.com/shop' using AI."

**🤖 AI Agent:**
> Processing extraction... I've retrieved 5 products from the shop. 'Item A' is $19.99 and 'Item B' is $25.00. Would you like the full JSON results?

---

**👤 You:**
> "Convert the page 'https://example.com/blog/post-1' to Markdown."

**🤖 AI Agent:**
> Retrieving page content... I've successfully converted the blog post to Markdown. It includes the main heading, 3 subheaders, and all body text. Should I save this content for you?

---

**👤 You:**
> "Check my current API credit balance in ScrapingAnt."

**🤖 AI Agent:**
> Fetching usage stats... You have 4,500 credits remaining out of your 5,000 monthly limit. Your plan resets in 12 days.


## ❓ FAQ

**Q: Can my AI automatically convert a web page into Markdown format?**
Yes! Use the `scrape_markdown` tool. Provide the URL, and your agent will return the page content cleanly formatted in Markdown instantly.

**Q: How do I use AI to extract specific data like prices or stock from a site?**
Simply ask the agent to run the `extract_data` action. Provide the URL and a prompt or schema of what you need, and ScrapingAnt's AI models will parse the page for you.

**Q: How do I find my ScrapingAnt API Key?**
Log in to your ScrapingAnt dashboard, and you will find your unique API Key prominently displayed on the main page.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scrapingant](https://vinkius.com/mcp/scrapingant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ScrapingAnt** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scrapingant` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ScrapingAnt** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scrapingant": {
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
