# Moova MCP Server

Automate smart logistics via Moova — create shipments, track deliveries, get shipping quotes, and orchestrate carriers from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/moova)

## Overview
**Category:** ecommerce
**Tools Count:** 14

## Description
Connect your **Moova** B2B logistics account to any AI agent and orchestrate your entire delivery operation through natural conversation.

### What you can do

- **Shipment Management** — Create, update, and cancel delivery orders with full origin/destination address details and contact information
- **Real-time Tracking** — Follow every shipment through GPS-powered tracking events including carrier handoffs, delivery attempts, and proof of delivery
- **Smart Quoting** — Get instant shipping cost estimates between any two addresses using Moova's intelligent carrier routing engine
- **Label Generation** — Download printable shipping labels with barcodes and QR codes for any registered shipment
- **Coverage Intelligence** — Query available delivery zones across Argentina and Latin America before committing to an order
- **Webhook Automation** — Configure real-time notifications for shipment status changes to keep your systems synchronized

### How it works

1. Subscribe to this server
2. Enter your Moova App ID and App Key
3. Start managing logistics from Claude, Cursor, or any MCP-compatible client

Your AI becomes a dedicated logistics coordinator, eliminating manual order entry and constant dashboard monitoring.

### Who is this for?

- **E-commerce Operations** — automate shipment creation from order data and monitor delivery progress without a separate logistics dashboard
- **Logistics Managers** — track fleet-wide delivery status and generate cost estimates for sales teams in real-time
- **Customer Support** — instantly pull tracking information and shipment status to respond to delivery inquiries within seconds


## Available Tools
- **cancel_shipment**: Once cancelled, the shipment cannot be reactivated and a new one must be created if needed.

Cancel an active shipment order
- **create_shipment**: Requires origin and destination addresses with full street details, contact information, and package dimensions. Moova will automatically assign the optimal carrier and route based on real-time availability.

Create a new logistics shipment
- **create_webhook**: Essential for keeping your e-commerce platform synchronized with delivery progress.

Register a new webhook for shipment events
- **delete_webhook**: Remove a webhook endpoint
- **get_account_info**: Get merchant account information
- **get_budget**: Returns pricing from available carriers including express, same-day, and standard delivery options.

Get a shipping cost estimate
- **get_shipment_label**: The label includes barcode, QR code, and all routing information required by the assigned carrier.

Download the shipping label for a shipment
- **get_shipment_status**: Get the current status of a shipment
- **get_shipment**: Get full details of a specific shipment
- **list_coverage_zones**: List all available delivery coverage zones
- **list_shipments**: Can be filtered by shipment status (e.g., CREATED, IN_TRANSIT, DELIVERED, CANCELLED) to narrow results.

List all shipments with optional status filter
- **list_webhooks**: List all registered webhooks
- **track_shipment**: Get real-time tracking events for a shipment
- **update_shipment**: Changes are not allowed after the carrier has collected the package.

Update shipment details before pickup


## Installation & Usage

To install and use the **Moova** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moova](https://vinkius.com/mcp/moova)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
