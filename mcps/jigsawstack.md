# JigsawStack MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jigsawstack)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/jigsawstack-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/jigsawstack-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access a suite of AI utility APIs for web scraping, translation, OCR, and sentiment analysis in one developer-friendly platform.

## Description
Connect your **JigsawStack** account to any AI agent and access AI-powered utilities through natural conversation.

### What you can do

- **Web Scraping** — Extract structured data from any web page using AI
- **Text-to-SQL** — Generate SQL queries from natural language descriptions
- **Translation** — Translate text between multiple languages
- **Data Validation** — Validate emails, phone numbers, and other data formats
- **Geocoding** — Convert addresses to coordinates and reverse geocode
- **Image Processing** — Analyze and process images with AI

### How it works

1. Subscribe to this server
2. Enter your JigsawStack API Key
3. Start using AI utilities from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — integrate AI scraping, translation, and data validation
- **Data Teams** — generate SQL from natural language and geocode addresses
- **Automation Engineers** — build AI-powered data pipelines


## Available Tools
- **ai_web_scrape**: Scrape a website using natural language
- **check_nsfw_image**: Check if an image is NSFW
- **check_profanity_text**: Check text for profanity
- **summarize_text**: Summarize long text content
- **translate_text**: Translate text between languages
- **extract_text_from_image**: Perform vOCR on an image URL
- **ai_web_search**: Perform an AI-powered web search


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JigsawStack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scrape the top 10 products from this e-commerce page and validate the contact emails."

**🤖 AI Agent:**
> Scraped 10 products from example-shop.com. 1) 'Wireless Headphones' ($79.99, 4.5★). 2) 'Smart Watch' ($199.99, 4.8★). 3) 'USB-C Hub' ($34.99, 4.2★). Emails validated: contact@shop.com ✅ valid, support@shop.com ✅ valid, info@shop.com ⚠️ catch-all.

---

**👤 You:**
> "Generate a SQL query to find the top 5 customers by revenue and geocode their addresses."

**🤖 AI Agent:**
> SQL generated: `SELECT c.name, SUM(o.total) as revenue FROM customers c JOIN orders o ON c.id = o.customer_id GROUP BY c.id ORDER BY revenue DESC LIMIT 5`. Geocoded: 1) '123 Main St, NYC' → 40.7128, -74.0060. 2) '456 Market St, SF' → 37.7749, -122.4194. 3) '789 Michigan Ave, Chicago' → 41.8781, -87.6298.

---

**👤 You:**
> "Translate this product description to Spanish, French, and Portuguese."

**🤖 AI Agent:**
> Translations complete! ES: 'Transforma tus datos en insights accionables con nuestra plataforma de analytics.' FR: 'Transformez vos données en insights actionnables avec notre plateforme d'analytics.' PT: 'Transforme seus dados em insights acionáveis com nossa plataforma de analytics.' All 3 translations delivered with natural phrasing.


## Installation & Usage

To install and use the **JigsawStack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jigsawstack](https://vinkius.com/mcp/jigsawstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
