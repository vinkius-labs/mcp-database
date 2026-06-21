# ItemPath MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/itempath)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/itempath-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/itempath-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage inventory, materials, and orders via ItemPath API.

## Description
Empower your AI agents to manage your warehouse and inventory with ItemPath. This MCP server allows you to list materials, retrieve order details, track inventory transactions, and view storage locations directly through the ItemPath API. Ideal for automating supply chain operations and stock monitoring.


## Available Tools
- **get_material**: Returns SKU details, storage rules, and quantity-on-hand. Essential for analyzing the status of specific inventory items.

Retrieves details for a specific material
- **get_me**: Use to verify connection health and current user identity.

Gets current authenticated user info
- **get_order**: Returns the list of materials involved, target locations, and picker information. Use this for troubleshooting order fulfillment or providing status updates.

Retrieves details for a specific order
- **list_batches**: Essential for managing perishable goods or regulated materials requiring lot tracking.

Lists all material batches
- **list_calls**: Useful for debugging integrations and monitoring system interaction frequency.

Lists recent API request history
- **list_locations**: Useful for understanding warehouse layout and identifying where specific materials are stored.

Lists all storage locations
- **list_materials**: Returns material names, descriptions, and IDs. Use this to identify products for inventory auditing or order analysis.

Lists all materials in ItemPath
- **list_orders**: Includes order IDs, types, and current status. Essential for monitoring warehouse throughput and workflow.

Lists all orders
- **list_transactions**: Returns timestamps, material IDs, quantity changes, and user IDs. Essential for auditing inventory accuracy and identifying recent stock changes.

Lists all inventory transactions
- **list_users**: Useful for identifying who performed specific inventory transactions.

Lists all system users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ItemPath** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active materials in the warehouse."

**🤖 AI Agent:**
> I'll fetch the list of materials and current stock levels from ItemPath.

---

**👤 You:**
> "Show me the details for order ID 'ORD-123'."

**🤖 AI Agent:**
> I'll retrieve the full details and status for that specific order.

---

**👤 You:**
> "Check recent inventory transactions."

**🤖 AI Agent:**
> I'll look up the recent material movements and transaction history for you.


## Installation & Usage

To install and use the **ItemPath** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/itempath](https://vinkius.com/mcp/itempath)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
