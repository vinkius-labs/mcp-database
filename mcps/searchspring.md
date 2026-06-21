# Searchspring MCP Server

Empower your AI to search, filter, and recommend e-commerce products using the Searchspring (Athos Commerce) catalog API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/searchspring)

## Overview
**Category:** marketing-automation
**Tools Count:** 10

## Description
Connect your **Searchspring** store (now part of Athos Commerce) to any AI agent to interact with your e-commerce product catalog conversationally. Bring enterprise-grade site search and merchandising directly into your AI workflows without manually browsing storefronts.

### What you can do

- **Product Discovery** — Query your catalog using natural language, check stock availability, and pull in high-resolution product images and pricing
- **Merchandising & Filtering** — Narrow down thousands of SKUs using faceted parameters (size, color, brand) or strict price range thresholds instantly
- **Autocomplete Trends** — Expose the exact query suggestions (autocomplete) that your customers are seeing on the front-end to gauge search behavior
- **Catalog Auditing** — Browse through deep category trees or request specific details for a single SKU to verify if product metadata is synced correctly

### How it works

1. Subscribe to this server
2. Enter your unique Searchspring Site ID
3. Start fetching product cards or auditing search logic natively from Claude, Cursor, or any MCP-compatible environment

### Who is this for?

- **E-commerce Managers** — ask the AI to show all out-of-stock items in the 'Mens Shoes' category to identify merchandising gaps
- **Developers** — verify if newly integrated custom JSON facets and sorting rules are being parsed properly by the API before deploying front-end UI changes
- **Customer Support** — quickly lookup an exact SKU to confirm pricing and specs without leaving the chat interface when responding to a customer


## Available Tools
- **search_brand**: Lists products from a specific brand
- **search_category**: g., "Mens>Shoes").

Lists products within a specific category hierarchy
- **search_custom**: Performs a search with custom Searchspring parameters
- **search_filtered**: Format: "key:value,key2:value2".

Performs a filtered product search
- **search_pagination**: Retrieves a specific page of search results
- **search_price_range**: Searches for products within a specific price range
- **search_products**: Searches for products in the Searchspring catalog
- **search_sku**: Retrieves details for a specific product SKU
- **search_sorted**: Format: "key:direction" (e.g., "price:asc").

Performs a sorted product search
- **suggest_queries**: Retrieves autocomplete query suggestions


## Installation & Usage

To install and use the **Searchspring** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/searchspring](https://vinkius.com/mcp/searchspring)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
