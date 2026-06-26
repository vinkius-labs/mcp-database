# Kelkoo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kelkoo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Search product offers, compare prices, and explore retail catalogs via Kelkoo.

## Description
Connect your **Kelkoo Group** publisher account to any AI agent to access millions of product offers and shopping data. This MCP server allows your agent to search for products, compare prices across merchants, and explore rich retail catalogs directly.

### What you can do

- **Offer Discovery** — Search for real-time product offers across 39 countries using keywords and categories
- **Price Comparison** — Retrieve detailed price and merchant information for millions of items
- **Catalog Exploration** — Navigate hierarchical category trees and list merchants by country
- **Deal Hunting** — Search for active discount coupons and promotional deals
- **Market Insights** — List supported countries and access performance reporting summaries

### How it works

1. Subscribe to this server
2. Enter your Kelkoo Shopping API v2 JWT Token
3. Start searching and comparing products from Claude, Cursor, or any MCP client

### Who is this for?

- **Shopping Assistants** — Automate price comparison and product discovery for users via natural language
- **E-commerce Analysts** — Quickly query market prices and merchant availability across different regions
- **Content Publishers** — Retrieve offer metadata and coupons to integrate into your shopping guides


## Available Tools (8)
- **list_merchants**: List merchants for a country
- **get_offer_details**: Get details for a specific offer
- **get_reporting_summary**: Get publisher reporting summary
- **search_offers**: Requires a country code (e.g., "us", "uk", "fr") and a search keyword.

Search for product offers on Kelkoo
- **list_categories**: List product categories for a country
- **get_category_tree**: Get the hierarchical category tree
- **list_countries**: List all supported countries
- **search_coupons**: Search for discount coupons


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kelkoo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'iPhone 15' offers in the UK on Kelkoo."

**🤖 AI Agent:**
> I've searched Kelkoo UK and found several offers for 'iPhone 15'. Prices start from £799.00 at 'Amazon UK' and £815.00 at 'Currys'. Would you like more details?

---

**👤 You:**
> "List all shopping categories available in France."

**🤖 AI Agent:**
> I've retrieved the categories for Kelkoo France. Major categories include 'Informatique', 'Image & Son', 'Electroménager', and 'Mode'.

---

**👤 You:**
> "Find active coupons for the US market."

**🤖 AI Agent:**
> I found 12 active coupons for Kelkoo US, including '10% OFF at TechStore' and 'Free Shipping on orders over $50 at FashionHub'.


## ❓ FAQ

**Q: In which countries can I search for offers?**
Kelkoo supports search across 39 countries. Use the `list_countries` tool to see the full list of supported regions and their codes.

**Q: Can I filter results by specific merchants?**
Yes, you can list available merchants for a country using `list_merchants` and then refine your search or explore specific merchant catalogs.

**Q: Is it possible to search for discount coupons?**
Absolutely. Use the `search_coupons` tool with a country code to find active promotional deals and discounts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kelkoo](https://vinkius.com/mcp/kelkoo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kelkoo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kelkoo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kelkoo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kelkoo": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
