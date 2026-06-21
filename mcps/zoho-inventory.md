# Zoho Inventory MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-inventory)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage inventory items, sales orders, and stock levels via the Zoho Inventory API.

## Description
Connect your **Zoho Inventory** account to any AI agent to automate your order management and stock control. This MCP server enables your agent to interact with products, sales orders, and purchase orders directly through natural language interfaces.

### What you can do

- **Inventory Oversight** — List all items in your inventory and retrieve real-time stock levels and metadata
- **Order Management** — List, retrieve, and create sales orders and purchase orders across your organizations
- **Stock Tracking** — Monitor item availability and identify stockouts before they happen
- **Bundle Visibility** — List composite items and bundles to understand your product kits and assemblies
- **Multi-Org Support** — Manage multiple business entities by providing the required organization ID for all operations

### How it works

1. Subscribe to this server
2. Enter your Zoho Client ID, Client Secret, and Data Center Domain
3. Start managing your inventory from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Inventory Managers** — Quickly check item availability and update stock notes via natural language commands
- **Warehouse Operations** — Monitor incoming and outgoing orders without opening the administrative panel
- **Developers** — Integrate real-time inventory data and order automation into your daily development workflow


## Available Tools
- **list_composite_items**: List all composite items (bundles)
- **create_new_item**: Requires a JSON body with item details (name, rate, etc.).

Add a new item to the inventory
- **create_sales_order**: Requires a JSON body with customer and line item details.

Create a new sales order
- **get_item_details**: Get details for a specific item
- **get_sales_order_details**: Get details for a specific sales order
- **list_inventory_items**: List all items in the inventory
- **list_organizations**: Use this to identify the organization ID for other calls.

List all Zoho Inventory organizations
- **list_purchase_orders**: List all purchase orders
- **list_sales_orders**: List all sales orders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho Inventory** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all organizations in my Zoho Inventory account."

**🤖 AI Agent:**
> I've retrieved your organizations. You have 2 entities: 'Main Store (ID: 123456)' and 'Secondary Warehouse (ID: 789012)'. Which one would you like to access?

---

**👤 You:**
> "Show the stock level for 'Professional Camera'."

**🤖 AI Agent:**
> For 'Professional Camera' (ID: 101) in organization 123456, there are currently 45 units available in stock.

---

**👤 You:**
> "List my 5 most recent sales orders in organization '123456'."

**🤖 AI Agent:**
> I've fetched your latest sales orders. Recent transactions include Order #SO-001 for 'Alice Smith' ($1,500.00) and Order #SO-002 for 'Bob Jones' ($850.50).


## ❓ FAQ

**Q: How do I find my Organization ID?**
Use the `list_organizations` tool to retrieve all businesses registered in your account along with their unique IDs.

**Q: Which Data Center domains are supported?**
You can use Zoho domains such as `com` (US), `eu` (Europe), `in` (India), `com.au` (Australia), or `jp` (Japan).

**Q: Can I create a sales order directly via the agent?**
Yes, use the `create_sales_order` tool by providing the Organization ID and a JSON object containing the customer and line item details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-inventory](https://vinkius.com/mcp/zoho-inventory)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho Inventory** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zoho-inventory` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho Inventory** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-inventory": {
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
