# ShipStation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shipstation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate shipping and order management via ShipStation — manage carriers, create labels, and track orders directly from any AI agent.

## Description
Connect your **ShipStation** account to any AI agent and take full control of your e-commerce logistics and fulfillment workflows through natural conversation.

### What you can do

- **Order Management** — List, create, and fetch detailed information for orders across all your connected stores.
- **Carrier Logistics** — List connected carriers, check account balances, and retrieve supported packages and services.
- **Shipping Rates & Labels** — Get real-time shipping rates and generate labels for orders or manual shipments instantly.
- **Fulfillment Operations** — Mark orders as shipped, void labels, and manage order tags to keep your workflow organized.
- **Store & Warehouse Sync** — List and update store configurations and manage warehouse locations for accurate inventory tracking.

### How it works

1. Subscribe to this server
2. Enter your ShipStation API Key and API Secret
3. Start managing your shipping operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Operators** — quickly check order statuses and generate labels without switching between multiple browser tabs.
- **Logistics Managers** — compare shipping rates and manage carrier balances through simple natural language commands.
- **Support Teams** — instantly retrieve customer order history and shipping details to provide faster assistance.


## Available Tools
- **add_funds**: Add funds to a carrier account
- **add_tag_to_order**: Add a tag to an order
- **create_label_for_order**: Create a shipping label for an order
- **create_order**: Create or update an order
- **create_shipment_label**: Create a manual shipment label
- **get_carrier**: Get carrier details and balance
- **get_customer**: Get customer details
- **get_order**: Get a single order by ID
- **get_rates**: Get shipping rates
- **get_store**: Get store details
- **list_carriers**: List all connected carriers
- **list_customers**: List customers with filters
- **list_orders_by_tag**: List orders by status and tag
- **list_orders**: List orders with filters
- **list_packages**: List packages for a carrier
- **list_services**: List services for a carrier
- **list_shipments**: List shipments (generated labels)
- **list_stores**: List stores
- **list_tags**: List all account tags
- **list_warehouses**: List warehouses (Ship From Locations)
- **list_webhooks**: List webhooks
- **mark_as_shipped**: Mark an order as shipped
- **register_account**: Register a new ShipStation account
- **remove_tag_from_order**: Remove a tag from an order
- **subscribe_webhook**: Subscribe to a webhook
- **unsubscribe_webhook**: Unsubscribe from a webhook
- **update_store**: Update a store
- **void_label**: Void a shipping label


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ShipStation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all orders with status 'awaiting_shipment' from the last 24 hours."

**🤖 AI Agent:**
> I've found 12 orders awaiting shipment. Notable orders include #ORD-5521 from John Doe and #ORD-5522 from Jane Smith. Would you like to see the details for any of these?

---

**👤 You:**
> "Get the full details for order ID 123456789."

**🤖 AI Agent:**
> Retrieving order 123456789... This order is for 'Wireless Headphones', status is 'awaiting_shipment', and it's shipping to New York via UPS Ground. The total amount is $89.99.

---

**👤 You:**
> "List all connected carriers and their current balances."

**🤖 AI Agent:**
> You have 3 carriers connected: Stamps.com (Balance: $45.20), FedEx (Account-based), and UPS (Account-based). Would you like to add funds to your Stamps.com account?


## ❓ FAQ

**Q: Can I check shipping rates for a specific order before creating a label?**
Yes! Use the `get_rates` tool. Provide the carrier, service, and package details to receive real-time pricing for your shipment.

**Q: How do I list all orders that are currently awaiting shipment?**
You can use the `list_orders` tool and set the `order_status` parameter to 'awaiting_shipment'. This will return all orders ready for fulfillment.

**Q: Is it possible to add funds to my carrier account through the AI?**
Yes, the `add_funds` tool allows you to add a specific amount to a carrier account (like Stamps.com) using the payment method you have on file in ShipStation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shipstation](https://vinkius.com/mcp/shipstation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ShipStation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `shipstation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ShipStation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shipstation": {
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
