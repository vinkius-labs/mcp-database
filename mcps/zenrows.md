# ZenRows MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zenrows)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Scrape HTML, bypass anti-bots, and extract structured data using ZenRows' advanced proxy and browser network.

## Description
Connect your **ZenRows** account to any AI agent and harness the power of industrial-grade web scraping through natural conversation.

### What you can do

- **Universal Scraping** — Retrieve raw HTML from any website while ZenRows automatically rotates proxies and handles CAPTCHAs
- **JavaScript Rendering** — Scrape dynamic SPAs and complex web apps by using a headless browser to capture the full rendered state
- **Anti-Bot Bypass** — Effortlessly bypass sophisticated protections like Cloudflare, DataDome, and PerimeterX with specialized bypass technology
- **Markdown Conversion** — Automatically convert web pages into clean Markdown, ideal for LLM ingestion and RAG applications
- **Structured Data** — Use auto-parse to extract JSON data from major e-commerce, search, and social platforms without manual selectors
- **Visual Previews** — Generate real-time screenshots of target pages to verify rendering or monitor visual changes
- **Geographic Targeting** — Execute scrapes using high-anonymity residential proxies from specific countries for localized content

### How it works

1. Subscribe to this server
2. Enter your ZenRows API Key
3. Start extracting web data through Claude, Cursor, or any MCP-compatible client

No more manual proxy rotation or CAPTCHA solving. Your AI agent becomes your web data architect.

### Who is this for?

- **Data Engineers** — automate web scraping pipelines and bypass aggressive bot detections through simple chat commands
- **AI Researchers** — quickly collect clean Markdown datasets for model training and fine-tuning
- **Market Analysts** — monitor global product pricing and availability across different regions via residential proxies
- **SEO Specialists** — analyze rendered page content and verify technical SEO data across complex dynamic websites


## Available Tools
- **scrape_geo**: g. "us", "gb") for localized content.

Scrape using a proxy from a specific country
- **scrape_custom**: g. wait, css_extractor, session_id).

Execute a scrape using advanced custom parameters
- **scrape_html**: ZenRows automatically rotates proxies and handles CAPTCHAs.

Scrape raw HTML using ZenRows anti-bot proxy pool
- **scrape_js**: Enables js_render=true. Slower and more expensive than static scraping.

Scrape JS-rendered HTML using ZenRows headless browser
- **scrape_antibot**: Enables js_render and antibot=true.

Scrape with full anti-bot bypass for heavily protected sites
- **scrape_premium**: Sets premium_proxy=true for higher anonymity.

Scrape using ZenRows premium residential proxies
- **scrape_autoparse**: Scrape with automatic structured data extraction
- **get_screenshot**: Generates a URL that returns a screenshot of the target page
- **scrape_markdown**: Automatically removes boilerplate like navigation and ads.

Scrape and convert page content to clean Markdown
- **scrape_wait**: g. "#results") to wait for before capturing the HTML.

Scrape with JS render waiting for a specific CSS selector


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ZenRows** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scrape 'https://example.com' and return the content in Markdown."

**🤖 AI Agent:**
> I've retrieved the page content and converted it to clean Markdown. Here is the structured text, with all ads and navigation boilerplate removed for your review.

---

**👤 You:**
> "Bypass Cloudflare and scrape the rendered HTML of 'https://protected-site.com'."

**🤖 AI Agent:**
> Cloudflare protection successfully bypassed. I've used a headless browser to render the JavaScript and captured the full HTML state for you. What data points would you like me to analyze from this source?

---

**👤 You:**
> "Get a screenshot of 'https://news-portal.com/breaking-news'."

**🤖 AI Agent:**
> Screenshot generated successfully. You can view the fully rendered page here: https://zenrows.com/screenshot/.... Would you like me to extract the text content from this page as well?


## ❓ FAQ

**Q: Can ZenRows bypass Cloudflare or other aggressive bot protections?**
Yes. Using the `scrape_antibot` tool, ZenRows activates specialized technology to bypass Cloudflare, DataDome, and other advanced bot detection systems, ensuring you can access the content you need through chat.

**Q: How do I get clean Markdown from a website for my AI agent?**
You can use the `scrape_markdown` tool. ZenRows will retrieve the page and automatically convert the content into structured Markdown, removing ads and navigation headers to provide a clean input for LLMs.

**Q: Can I see what a dynamic page looks like before extracting data?**
Absolutely. Use the `get_screenshot` tool to retrieve a direct link to an image file representing the fully rendered target page, helping you verify that JavaScript content is correctly displayed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zenrows](https://vinkius.com/mcp/zenrows)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ZenRows** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zenrows` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ZenRows** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zenrows": {
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
