# WooCommerce Inventory Updater MCP Server

This MCP allows your AI agent to surgically update the stock quantity of any product or variation in your WooCommerce store. Perfect for reading supplier spreadsheets and syncing inventory automatically.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/woocommerce-inventory-updater)

## Overview
**Category:** ecommerce
**Tools Count:** 1

## Description
Stop manually copying numbers from your ERP or supplier PDFs into WooCommerce. This MCP gives your AI the exact capability to update product stock quantities on the fly, with zero-trust safety.

### The Superpowers

- **Automated Restocking:** Give Claude a PDF invoice from your supplier and say "Update my store inventory based on these new items". It will extract the data and update WooCommerce for you.
- **Variation Support:** Automatically updates specific sizes or colors if you provide the `variationId` along with the `productId`.
- **Zero-Trust Safety:** The AI can only update the `stock_quantity`. It cannot change prices, delete products, or alter descriptions. A surgical tool for a specific job.


## Available Tools
- **update_woocommerce_inventory**: You must provide the numeric productId and the new stockQuantity. If it is a variable product, you must also provide the variationId.

Updates the inventory (stock quantity) of a WooCommerce product or variation


## Installation & Usage

To install and use the **WooCommerce Inventory Updater** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/woocommerce-inventory-updater](https://vinkius.com/mcp/woocommerce-inventory-updater)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
