# VTEX Catalog MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vtex-catalog)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vtex-catalog-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vtex-catalog-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search products, manage SKUs, update stock levels, and explore categories and brands on your VTEX store — all from any AI agent.

## Description
Connect your **VTEX** Catalog API to any AI agent and manage your entire product catalog through natural conversation.

### What you can do

- **Product Search** — Run full-text searches across your product catalog by name, brand ID, or category ID. Returns complete product listings with pricing, availability, and images.
- **Product Details** — Retrieve the full specification sheet of any product by ID, including all associated SKUs, categories, dimensions, and metadata.
- **Product Management** — Create or update products directly from your agent. Send structured product data and have it reflected in your VTEX catalog immediately.
- **SKU Inspection** — Look up specific SKUs with detailed attributes like price, weight, dimensions, EAN, and stock status.
- **Stock Management** — Update the available quantity of any SKU across your logistics warehouses. Adjust inventory in real-time without opening the VTEX Admin.
- **Category & Brand Lookup** — Explore your category tree and brand directory to understand how your catalog is organized and ensure correct product classification.

### How it works

1. Subscribe to this server
2. Enter your VTEX Account Name, App Key, and App Token (found in **Account Settings → Application Keys** in your VTEX Admin)
3. Start managing your catalog from Claude, Cursor, or any MCP-compatible agent

### Who is this for?

- **Catalog Managers** — Search, audit, and update products without navigating through dense VTEX Admin screens.
- **Inventory Teams** — Adjust stock levels across warehouses instantly using plain-language commands.
- **Merchandising Teams** — Explore category hierarchies and brand structures to optimize product placement and discoverability.


## Available Tools
- **get_brand**: Get details of a brand
- **get_category**: Get details of a category
- **get_product**: Get full details of a specific product
- **save_product**: Create or update a product
- **search_products**: Examples: "Coca Cola", "b/1234" (brand ID), "c/5678" (category ID).

Search for products by text, brand, or category
- **get_sku**: Get details of a specific SKU
- **manage_stock**: Update the available quantity of a SKU


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VTEX Catalog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Nike Air Max' in my VTEX catalog"

**🤖 AI Agent:**
> Found **8 products** matching 'Nike Air Max':

1. **Nike Air Max 90** — R$ 799.90 (3 SKUs: White/Black/Grey)
2. **Nike Air Max 270** — R$ 899.90 (2 SKUs: Black/Red)
3. **Nike Air Max Plus** — R$ 1,099.90 (4 SKUs)

Would you like the full specification sheet for any of these, or check stock levels for a specific SKU?

---

**👤 You:**
> "Update the stock of SKU 12345 to 150 units"

**🤖 AI Agent:**
> Stock updated! SKU **12345** now has **150 units** available in your primary warehouse. The previous balance was 23 units. The inventory change is reflected immediately across all VTEX sales channels.

---

**👤 You:**
> "Show me the details of category 5678"

**🤖 AI Agent:**
> Category **5678** — **Running Shoes**

📂 Parent: Shoes (ID: 1234)
🏷️ Active: Yes
📦 Products: 42 products listed
🔗 URL: /shoes/running-shoes

Would you like to list all products in this category or check a specific brand within it?


## Installation & Usage

To install and use the **VTEX Catalog** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vtex-catalog](https://vinkius.com/mcp/vtex-catalog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
