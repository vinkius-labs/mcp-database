# Klevu (E-commerce AI Search) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/klevu-e-commerce-ai-search)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/klevu-e-commerce-ai-search-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/klevu-e-commerce-ai-search-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Power your e-commerce discovery via Klevu AI — execute keyword searches, manage category merchandising, and retrieve product recommendations.

## Description
Connect your **Klevu** account to any AI agent and take full control of your e-commerce search foundation and product discovery through natural conversation.

### What you can do

- **AI Keyword Search** — Execute high-relevancy keyword searches against your product catalog, categories, and CMS pages directly from your agent
- **Category Merchandising** — Retrieve products configured for specific category navigation paths to audit smart merchandising rules and display sequences
- **Facet & Filter Analytics** — Perform complex filtered searches using explicit facets like color, size, or brand to identify specific product segments
- **Predictive Autocomplete** — Access fast autocomplete suggestions and popular product matches based on partial search terms to improve UX navigation
- **ML Recommendations** — Fetch visually similar, frequently bought together, or trending product recommendations driven by Klevu's machine learning models
- **Trending Intelligence** — Monitor global product velocity and relevance to identify top-selling items and seasonal trends across your entire store
- **Raw API Access** — Execute custom JSON search payloads for deeply nested query configurations and specific V2 API settings

### How it works

1. Subscribe to this server
2. Enter your Klevu Search URL and API Key
3. Start optimizing your product discovery from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Developers** — test search relevance and category API results through natural conversation without manual Postman queries
- **Digital Merchandisers** — audit product rankings and recommendation logics across multiple categories and store views efficiently
- **Data Analysts** — monitor trending products and search performance to identify market opportunities and catalog gaps


## Available Tools
- **search_autocomplete**: Fetch search autocomplete suggestions as the user types
- **search_category**: Retrieve products for a specific category page (Smart Category Merchandising)
- **search_filtered**: g., color, size, brand) applied to narrow down the result set.

Search the Klevu catalog with specific facet filters applied
- **search_keyword**: Search catalog by keyword using Klevu AI
- **search_pagination**: Retrieve paginated results for a search query
- **search_product_id**: Retrieve details for a specific catalog product by ID
- **search_raw**: Execute a custom JSON search payload against the Klevu API
- **search_recs**: Fetch Klevu AI product recommendations
- **search_sorted**: Perform a keyword search with a custom sorting order
- **search_trending**: View currently trending and most relevant global products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Klevu (E-commerce AI Search)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'waterproof jackets' in my Klevu catalog"

**🤖 AI Agent:**
> Searching catalog… I've found 12 waterproof jackets. Top results include the 'Summit Pro Hardshell', 'RainGuard Trail Jacket', and 'Urban Explorer Parka'. Prices range from $89 to $245. Would you like to filter these by size or brand?

---

**👤 You:**
> "Show me trending products for the 'Home Decor' category"

**🤖 AI Agent:**
> Retrieving trending items for 'Home Decor'… Current top sellers include 'Minimalist Ceramic Vase', 'Boho Woven Throw', and 'Smart Ambient Lamp'. These items are showing high engagement over the last 24 hours. Would you like to see visual similar items?

---

**👤 You:**
> "Execute a filtered search for 'sneakers' with brand 'Nike'"

**🤖 AI Agent:**
> Filtering search for Nike sneakers… Found 8 matches. Featured models: 'Air Max Pulse', 'Dunk Low Retro', and 'Zoom Fly 5'. Would you like me to sort these by price from lowest to highest?


## Installation & Usage

To install and use the **Klevu (E-commerce AI Search)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/klevu-e-commerce-ai-search](https://vinkius.com/mcp/klevu-e-commerce-ai-search)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
