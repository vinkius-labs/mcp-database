# MRPeasy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mrpeasy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage manufacturing and inventory via MRPeasy — track customer orders, MOs, and stock items directly from your AI agent.

## Description
Connect your **MRPeasy** manufacturing and ERP account to your AI agent and streamline your production and inventory management through natural conversation.

### What you can do

- **Order Tracking** — List and inspect all customer and sales orders to monitor fulfillment and statuses.
- **Production Oversight** — Access manufacturing orders (MOs) to track real-time progress on the shop floor.
- **Inventory Management** — View all stock items, check current levels, and retrieve detailed history for specific items.
- **Procurement Insights** — List purchase orders (POs) sent to your vendors and manage supplier relationships.
- **Financial Overview** — Retrieve lists of sales invoices related to your manufacturing operations.
- **Work Station Monitoring** — View all defined work stations in your production environment.
- **Vendor Lookup** — Access a list of all registered raw material and product suppliers.

### How it works

1. Subscribe to this server
2. Enter your MRPeasy API Key and API Secret (requires Unlimited plan)
3. Start managing your factory from Claude, Cursor, or any MCP client

### Who is this for?

- **Production Managers** — quickly check the status of a manufacturing order without searching the ERP.
- **Inventory Coordinators** — verify stock levels for critical raw materials directly from your chat.
- **Operations Teams** — automate the retrieval of order and vendor data for daily standups.


## Available Tools (10)
- **list_purchase_orders**: List purchase orders (POs)
- **get_manufacturing_order**: Get specific manufacturing order info
- **get_stock_item**: Get specific stock item details
- **list_customer_orders**: List MRPeasy customer orders
- **list_invoices**: List sales invoices
- **list_manufacturing_orders**: List manufacturing orders (MOs)
- **list_stock_items**: List inventory stock items
- **list_vendors**: List suppliers and vendors
- **list_work_stations**: List manufacturing work stations
- **get_customer_order**: Get specific customer order details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MRPeasy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active manufacturing orders."

**🤖 AI Agent:**
> I've fetched the active manufacturing orders. You have 8 MOs currently in progress, including 'MO-501' (Status: In Production) and 'MO-502' (Status: Scheduled). Shall I give you the item details for MO-501?

---

**👤 You:**
> "Check current stock levels for raw materials."

**🤖 AI Agent:**
> Retrieving inventory list... You have 45 items in stock. Notable materials include 'Aluminum Plate' (150 units), 'Steel Bolt' (2,000 units), and 'Plastic Housing' (15 units - Low Stock Alert). Would you like the vendor info for the plastic housing?

---

**👤 You:**
> "List our registered vendors."

**🤖 AI Agent:**
> I've retrieved your vendor list. You have 12 registered suppliers, including 'Global Metals Co.', 'Swift Fasteners', and 'Reliable Plastics'. Would you like the contact info for Swift Fasteners?


## ❓ FAQ

**Q: Is API access available on all MRPeasy plans?**
No. According to MRPeasy documentation, the API is exclusively available to clients on the 'Unlimited' pricing plan.

**Q: Can I see the Bill of Materials (BOM) for a production order?**
Yes! Use the `get_manufacturing_order` tool with a specific MO ID to see the detailed metadata including the bill of materials required for that order.

**Q: How do I find a specific item's stock history?**
Use the `get_stock_item` tool with the item ID to retrieve its complete metadata and stock levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mrpeasy](https://vinkius.com/mcp/mrpeasy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MRPeasy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mrpeasy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MRPeasy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mrpeasy": {
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
