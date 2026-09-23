# Cleaning Product Inventory Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cleaning-product-inventory-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Manage and audit cleaning supply inventories with real-time stock tracking.

## Description
This MCP server provides tools to manage cleaning supply inventories. You can use `get_inventory_summary` to view current stock levels across categories, `add_product_stock` to increase quantities of specific items, `verify_stock_accuracy` to audit inventory against expected counts, and `get_product_details` to retrieve measurement units and classifications.


## Available Tools (4)
- **add_product_stock**: Increases the stock level of an existing cleaning product
- **get_inventory_summary**: Provides a high-level overview of all cleaning products currently in the system
- **get_product_details**: Retrieves the specific measurement unit and classification for a single product
- **verify_stock_accuracy**: Compares the current system stock against a user-provided target value


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cleaning Product Inventory Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current stock level for Sanitizers?"

**🤖 AI Agent:**
> The current stock for Sanitizers includes: All-Purpose Cleaner: 50 liters, Glass Cleaner: 20 liters.

---

**👤 You:**
> "I just received 10 more bottles of Glass Cleaner. Please update the stock."

**🤖 AI Agent:**
> The stock for Glass Cleaner has been updated. The new total quantity is 30 liters.

---

**👤 You:**
> "Check if my All-Purpose Cleaner stock is correct. I should have 45 liters."

**🤖 AI Agent:**
> The audit for All-Purpose Cleaner shows a current quantity of 50 liters. This is a SURPLUS of 5 liters compared to your expected 45 liters.


## ❓ FAQ

**Q: How can I see all my current cleaning supplies?**
You can use the `get_inventory_summary` tool to see a high-level overview of all products currently in the system.

**Q: How do I report a shortage in my stock?**
Use the `verify_stock_accuracy` tool. It compares your current system stock against your physical count and will identify if there is a shortage.

**Q: Can I add new stock to an existing product?**
Yes, use the `add_product_stock` tool to increase the quantity of an existing product in the inventory.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cleaning-product-inventory-manager](https://vinkius.com/en/ai-agent-connect/cleaning-product-inventory-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cleaning Product Inventory Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cleaning-product-inventory-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cleaning Product Inventory Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cleaning-product-inventory-manager": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
