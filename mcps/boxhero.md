# BoxHero MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/boxhero)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your inventory via BoxHero — list items, track stock transactions, and handle storage locations directly from any AI agent.

## Description
Connect your **BoxHero** account to any AI agent and orchestrate your inventory management workflows through natural conversation.

### What you can do

- **Item Oversight** — List all items in your inventory, create new ones, and retrieve detailed specifications.
- **Stock Tracking** — Check real-time stock levels and monitor transaction histories (stock-in, stock-out, moves).
- **Location Management** — List all storage locations and warehouses managed in your account.
- **Inventory Adjustments** — Create stock transactions directly to correct inventory levels or record shipments.
- **Attribute Discovery** — Retrieve custom item attributes defined in your catalog.

### How it works

1. Subscribe to this server
2. Enter your BoxHero API Token
3. Start managing your inventory from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **create_item**: Create a new inventory item
- **create_transaction**: Create a new stock transaction (In/Out/Move)
- **delete_item**: Delete an item
- **get_account_info**: Get authenticated user info
- **get_item**: Get details of a specific item
- **list_attributes**: List custom item attributes
- **list_items**: List all inventory items
- **list_locations**: List all storage locations
- **list_transactions**: List inventory transactions (Stock In/Out)
- **update_item**: Update an existing item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BoxHero** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active inventory items."

**🤖 AI Agent:**
> I've retrieved your items. You have 'Wireless Mouse' (Stock: 150), 'Keyboard' (Stock: 80), and 'Monitor' (Stock: 25).

---

**👤 You:**
> "Show the recent stock transactions."

**🤖 AI Agent:**
> Retrieving transactions... I found a 'Stock In' of 50 units for 'Keyboard' and a 'Stock Out' of 2 units for 'Monitor' today.

---

**👤 You:**
> "List the storage locations."

**🤖 AI Agent:**
> Your current locations are 'Main Warehouse', 'Store Room A', and 'Return Processing'.


## ❓ FAQ

**Q: Can I check the stock level of a specific item?**
Yes! Use the `get_item` tool with the Item ID. Your agent will fetch the detailed information, including the current total quantity in stock.

**Q: How do I list my storage locations?**
Simply ask the agent to `list_locations`. It will retrieve the directory of all active warehouses and zones.

**Q: Does the integration allow registering a new stock delivery?**
Yes. Use the `create_transaction` tool with type 'IN' to log incoming stock, specifying the items and quantities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boxhero](https://vinkius.com/mcp/boxhero)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BoxHero** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `boxhero` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BoxHero** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "boxhero": {
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
