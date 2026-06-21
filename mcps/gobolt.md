# GoBolt MCP Server

Manage shipping rates, track parcel deliveries, and oversee logistics via AI agents with GoBolt.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gobolt)

## Overview
**Category:** ecommerce
**Tools Count:** 12

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


## Installation & Usage

To install and use the **GoBolt** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gobolt](https://vinkius.com/mcp/gobolt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
