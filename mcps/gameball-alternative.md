# Gameball MCP Server

Automate loyalty programs and gamification via Gameball — manage customer profiles, track points, and handle order rewards directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gameball-alternative)

## Overview
**Category:** ecommerce
**Tools Count:** 8

## Description
Connect your **Gameball** account to any AI agent to orchestrate your loyalty and retention strategies through natural conversation.

### What you can do

- **Customer Management** — Create or update customer profiles with custom attributes and contact details instantly.
- **Points & Balances** — Retrieve real-time points balances, monetary values, and upcoming expiration dates for any customer.
- **Transaction Control** — Hold points for temporary redemption to prevent double-spending during checkout processes.
- **Order Tracking** — Submit order details to automatically award loyalty points and finalize held redemptions.
- **Refund Handling** — Process refunds or cancellations to reverse points earned or restore points redeemed accurately.

### How it works

1. Subscribe to this server
2. Enter your Gameball API Key (and optional Secret Key)
3. Start managing your loyalty ecosystem from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — quickly check customer loyalty tiers and reward status without leaving your workflow.
- **Growth & Marketing Teams** — automate customer profiling and event tracking to drive retention.
- **Support Teams** — handle point refunds and balance inquiries directly within the chat interface.


## Available Tools
- **create_or_update_customer**: This API is idempotent.

Create or update a Gameball customer profile
- **get_customer_activities**: Get a log of customer activities
- **get_customer_balance**: Get a customer's points balance
- **get_order_transactions**: Get all loyalty transactions for an order
- **hold_points**: Holds typically expire after 10 minutes.

Hold points for temporary redemption
- **refund_transaction**: Refund a transaction
- **send_events**: Send customer events
- **track_order**: Track an order to award points and finalize redemptions


## Installation & Usage

To install and use the **Gameball** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gameball-alternative](https://vinkius.com/mcp/gameball-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
