# Beauty Product Inventory Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/beauty-product-inventory-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Track and manage beauty product stock levels and usage.

## Description
This MCP server connects AI agents to your beauty product inventory system. It allows for real-time monitoring of stock levels, recording product consumption, and identifying items that need restocking. Use `get_current_stock` to check specific item availability, `record_usage` to subtract used quantities, `check_low_stock_items` to find products below their threshold, and `get_inventory_summary` for a high-level overview of all categories.


## Available Tools (4)
- **get_current_stock**: Answers how much of a specific product is left right now
- **get_inventory_summary**: Provides an overall status of the entire inventory
- **record_usage**: Records the usage of a product and updates inventory
- **check_low_stock_items**: Identifies products that are at or below their restock threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beauty Product Inventory Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much of SKU 'SERUM-123' do I have left?"

**🤖 AI Agent:**
> You have 15 units of SKU 'SERUM-123' remaining in stock.

---

**👤 You:**
> "I just used 2 units of SKU 'CREAM-456'. Update my inventory."

**🤖 AI Agent:**
> Inventory updated. There are now 48 units of SKU 'CREAM-456' remaining.

---

**👤 You:**
> "Which items are low on stock in the Haircare category?"

**🤖 AI Agent:**
> The following items are low on stock: SKU 'SHAMPOO-01' (2 remaining) and SKU 'CONDITIONER-02' (1 remaining).


## ❓ FAQ

**Q: How do I check if a specific serum is low on stock?**
You can use the `get_current_stock` tool with the product's SKU to see its current quantity and whether it is marked as low stock.

**Q: Can I update the inventory after using a product?**
Yes, use the `record_usage` tool by providing the SKU and the amount used to automatically subtract it from the available stock.

**Q: How can I see a summary of all my skincare products?**
Use the `get_inventory_summary` tool and specify the 'Skincare' category to get a total count and quantity overview.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/beauty-product-inventory-manager](https://vinkius.com/en/ai-agent-connect/beauty-product-inventory-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beauty Product Inventory Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `beauty-product-inventory-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beauty Product Inventory Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beauty-product-inventory-manager": {
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
