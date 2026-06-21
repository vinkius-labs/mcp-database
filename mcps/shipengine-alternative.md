# ShipEngine MCP Server

Automate shipping and logistics via ShipEngine — validate addresses, compare rates, and track packages directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/shipengine-alternative)

## Overview
**Category:** ecommerce
**Tools Count:** 13

## Description
Connect your **ShipEngine** account to any AI agent to streamline your entire shipping workflow through natural conversation.

### What you can do

- **Address Validation** — Verify domestic and international addresses to prevent delivery failures and surcharges.
- **Rate Comparison** — Get real-time shipping rates across multiple carriers to find the best price for every shipment.
- **Label Creation** — Generate and purchase shipping labels instantly, using rate-shopping strategies (cheapest, fastest, best value).
- **Package Tracking** — Monitor shipments in real-time using tracking numbers or ShipEngine label IDs.
- **Carrier Management** — List connected carriers, connect new accounts, and manage balances for seamless operations.
- **Manifesting** — Create manifests and SCAN forms for carrier pickups directly from your agent.

### How it works

1. Subscribe to this server
2. Enter your ShipEngine API Key
3. Start managing logistics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — quickly compare shipping costs and generate labels without manual data entry or switching tabs.
- **Logistics Teams** — track multiple packages and validate customer addresses directly from the chat interface.
- **Developers** — test shipping workflows and carrier integrations using natural language instead of manual API calls.


## Available Tools
- **add_funds**: Add funds to a carrier balance
- **connect_carrier**: Connect a carrier account
- **create_label_rate_shopper**: Create a label using the rate shopper
- **create_label**: Create a shipping label
- **create_manifest**: Create a manifest (e.g., USPS SCAN form)
- **create_shipment**: Requires carrier_id, service_code, ship_to, and ship_from.

Create a new shipment
- **get_rates**: Calculate shipping rates
- **list_carriers**: List connected carriers
- **list_labels**: List shipping labels
- **track_label**: Track a package by label ID
- **track_package**: Track a package by carrier code and tracking number
- **validate_addresses**: Max 250 addresses.

Validate shipping addresses
- **void_label**: Void a shipping label


## Installation & Usage

To install and use the **ShipEngine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shipengine-alternative](https://vinkius.com/mcp/shipengine-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
