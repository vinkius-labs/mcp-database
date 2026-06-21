# Oxylabs MCP Server

Scrape any website via Oxylabs — extract Google SERPs, Amazon products, Bing and Yandex results, or any arbitrary URL with JS rendering from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/oxylabs)

## Overview
**Category:** developer-tools
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Oxylabs** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oxylabs](https://vinkius.com/mcp/oxylabs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
