# Oxylabs MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/oxylabs)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/oxylabs-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/oxylabs-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Scrape any website via Oxylabs — extract Google SERPs, Amazon products, Bing and Yandex results, or any arbitrary URL with JS rendering from any AI agent.

## Description
Give your AI agent the ability to extract structured data from any website with **Oxylabs Web Scraping API**. Scrape Google, Amazon, Bing, and Yandex with specialized parsers, or hit any arbitrary URL with the universal scraper — with optional headless browser rendering.

### What you can do

- **Universal Scraper** — Extract HTML from any website. Enable JS rendering for single-page apps that require client-side execution
- **Google Search** — Parse Google SERPs with organic rankings, knowledge panels, ads, and featured snippets, localized by country TLD
- **Google Shopping** — Extract product listings with merchants, prices, reviews, and availability from Google Shopping
- **Google Images** — Pull image URLs, dimensions, and hosting origins from Google Image Search
- **Google News** — Extract time-indexed news articles with publishers and publication dates
- **Amazon Search** — Scrape Amazon product listings with ASINs, prices, Prime markers, and seller data across regional domains
- **Amazon Product** — Deep-extract individual product pages with variations, stock states, bullet points, and vendor hierarchies
- **Bing Search** — Parse Bing SERPs with organic web graph snippets
- **Yandex Search** — Extract rankings from the Yandex search engine for CIS/RU market analysis
- **Custom Payload** — Send fully customized Oxylabs schema payloads for advanced proxy and location configurations

### How it works

1. Subscribe to this server
2. Enter your Oxylabs Username and Password
3. Start scraping from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SEO teams** — track keyword rankings across Google, Bing, and Yandex without managing proxy infrastructure
- **E-commerce analysts** — monitor competitor pricing and product availability on Amazon across regional markets
- **Data engineers** — extract structured web data at scale for market research, lead generation, or content indexing


## Available Tools
- **scrape_universal**: oxylabs.io/v1/queries` endpoint mapping `source=universal`. Dynamically extracts raw remote HTML safely avoiding proxy blocks. Use `js_render=true` explicitly if the target SPA strictly requires client rendering.

Scrape any arbitrary HTML website using Oxylabs Universal Scraper API
- **scrape_google_serp**: Extract Google Search Engine Results Page (SERP) blocks structurally
- **scrape_google_shopping**: Extract E-Commerce structures hitting Google Shopping engines
- **scrape_google_images**: Parse and Scrape specific Google Image Search layout blocks
- **scrape_google_news**: Export time-indexed News articles via Google News blocks
- **scrape_amazon_search**: Perform structured data extraction looping over Amazon query listings
- **scrape_amazon_product**: Extract deep E-Commerce retail arrays extracting arbitrary Amazon ASINs
- **scrape_bing_serp**: Calculate and extract structured Bing Search Web mappings
- **scrape_yandex_serp**: Execute structural analysis indexing Yandex Search instances
- **scrape_custom_payload**: oxylabs.io/v1/queries` customizing Proxy Types, Locations and deeply nested config params.

Dispatch entirely arbitrary strict Oxylabs Payload JSON structures


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Oxylabs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Google for 'best noise cancelling headphones 2024' and show me the top 5 organic results."

**🤖 AI Agent:**
> Top 5 organic results for 'best noise cancelling headphones 2024': 1) Wirecutter — 'The Best Noise-Canceling Headphones' (score: featured snippet). 2) RTINGS — 'The 8 Best Noise Cancelling Headphones'. 3) TechRadar — 'Best noise-cancelling headphones 2024'. 4) Tom's Guide — 'Best ANC headphones'. 5) CNET — 'Best Noise-Canceling Headphones for 2024'. Want me to scrape any of these pages for full content?

---

**👤 You:**
> "Get the full product details for Amazon ASIN B0C8PSXB2M."

**🤖 AI Agent:**
> Product: Sony WH-1000XM5 Wireless Noise Canceling Headphones. Price: $328.00 (was $399.99 — 18% off). Rating: 4.6/5 (12,847 reviews). Prime: Yes. Colors available: Black, Silver, Midnight Blue. In stock. Key features: 30-hour battery, 8 microphones, touch sensor controls. Sold by Amazon.com. Want me to check pricing on amazon.de or amazon.co.uk?

---

**👤 You:**
> "Scrape the homepage of techcrunch.com with JavaScript rendering enabled."

**🤖 AI Agent:**
> Successfully scraped techcrunch.com with JS rendering. Page title: 'TechCrunch | Startup and Technology News'. Extracted 42 article headlines, 28 author names, 15 featured images, and 8 category tags. Top headline: 'AI startup raises $200M Series C at $2B valuation'. Content size: 245 KB (after rendering). Want me to extract just the article titles and links in a structured format?


## Installation & Usage

To install and use the **Oxylabs** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oxylabs](https://vinkius.com/mcp/oxylabs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
