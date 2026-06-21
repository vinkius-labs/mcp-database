# Boloo (Bol.com Retailer) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/boloo-bolcom-retailer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your bol.com store via the Retailer API — track orders, update stock, and manage offers directly from any AI agent.

## Description
Connect your **bol.com Retailer** account to any AI agent and orchestrate your e-commerce operations through natural conversation.

### What you can do

- **Order Oversight** — List open and handled orders, and retrieve detailed metadata for individual order items.
- **Inventory Management** — Update stock levels and prices for your offers in real-time to maintain accuracy.
- **Offer Coordination** — List and inspect all active product offers in your Boloo catalog.
- **Logistics Control** — Confirm shipments for order items and manage cancellations with valid reason codes.
- **Product Intelligence** — Retrieve global product details using EAN codes from the bol.com public catalog.
- **Integration Monitoring** — List configured webhook subscriptions to verify your event-driven data flow.

### How it works

1. Subscribe to this server
2. Enter your bol.com Client ID and Client Secret
3. Start managing your Dutch e-commerce business from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Retailers & Sellers** — quickly check for new orders and update inventory without logging into the seller dashboard.
- **Operations Managers** — monitor shipment statuses and offer performance straight from their workflow tools.
- **Developers** — verify API interactions and stock syncs using natural language.


## Available Tools (10)
- **cancel_order_item**: Requires a valid reason code.

Cancel an order item
- **get_offer**: Get details of a specific offer
- **get_order**: Get details of a specific order
- **get_product_details**: com catalog.

Get global product info by EAN
- **list_offers**: List all product offers
- **list_orders**: Default is OPEN.

List all open or handled orders
- **list_subscriptions**: List event subscriptions (webhooks)
- **ship_order_item**: Confirm shipment of an order item
- **update_offer_price**: Update the price for an offer
- **update_offer_stock**: Update the stock level for an offer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Boloo (Bol.com Retailer)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my open orders on bol.com."

**🤖 AI Agent:**
> I've retrieved your open orders. You have 3 pending orders, including Order #123456789 from John Doe. Would you like to see the items in these orders?

---

**👤 You:**
> "Update stock for offer 99283-abc to 50 units."

**🤖 AI Agent:**
> Stock for offer 99283-abc successfully updated to 50. The change is now live on bol.com.

---

**👤 You:**
> "Find product details for EAN 8712345678901."

**🤖 AI Agent:**
> I've retrieved the product info for EAN 8712345678901. It is a 'Wireless Gaming Mouse' in the Electronics category. Current lowest offer is €45.00.


## ❓ FAQ

**Q: Can I check for new open orders using the agent?**
Yes! Use the `list_orders` tool with the status 'OPEN'. Your agent will fetch all orders that are currently awaiting handling in your bol.com account.

**Q: How do I update the stock level for an existing product offer?**
Simply ask the agent to `update_offer_stock` and provide the Offer ID and the new amount. It will update the availability on the bol.com platform instantly.

**Q: Does the integration allow shipping items through bol.com Logistics?**
Yes. Use the `ship_order_item` tool to confirm that an item has been handed over to the carrier. You will need to provide a shipment reference and the carrier details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boloo-bolcom-retailer](https://vinkius.com/mcp/boloo-bolcom-retailer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Boloo (Bol.com Retailer)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `boloo-bolcom-retailer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Boloo (Bol.com Retailer)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "boloo-bolcom-retailer": {
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
