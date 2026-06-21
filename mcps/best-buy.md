# Best Buy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/best-buy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/best-buy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/best-buy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search products, check store availability, read reviews, and explore categories via Best Buy — execute retail inquiries directly from any AI agent.

## Description
Connect the **Best Buy API** to any AI agent and bring the entire consumer electronics catalog into your conversational workflow.

### What you can do

- **Product Discovery** — Search for laptops, TVs, and electronics using advanced filters like brand, price, and features.
- **Store Availability** — Check real-time inventory for specific SKUs at local stores using ZIP codes or store IDs.
- **Ratings & Reviews** — Fetch aggregated user reviews and detailed product ratings to inform purchasing decisions.
- **Category Navigation** — Browse through Best Buy's massive category hierarchy to map products or find related items.

### How it works

1. Subscribe to this server
2. Enter your API credentials (get your API Key from **developer.bestbuy.com → My Apps**)
3. Start fetching retail data and availability directly from Claude, Cursor, or any MCP-compatible client

No more scraping websites or building custom integrations. Your AI acts as a dedicated retail analyst and personal shopper.

### Who is this for?

- **E-commerce Analysts** — instantly compare pricing and match competitor catalogs without leaving your workspace.
- **Developers** — fetch clean, structured product data and images straight from the code editor to build affiliate apps.
- **Personal Shoppers** — automate the process of finding the best-rated electronics available near you today.


## Available Tools
- **get_also_viewed_products**: Get recommended or also-viewed products for a SKU
- **get_category_by_id**: Get detailed child categories for a given category ID
- **get_open_box_products**: Can be optionally filtered by category ID.

Fetch open-box discounted products
- **get_product_reviews**: Fetch user reviews and ratings for a product
- **get_product_by_sku**: Get detailed specification for a specific product SKU
- **get_store_details**: Get full details for a specific Best Buy store
- **get_trending_products**: Get trending and highly rated products
- **list_categories**: List top-level Best Buy categories
- **search_products**: Search for products in the Best Buy catalog
- **search_stores**: Search for Best Buy stores near a location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Best Buy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for OLED TVs made by LG under $1500."

**🤖 AI Agent:**
> I found 3 LG OLED models matching your parameters. The 'LG C3 Series 55-Inch' is currently on sale for $1299.00 with a 4.8 star rating across 400 reviews. Would you like the full specs?

---

**👤 You:**
> "Check if SKU 6537363 is in stock at the store in ZIP code 10001."

**🤖 AI Agent:**
> Checking local inventory... Good news, SKU 6537363 (Sony A7 IV Camera) is currently 'In Stock' at the Chelsea, NY store. You can reserve this item for order pickup today.

---

**👤 You:**
> "Give me the top user reviews for the Dyson Airwrap."

**🤖 AI Agent:**
> Gathering feedback metrics... The Dyson Airwrap maintains a 4.6 average. Positive reviews frequently highlight 'drying speed' and 'heat protection', while negative ones cite 'steep learning curve' and price. Want to see the exact text of the top 3 critical reviews?


## Installation & Usage

To install and use the **Best Buy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/best-buy](https://vinkius.com/mcp/best-buy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
