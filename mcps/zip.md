# Zip MCP Server

Manage BNPL checkouts, orders, and payments via the Zip (Quadpay) REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zip)

## Overview
**Category:** money-moves
**Tools Count:** 8

## Description
Connect your **Zip** (formerly Quadpay) merchant account to any AI agent to automate your Buy Now, Pay Later (BNPL) workflows. This MCP server enables your agent to initiate checkouts, manage order authorizations, and process captures or refunds directly from natural language interfaces.

### What you can do

- **Checkout Initiation** — Create new checkout sessions and retrieve redirect URLs for customers
- **Order Management** — Authorize and confirm orders across US and Global gateway environments
- **Payment Ingestion** — Capture authorized funds once goods are shipped to finalize transactions
- **Financial Resolution** — Process full or partial refunds and void authorized but uncaptured payments
- **Status Monitoring** — Retrieve real-time status and lifecycle updates for any Zip order
- **Account Insight** — Access merchant configuration, currency limits, and account-level settings

### How it works

1. Subscribe to this server
2. Enter your Zip Merchant API Key, Region, and Environment (Sandbox/Production)
3. Start managing your BNPL payments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Operations** — Monitor order lifecycles and process captures/refunds via simple natural language commands
- **Financial Controllers** — Quickly audit transaction statuses and merchant configurations without opening the portal
- **Developers** — Integrate BNPL checkout logic and status monitoring into your custom applications


## Available Tools
- **authorize_zip_order**: Typically used in US gateway integrations.

Authorize a payment order
- **capture_zip_payment**: Capture funds for an authorized order
- **confirm_zip_order**: Finalize an authorized order
- **create_zip_checkout**: Requires amount, currency, and redirect URLs.

Initialize a new Zip checkout session
- **get_zip_merchant_config**: Retrieve merchant account configuration
- **get_zip_order_status**: g., Authorized, Captured, Cancelled) for a target order.

Check the status of a Zip order
- **refund_zip_payment**: Process a refund for an order
- **void_zip_payment**: Void an authorized but uncaptured payment


## Installation & Usage

To install and use the **Zip** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zip](https://vinkius.com/mcp/zip)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
