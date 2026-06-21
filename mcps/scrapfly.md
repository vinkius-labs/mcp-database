# Scrapfly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scrapfly)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/scrapfly-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/scrapfly-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Scrape web data at scale with a managed API that handles proxies, browser rendering, and anti-bot bypassing automatically.

## Description
Connect your **Scrapfly** account to any AI agent and take full control of your web data extraction and scraping orchestration through natural conversation. Scrapfly provides a professional-grade scraping API that combines headless browser rendering, premium residential proxies, and AI-driven data extraction, and this integration allows you to retrieve raw HTML, take element-level screenshots, and convert pages into structured JSON directly from your chat interface.

### What you can do

- **Stealth Scraper Orchestration** — Retrieve clean HTML from any website while bypassing Cloudflare, Akamai, and other anti-bot systems programmatically.
- **AI-Driven Data Extraction** — Use LLM-powered extraction models to transform complex web pages into structured JSON data directly from the AI interface.
- **Visual Intelligence** — Capture full-page or element-specific screenshots with support for dark mode and ad-blocking via natural language.
- **Proxy & Region Control** — Access millions of residential proxies across 50+ countries to ensure your data collection is always localized and reliable.
- **Operational Monitoring** — Track system activity, monitor API credit consumption, and manage project metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Scrapfly API Key from your dashboard
3. Start scraping and extracting web data from Claude, Cursor, or any MCP-compatible client

No more managing browser clusters or rotating IPs. Your AI acts as a dedicated data engineer or market researcher.

### Who is this for?

- **Data Scientists** — quickly retrieve high-fidelity datasets from the web without technical blocks.
- **Market Researchers** — automate the extraction of competitor pricing and sentiment data via natural conversation.
- **Growth Engineers** — streamline the generation of visual audits and lead metadata directly within the chat.


## Available Tools
- **ai_data_extraction**: Extract structured data
- **get_api_status**: Check account info
- **list_extraction_models**: List AI models
- **get_project_details**: Get project info
- **get_scraping_capabilities**: Check scraping features
- **get_screenshot_capabilities**: Check screenshot features
- **check_credit_usage**: Check usage stats
- **list_proxy_regions**: Check proxy options
- **list_api_webhooks**: List configured webhooks
- **web_scrape**: Scrape any website
- **capture_screenshot**: Take a website screenshot
- **test_scrapfly_auth**: Verify credentials


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scrapfly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scrape the homepage of 'https://news.ycombinator.com' and return the HTML."

**🤖 AI Agent:**
> Retrieving website content... I've successfully scraped Hacker News. Should I extract the top story titles and links for you?

---

**👤 You:**
> "Scrape the product listings from the first 3 pages of an e-commerce category with pricing data."

**🤖 AI Agent:**
> Scraping completed across 3 pages. Total products extracted: 72 (24 per page). Data fields: product name, price, original price, discount %, rating, review count, availability, SKU. Price range: $12.99 - $299.99. Average price: $67.40. 18 products on sale (25% of listings). 5 products out of stock. Anti-bot protection bypassed successfully. JavaScript rendering used for dynamic content. Total API credits used: 6. Data exported as JSON (234 KB).

---

**👤 You:**
> "Take a full-page screenshot of our competitor's pricing page and extract the plan details."

**🤖 AI Agent:**
> Full-page screenshot captured: competitor_pricing_may2025.png (2400x8600px). Plan details extracted: Starter ($29/mo, 1 user, 5GB storage), Professional ($79/mo, 5 users, 50GB, API access), Enterprise ($199/mo, unlimited users, 500GB, priority support, SSO). Annual discount: 20% across all plans. Free trial: 14 days. Compared to your pricing: you are 15% lower on Starter, comparable on Professional, 10% higher on Enterprise. New feature since last check: AI assistant added to Professional tier.


## Installation & Usage

To install and use the **Scrapfly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scrapfly](https://vinkius.com/mcp/scrapfly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
