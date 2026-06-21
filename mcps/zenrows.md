# ZenRows MCP Server

Scrape HTML, bypass anti-bots, and extract structured data using ZenRows' advanced proxy and browser network.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zenrows)

## Overview
**Category:** developer-tools
**Tools Count:** 10

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


## Installation & Usage

To install and use the **ZenRows** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zenrows](https://vinkius.com/mcp/zenrows)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
