# BoxHero MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/boxhero)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/boxhero-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/boxhero-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **BoxHero** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boxhero](https://vinkius.com/mcp/boxhero)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
