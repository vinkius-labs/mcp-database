# eBay Shopper MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ebay-shopper)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ebay-shopper-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ebay-shopper-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Connect eBay Shopper to any AI agent via MCP.



## Available Tools
- **get_categories**: Optional parentId filters to subcategories. Use this to discover available categories or navigate the eBay catalog structure.

List eBay product categories and subcategories
- **get_item_compatibility**: Essential for auto parts buyers to verify fitment before purchase.

Get vehicle compatibility information for an auto parts listing
- **get_item_details**: The itemId is obtained from search results. Use this to get complete product specs before purchasing or comparing.

Get full details for a specific eBay item by its ID
- **get_item_rating**: Use this for a quick quality assessment without reading individual reviews.

Get aggregated rating summary for an eBay item
- **get_item_reviews**: Returns rating (1-5), review text, reviewer name, and date. Use this to assess product quality and customer satisfaction before buying.

Get customer reviews and ratings for a specific eBay item
- **get_merchant_item_details**: Similar to get_item_details but with merchant-focused data. Use this for inventory research.

Get item details from the merchant perspective
- **search_items**: Returns a list of matching items with title, price, condition, image URL, and item ID. Use optional parameters: limit (max 10), offset (pagination), sort (BestMatch, price, etc.). Ideal for finding products, comparing prices, or discovering available inventory.

Search for items on eBay by keyword, brand, or product name
- **search_by_category**: g., Electronics, Fashion, Motors). Requires categoryId from get_categories endpoint. Useful for browsing specific sections of eBay.

Search for items within a specific eBay category
- **search_by_image**: Useful when you know what something looks like but not its name or model. Returns visually similar items with prices and details.

Search eBay for visually similar items using an image URL
- **get_shipping_estimate**: Use this to calculate total cost before buying.

Get estimated shipping cost and delivery date for an item




## Installation & Usage

To install and use the **eBay Shopper** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ebay-shopper](https://vinkius.com/mcp/ebay-shopper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
