# WooCommerce Inventory Updater MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/woocommerce-inventory-updater)
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


## ❓ FAQ

**Q: Will it enable stock management if it is turned off?**
Yes. When this tool updates the quantity, it automatically sends `manage_stock: true` to the WooCommerce API, ensuring the new stock quantity is actually tracked by the system.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/woocommerce-inventory-updater](https://vinkius.com/mcp/woocommerce-inventory-updater)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WooCommerce Inventory Updater** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `woocommerce-inventory-updater` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WooCommerce Inventory Updater** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "woocommerce-inventory-updater": {
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
