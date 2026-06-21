# GoBolt MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gobolt)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage shipping rates, track parcel deliveries, and oversee logistics via AI agents with GoBolt.

## Description
Connect your **GoBolt** merchant account to any AI agent to automate your e-commerce logistics and parcel tracking through the Model Context Protocol (MCP). GoBolt is a sustainable logistics and 3PL provider that simplifies global shipping. This MCP server enables you to retrieve real-time shipping rates, manage fulfillment orders, and track deliveries directly through natural conversation.

### Key Features

- **Real-time Quoting** — Retrieve live shipping rates based on origin, destination, and package dimensions to provide accurate costs to your customers.
- **Order Management** — Create and manage shipping orders in GoBolt's fulfillment system, including updating recipient and package details.
- **Precision Tracking** — Access real-time status updates and full event histories for any order ID or tracking number.
- **Label Generation** — Retrieve PDF or ZPL shipping labels for fulfilled orders programmatically from your chat interface.
- **Sustainability Insights** — Access metadata related to GoBolt's eco-friendly logistics and last-mile delivery services.
- **Merchant Oversight** — Access metadata for your authenticated account to verify connectivity and authorized project scopes.
- **Real-time Synchronization** — Keep your logistics and fulfillment data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GoBolt Client ID and Client Secret (found in the Merchant Portal)
3. Start managing your logistics from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Operations** — quickly check the status of a high-value parcel or retrieve a shipping label without manual portal navigation.
- **Logistics Managers** — get a real-time overview of shipping rates and delivery estimates via simple AI commands.
- **Customer Support** — automate the retrieval of tracking information and troubleshoot delivery issues seamlessly.


## Available Tools
- **verify_api_connection**: Check connection
- **create_shipping_order**: Place shipping order
- **get_merchant_info**: Get account identity
- **find_fastest_rate**: Find fastest delivery
- **get_shipping_labels**: Download labels
- **find_cheapest_rate**: Find lowest cost
- **get_order_details**: Get order metadata
- **get_shipping_rates**: Get real-time rates
- **get_tracking_history**: View full events
- **track_shipment**: Get tracking info
- **list_shipping_orders**: List all orders
- **modify_shipping_order**: Update order info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GoBolt** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get shipping rates from NY to LA for a 2kg package."

**🤖 AI Agent:**
> Retrieving rates... I found 3 options: Standard Ground ($12.50, 4 days), Express ($25.00, 2 days), and Overnight ($45.00). Would you like to create an order for any of these?

---

**👤 You:**
> "Track my order with ID 'GBLT-98765'."

**🤖 AI Agent:**
> Checking status... Order GBLT-98765 is currently 'In Transit'. It was scanned in Chicago this morning and is estimated to arrive on Thursday by 5 PM.

---

**👤 You:**
> "Find the cheapest shipping rate for a package to Toronto."

**🤖 AI Agent:**
> Calculating best rate... The cheapest option for Toronto is 'Postal Surface' at $8.75 CAD with an estimated delivery in 6 business days.


## ❓ FAQ

**Q: How do I get a Client ID and Secret for GoBolt?**
Log in to the GoBolt Merchant Portal, navigate to Settings > API, and create a new Service User to generate your Client ID and Secret.

**Q: What format should the addresses be in for rates?**
Addresses should be provided as JSON objects with 'street', 'city', 'state_province', 'postal_code', and 'country' fields.

**Q: Can I track a shipment without a GoBolt ID?**
Yes! The 'track_shipment' tool accepts either a GoBolt Order ID or a Carrier Tracking Number.

**Q: What label formats are supported?**
The API supports 'pdf' for standard printers and 'zpl' for industrial thermal label printers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gobolt](https://vinkius.com/mcp/gobolt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GoBolt** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gobolt` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GoBolt** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gobolt": {
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
