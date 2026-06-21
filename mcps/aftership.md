# AfterShip MCP Server

Track packages worldwide — create, manage, and monitor shipments via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/aftership)

## Overview
**Category:** ecommerce
**Tools Count:** 9

## Description
Connect **AfterShip** tracking platform to any AI agent and track packages from 1,000+ couriers worldwide, auto-detect shipping companies, and manage all your shipments through natural language.

### What you can do

- **Package Tracking** — Create and monitor shipments from FedEx, UPS, DHL, USPS, and 1,000+ other couriers
- **Auto-Detect Courier** — Automatically identify the shipping company from just a tracking number
- **Tracking History** — View complete delivery history with checkpoint timestamps and locations
- **Delivery Management** — Mark trackings as completed, retrack expired ones, or delete old entries
- **Customer Notifications** — Set up email and SMS notifications for delivery updates
- **Courier Directory** — Browse all supported courier companies with their contact info and requirements

### How it works

1. Subscribe to this server
2. Enter your AfterShip API Key
3. Start tracking packages from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **create_tracking**: Requires at least the tracking number. Optionally specify the courier slug, title, customer emails, SMS phone numbers, order ID, and custom fields.

Create a new package tracking
- **delete_tracking**: This action cannot be undone.

Delete a tracking entry
- **detect_courier**: Useful when the user provides a tracking number but doesn't know which courier it belongs to. Returns a ranked list of likely couriers.

Auto-detect courier from tracking number
- **get_tracking**: Get details of a specific tracking
- **list_couriers**: ) that can be used for tracking packages.

List all supported courier companies
- **list_trackings**: Supports extensive filtering by courier (slug), tag, keyword, origin, destination, date ranges, and delivery status.

List all package trackings
- **mark_tracking_completed**: Useful when the package has been delivered but the courier hasn't updated the final status.

Mark a tracking as completed
- **retrack_tracking**: This restarts monitoring and will fetch new checkpoint updates.

Retrack an expired tracking
- **update_tracking**: Does not affect the tracking number or courier.

Update an existing tracking


## Installation & Usage

To install and use the **AfterShip** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aftership](https://vinkius.com/mcp/aftership)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
