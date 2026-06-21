# ManoMano (Home Improvement Marketplace) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/manomano-home-improvement-marketplace)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Manage your ManoMano seller account — update offer prices, track orders, and audit fulfillment stock.

## Description
Connect your **ManoMano Seller** account to any AI agent and take full control of your marketplace operations and home improvement catalog through natural conversation.

### What you can do

- **Offer Orchestration** — List all published offers and retrieve detailed metadata including current stock, VAT-included pricing, and SKUs directly from your agent
- **Live Catalog Updates** — Safely modify VAT-included prices and update available inventory quantities for specific offers to maintain competitive market positioning
- **Order Management** — List all received orders and retrieve complete representations including customer details, delivery addresses, and individual line items securely
- **Logistical Control** — Acknowledge and accept pending orders or transition them to 'Shipped' status by supplying carrier-specific tracking numbers and carrier names
- **Fulfillment Visibility** — Monitor stock levels maintained through ManoFulfillment (ManoMano warehouse) to ensure logistical accuracy and product availability
- **Taxonomy Discovery** — Enumerate root category lists and registered brands to guide product mapping and architectural catalog taxonomy natively

### How it works

1. Subscribe to this server
2. Enter your ManoMano API Key
3. Start managing your marketplace presence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketplace Sellers** — manage pricing and stock levels through natural conversation without manual Seller Central exports
- **E-commerce Managers** — monitor order flow and retrieve customer delivery data directly from your workspace for rapid auditing
- **Logistics Teams** — update shipping statuses and audit ManoFulfillment stock levels efficiently to maintain high fulfillment standards


## Available Tools (11)
- **list_offers**: List all published offers on ManoMano
- **get_offer**: Get details for a specific ManoMano offer (price, stock, SKU)
- **update_offer_price**: This is a reversible operation.

Change the price of a specific offer
- **update_offer_stock**: This is a reversible operation.

Update the available stock count for a specific offer
- **list_orders**: List all received ManoMano orders
- **get_order**: Get full order details including customer, addresses, and order lines
- **accept_order**: Accept a pending ManoMano order
- **ship_order**: Ship an order by supplying a valid tracking number and carrier
- **list_categories**: List ManoMano catalog categories
- **list_brands**: List available brands on ManoMano
- **list_fulfillment_stock**: Check stock maintained through ManoFulfillment (ManoMano warehouse)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ManoMano (Home Improvement Marketplace)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all ManoMano orders received today"

**🤖 AI Agent:**
> I've retrieved 5 new orders. Highlights include Order #MM-123 (Amount: €45.00, Status: Pending) and Order #MM-456 (Amount: €120.00, Status: Accepted). Would you like to see the delivery address for the pending order?

---

**👤 You:**
> "Update the stock for offer 'offer-987' to 50 units"

**🤖 AI Agent:**
> Updating inventory… I've successfully set the stock for offer 'offer-987' to 50 units. Your listing on ManoMano is now synchronized with this new quantity. Would you like me to check the current price as well?

---

**👤 You:**
> "Show me the stock levels in ManoFulfillment"

**🤖 AI Agent:**
> Retrieving fulfillment stock… I've identified several items in the ManoMano managed warehouse. You have 150 units of SKU 'DRILL-01' and 45 units of SKU 'SAW-05'. No low-stock alerts detected for today.


## ❓ FAQ

**Q: Can I update my product prices on ManoMano through my agent?**
Yes. Use the `update_offer_price` tool with a specific Offer ID. Your agent will safely modify the VAT-included price in EUR, allowing you to react to market changes instantly through conversation.

**Q: How do I mark a ManoMano order as shipped?**
The `ship_order` tool allows your agent to transition an accepted order into 'Shipped' status. You must provide the tracking number and the carrier name (e.g., DHL, UPS) to update the logistical state correctly.

**Q: Can my agent check the stock levels in ManoMano's own warehouse?**
Absolutely. Use the `list_fulfillment_stock` tool to retrieve the physical quantities maintained via ManoFulfillment. Your agent will report the current inventory levels available in the ManoMano managed warehouse.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/manomano-home-improvement-marketplace](https://vinkius.com/mcp/manomano-home-improvement-marketplace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ManoMano (Home Improvement Marketplace)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `manomano-home-improvement-marketplace` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ManoMano (Home Improvement Marketplace)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "manomano-home-improvement-marketplace": {
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
