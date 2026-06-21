# ItemPath MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/itempath)
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


## ❓ FAQ

**Q: How do I get ItemPath API credentials?**
Log in to your ItemPath instance, navigate to your user profile or security settings, and generate a new Application Token or Access Token.

**Q: What is the subdomain?**
The subdomain is the first part of your ItemPath URL (e.g., if you access ItemPath at acme.itempath.com, your subdomain is 'acme').

**Q: Can I see real-time inventory levels?**
Yes, the list_materials and list_batches tools provide real-time information on your current stock and material availability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/itempath](https://vinkius.com/mcp/itempath)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ItemPath** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `itempath` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ItemPath** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "itempath": {
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
