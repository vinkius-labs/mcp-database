# Klarna MCP Server

Manage payment sessions, orders, and fulfillment via the Klarna REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/klarna)

## Overview
**Category:** money-moves
**Tools Count:** 8

## Description
Connect your **Klarna** merchant account to any AI agent to automate your e-commerce payment and order management workflows. This MCP server enables your agent to interact with both the Klarna Payments API (checkout phase) and the Order Management API (post-purchase phase) directly from natural language.

### What you can do

- **Session Control** — Create and manage checkout sessions to obtain client tokens for your frontend
- **Order Placement** — Formally place orders using authorization tokens from your checkout widget
- **Payment Ingestion** — Capture authorized orders to trigger the actual payment from the customer
- **Financial Resolution** — Process full or partial refunds and cancel authorized but uncaptured orders
- **Logistics Integration** — Update shipping information and tracking numbers for existing orders
- **Data Oversight** — Retrieve detailed status, financial totals, and metadata for any Klarna order

### How it works

1. Subscribe to this server
2. Enter your Klarna API Key (Username), Shared Secret, and Region Domain
3. Start managing your payments and orders from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Operations** — Monitor order statuses and process captures/refunds via simple natural language commands
- **Financial Controllers** — Quickly audit payment sessions and transaction totals without logging into the portal
- **Developers** — Integrate Klarna's complex two-phase payment logic and status monitoring into your custom applications


## Available Tools
- **cancel_authorized_order**: Cancel an authorized but uncaptured order
- **capture_klarna_order**: Capture a formal order to trigger payment
- **create_payment_session**: Requires order amount, currency, and order lines (items).

Create a new Klarna payment session
- **get_order_details**: Get details for a specific Klarna order
- **get_payment_session**: Get details for an existing payment session
- **create_klarna_order**: Requires an authorization token.

Place a formal order using an authorization token
- **refund_klarna_order**: Refund a captured order
- **update_order_shipping**: Update shipping information for an order


## Installation & Usage

To install and use the **Klarna** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/klarna](https://vinkius.com/mcp/klarna)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
