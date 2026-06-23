# Crawlbase MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crawlbase)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Scrape and crawl via Crawlbase — perform HTML extraction, handle JS-rendered pages, bypass CAPTCHAs, and scrape social profiles directly from any AI agent.

## Description
Connect your **Crawlbase** (formerly ProxyCrawl) account to any AI agent and take full control of your web scraping and anonymous crawling workflows through natural conversation.

### What you can do

- **Standard Scraper** — Identify bounded routing spaces inside the headless engine to extract explicitly attached HTML content via datacenter proxies
- **JS Rendering** — Discover disconnected physical limits tracking exactly what JS-rendered frames expose to extract exact single-page UI bounds
- **Structured JSON Extraction** — Analyzes specific global bounds driving auto-extraction pipelines to force raw HTTP outputs into structured JSON format strictly
- **Screenshot Capture** — Dispatch automated validation checks to generate valid proxy endpoints returning configured Crawlbase screenshot URLs
- **Specialized Scraping** — Leverage dedicated algorithms for Amazon products, LinkedIn profiles, Facebook pages, and Twitter (X) graph profiles natively
- **Search Engine Discovery** — Explain explicitly mapped proxy lists targeting Google domains to parse SERP limits and bypass CAPTCHAs limitlessly
- **Custom Proxy Management** — Provision highly-available request payloads generating custom proxies with specific headers and crawling logic

### How it works

1. Subscribe to this server
2. Enter your Crawlbase Normal Token and your optional JavaScript Token (found in your Crawlbase Dashboard)
3. Start scraping and crawling from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — extract structured web data and search engine results without writing complex scraping scripts
- **Growth Hackers** — monitor competitor products on Amazon or social profiles on LinkedIn and Twitter in real-time
- **Developers** — test and debug web extraction pipelines and JS-rendering logic through natural conversation
- **Market Researchers** — perform deep web crawls and capture snapshots of target sites for offline analysis


## Available Tools (10)
- **scrape_html**: crawlbase.com` datacenter proxies.

Identify bounded routing spaces inside the Headless Crawlbase Engine
- **scrape_js_rendered**: Retrieve explicit Cloud logging tracing explicit Payload IDs limitlessly
- **scrape_json_format**: Perform structural extraction of properties driving active Fields
- **get_screenshot_link**: Dispatch an automated validation check routing explicit Web Snapshot domains
- **scrape_amazon**: Inspect deep internal arrays mitigating specific E-Commerce constraints
- **scrape_linkedin**: Retrieve the exact structural matching verifying Blueprint constraints
- **scrape_facebook**: Enumerate explicitly attached structured rules exporting active Social Pages
- **scrape_google_serp**: Identify precise active arrays spanning rented Context domains for Search
- **scrape_twitter**: Fetch elaborate explicit mapped limits via Crawlbase X extraction
- **custom_scrape**: Provision a highly-available Request Payload generating Custom proxies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crawlbase** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scrape the price and features from this Amazon product: [Amazon URL]"

**🤖 AI Agent:**
> Amazon scraping complete! I've extracted the following JSON data: Title: 'Eco-Smart Watch', Price: '$199.00', Rating: '4.5 stars', Features: ['Waterproof', 'Sleep tracking', '10-day battery'].

---

**👤 You:**
> "Get Google search results for 'best machine learning platforms 2024'"

**🤖 AI Agent:**
> I've extracted the Google SERP results for your query. Top organic links include 'Top 10 ML Platforms (Site A)', 'The Future of AI (Site B)', and 'Enterprise ML Guide (Site C)'. Would you like the full meta descriptions for these?

---

**👤 You:**
> "Take a screenshot of https://example.com"

**🤖 AI Agent:**
> Screenshot requested! Crawlbase is generating the snapshot. You can access the rendered image at this temporary proxy link: [Crawlbase Screenshot URL].


## ❓ FAQ

**Q: When should I use the JavaScript (JS) Token versus the Normal Token?**
Use the Normal Token for fast, static HTML extraction. Switch to the JavaScript Token when the target site uses frameworks like React or Angular, where content is rendered dynamically in the browser. The 'scrape_js_rendered' tool requires the JS Token to function.

**Q: Can my agent bypass CAPTCHAs while scraping Google or LinkedIn?**
Yes. Crawlbase is built to handle CAPTCHAs and blocks natively. When you use specialized tools like 'scrape_google_serp' or 'scrape_linkedin', the agent routes your requests through Crawlbase's advanced proxy infrastructure to ensure successful data extraction.

**Q: How do I get a structured JSON response instead of raw HTML?**
Use the 'scrape_json_format' tool or the specialized scraper tools (Amazon, LinkedIn, etc.). These trigger Crawlbase's auto-extraction pipelines, which analyze the page structure and return specific data fields in a clean JSON format.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crawlbase](https://vinkius.com/mcp/crawlbase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crawlbase** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crawlbase` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crawlbase** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crawlbase": {
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
