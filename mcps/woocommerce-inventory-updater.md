# WooCommerce Inventory Updater MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/woocommerce-inventory-updater)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/woocommerce-inventory-updater-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/woocommerce-inventory-updater-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

This MCP allows your AI agent to surgically update the stock quantity of any product or variation in your WooCommerce store. Perfect for reading supplier spreadsheets and syncing inventory automatically.

## Description
Stop manually copying numbers from your ERP or supplier PDFs into WooCommerce. This MCP gives your AI the exact capability to update product stock quantities on the fly, with zero-trust safety.

### The Superpowers

- **Automated Restocking:** Give Claude a PDF invoice from your supplier and say "Update my store inventory based on these new items". It will extract the data and update WooCommerce for you.
- **Variation Support:** Automatically updates specific sizes or colors if you provide the `variationId` along with the `productId`.
- **Zero-Trust Safety:** The AI can only update the `stock_quantity`. It cannot change prices, delete products, or alter descriptions. A surgical tool for a specific job.


## Available Tools
- **update_woocommerce_inventory**: You must provide the numeric productId and the new stockQuantity. If it is a variable product, you must also provide the variationId.

Updates the inventory (stock quantity) of a WooCommerce product or variation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WooCommerce Inventory Updater** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Update the stock of product 402 to 150 units."

**🤖 AI Agent:**
> I've successfully updated the inventory for Product #402. The new stock quantity is 150 (Status: instock).


## Installation & Usage

To install and use the **WooCommerce Inventory Updater** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/woocommerce-inventory-updater](https://vinkius.com/mcp/woocommerce-inventory-updater)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
