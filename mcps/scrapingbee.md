# ScrapingBee MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scrapingbee)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Scrape websites without getting blocked using headless browsers, proxy rotation, and JavaScript rendering handled for you.

## Description
Connect your **ScrapingBee** account to any AI agent and take full control of your web data extraction and stealth scraping orchestration through natural conversation. ScrapingBee provides a robust scraping API that handles headless browsers, rotating proxies, and automated CAPTCHA solving, and this integration allows you to retrieve raw HTML, take screenshots, and use AI-driven extraction rules directly from your chat interface.

### What you can do

- **Stealth Scraper Orchestration** — Retrieve raw HTML from any website while bypassing anti-bot systems and CAPTCHAs programmatically.
- **JavaScript Rendering Control** — Toggle headless browser rendering to extract data from modern, dynamic SPAs directly from the AI interface.
- **AI-Driven Data Extraction** — Use AI extraction rules to parse complex web pages into structured JSON data via natural language.
- **Premium Proxy Intelligence** — Access residential and premium proxies to scrape high-security websites without risk of IP blocking.
- **Operational Monitoring** — Track system activity and monitor API credit consumption using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your ScrapingBee API Key from your dashboard
3. Start scraping and extracting web data from Claude, Cursor, or any MCP-compatible client

No more managing browser clusters or rotating proxy pools. Your AI acts as a dedicated data engineer or automation coordinator.

### Who is this for?

- **Market Researchers** — quickly retrieve competitor pricing and product data without dealing with technical blocks.
- **Growth Engineers** — automate the extraction of lead metadata from high-security platforms via natural conversation.
- **Data Analysts** — streamline the conversion of dynamic web pages into structured datasets directly within the chat.


## Available Tools
- **extract_data**: Extract structured data from a page
- **get_usage**: Get current API usage and remaining credits
- **extract_data_with_ai**: Extract JSON data using natural language
- **extract_structured_data**: Extract JSON data using CSS/XPath selectors
- **scrape_webpage**: Automatically handles JavaScript, proxies, and anti-bot measures.

Scrape a webpage with full browser rendering
- **take_screenshot**: Handles rendering automatically.

Capture a screenshot of a website
- **get_api_usage**: Check API credit usage
- **scrape_with_js**: Scrape a page with JavaScript rendering enabled
- **scrape_with_proxy**: Scrape a page using premium proxy rotation
- **scrape_with_stealth**: Scrape a page with stealth mode to bypass bot detection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ScrapingBee** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the names and prices of all laptops from 'https://example.com/computers' using AI."

**🤖 AI Agent:**
> Processing AI extraction... I've retrieved 8 laptops. 'Model X' is $1,200 and 'Model Y' is $950. Should I format this data into a comparison table?

---

**👤 You:**
> "Scrape a Google search results page for the query 'best project management tools 2025' and extract the top 10 results."

**🤖 AI Agent:**
> Google SERP scraped successfully. Query: "best project management tools 2025". Top 10 organic results extracted. #1: "15 Best Project Management Software (2025)" - Forbes. #2: "Top PM Tools Compared" - G2. #3: "Project Management Tool Guide" - Gartner. #4-10: TechRadar, PCMag, Capterra, GetApp, Software Advice, Business News Daily, Zapier. Featured snippet: "Monday.com, Asana, and Jira lead in 2025 rankings". People Also Ask: 4 related questions captured. Ads detected: 3 sponsored results. Credits used: 5.

---

**👤 You:**
> "Extract structured product data from an e-commerce product page using CSS selectors."

**🤖 AI Agent:**
> Data extraction completed. URL: example-store.com/product/wireless-headphones. Selectors used: 5. Results: Product name: "Pro Wireless Headphones X3". Price: $149.99. Original price: $199.99. Discount: 25% off. Rating: 4.7/5 (2,340 reviews). Availability: In Stock. Description: 280 characters extracted. Specifications: 8 key-value pairs (battery life, driver size, frequency response, etc). Images: 6 URLs captured. Related products: 4 items extracted. API credits used: 1.


## ❓ FAQ

**Q: Can my AI automatically extract structured JSON from a web page using ScrapingBee?**
Yes! Use the `extract_data` tool. You can provide standard extraction rules or set `ai=true` to let ScrapingBee's AI models identify and parse the data fields you need automatically.

**Q: How do I use premium or residential proxies for high-security sites?**
Simply include `premium_proxy: true` in your `scrape_general` parameters. This will route your request through residential IPs, making it much harder for anti-bot systems to detect and block.

**Q: How do I find my ScrapingBee API Key?**
Log in to your ScrapingBee dashboard, and your API Key will be clearly visible in the **Credentials** section on the main page.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scrapingbee](https://vinkius.com/mcp/scrapingbee)
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
3. Set Type to "SSE", enter `scrapingbee` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ScrapingBee** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scrapingbee": {
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
