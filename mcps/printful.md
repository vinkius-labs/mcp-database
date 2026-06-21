# Printful MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/printful)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/printful-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/printful-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Access Printful's product catalog — list products, inspect variants, and retrieve detailed size guides directly from any AI agent.

## Description
Connect your **Printful** account to any AI agent to browse the extensive Print-on-Demand catalog and retrieve technical product specifications through natural conversation.

### What you can do

- **Product Discovery** — List available products in the Printful catalog, with the ability to filter by specific category IDs.
- **Detailed Inspection** — Fetch comprehensive metadata for specific products, including descriptions and available variants.
- **Variant Analysis** — Get precise details for individual variants, including size, color, pricing, and stock status using Variant IDs.
- **Size Guides** — Retrieve accurate size tables in both inches and centimeters to ensure perfect fit for your customers.

### How it works

1. Subscribe to this server
2. Enter your Printful API Token
3. Start exploring the catalog from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Store Owners** — quickly check product availability and variant details without navigating the Printful dashboard.
- **Designers & Merchandisers** — verify size guides and color options while planning new collections.
- **Developers** — retrieve technical IDs for products and variants directly within your coding environment.


## Available Tools
- **get_product**: Get details for a specific Printful product
- **list_products**: Can be filtered by category ID.

List Printful products
- **get_product_sizes**: Get size guides for a Printful product
- **get_variant**: Always use Variant IDs for orders.

Get details for a specific Printful variant


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Printful** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 10 products from the Printful catalog."

**🤖 AI Agent:**
> I've retrieved the latest products. You have items like the 'Unisex Staple T-Shirt' (ID: 71) and the 'Enhanced Matte Paper Poster' (ID: 1). Would you like to see the variants for any of these?

---

**👤 You:**
> "What are the available sizes and colors for product ID 71?"

**🤖 AI Agent:**
> For the Unisex Staple T-Shirt (ID: 71), there are multiple variants. Common colors include Black, White, and Navy, with sizes ranging from S to 3XL. I can fetch the specific Variant ID for a 'Black / L' if you need to check stock.

---

**👤 You:**
> "Show me the size guide for product 71 in centimeters."

**🤖 AI Agent:**
> The size guide for product 71 (Unisex Staple T-Shirt) in cm is: S (Width: 45.7, Length: 71.1), M (Width: 50.8, Length: 73.7), L (Width: 55.9, Length: 76.2). Would you like the measurements for larger sizes as well?


## Installation & Usage

To install and use the **Printful** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/printful](https://vinkius.com/mcp/printful)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
