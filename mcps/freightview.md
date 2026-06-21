# Freightview MCP Server

Automate LTL freight quoting, track shipments, and manage carriers via AI agents with Freightview.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/freightview)

## Overview
**Category:** logistics-supply-chain
**Tools Count:** 12

## Description
Connect your **Freightview** account to any AI agent to automate your LTL (Less-Than-Truckload) freight quoting and logistics management through the Model Context Protocol (MCP). Freightview is a centralized platform that connects shippers with all their carriers in one place. This MCP server enables you to request real-time rates, monitor active shipments, and oversee your logistics network directly through natural conversation.

### Key Features

- **Real-time Quoting** — Request freight rates from all your connected carriers simultaneously by providing origin and destination details.
- **Shipment Tracking** — List all active shipments and fetch detailed tracking metadata including current transit status and estimated delivery.
- **Carrier Oversight** — Access and list all carriers connected to your account to maintain full visibility of your logistics partners.
- **Logistics Directory** — Access your saved address book and item catalog to facilitate faster and more accurate quoting.
- **Webhook Integration** — Monitor active webhooks configured for real-time status updates and automated logistics notifications.
- **Account Metadata** — Fetch detailed account attributes and contact information to maintain full context of your shipping operations.
- **Audit & History** — Retrieve historical quotes and shipment details for better cost analysis and reporting.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Freightview User Key and Account Key (found in Account Settings > API Keys)
3. Start managing your LTL freight operations from Claude, Cursor, or any MCP client

### Who is this for?

- **Logistics Coordinators** — quickly compare rates or track multiple shipments while managing daily outbound freight.
- **Supply Chain Managers** — get a real-time overview of carrier performance and active shipment statuses via simple AI commands.
- **E-commerce Ops** — automate the retrieval of freight quotes and tracking information for customer support and order fulfillment.


## Available Tools
- **request_rates**: Request freight rates
- **get_account_details**: Get organization attributes
- **get_carrier_details**: Get carrier info
- **get_quote_details**: Get quote metadata
- **get_shipment_details**: Get shipment metadata
- **list_address_book**: List saved addresses
- **list_connected_carriers**: List connected carriers
- **list_contacts**: List logistics contacts
- **list_item_catalog**: List commonly shipped items
- **list_freight_quotes**: List recent quotes
- **list_shipments**: List freight shipments
- **list_webhooks**: List active webhooks


## Installation & Usage

To install and use the **Freightview** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freightview](https://vinkius.com/mcp/freightview)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
