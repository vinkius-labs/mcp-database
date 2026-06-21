# ItemPath MCP Server

Manage inventory, materials, and orders via ItemPath API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/itempath)

## Overview
**Category:** data-analytics
**Tools Count:** 10

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


## Installation & Usage

To install and use the **ItemPath** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/itempath](https://vinkius.com/mcp/itempath)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
