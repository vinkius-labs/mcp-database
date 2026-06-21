# Kueski Pay MCP Server

Integrate Kueski Pay to offer Buy Now, Pay Later (BNPL) at checkout. Manage BNPL orders, captures, refunds, and quincena simulations from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kueski-pay)

## Overview
**Category:** money-moves
**Tools Count:** 14

## Description
Connect your **Kueski Pay** merchant account to any AI agent and manage Mexico's leading Buy Now, Pay Later (BNPL) platform programmatically.

### What you can do

- **Checkout Automation** — Create new BNPL checkout sessions and simulate "pay in quincenas" installment plans for any purchase amount
- **Order Lifecycle** — Track orders from pending to approved, capture funds upon fulfillment, and process full or partial refunds
- **Settlement Tracking** — Reconcile merchant payouts by querying daily settlement batches and fees
- **Webhook Management** — Subscribe to real-time event notifications for order approvals and declines
- **Eligibility Checks** — Programmatically check if a customer's phone number is pre-approved for a specific loan amount

### How it works

1. Subscribe to this server
2. Enter your Kueski Pay API credentials
3. Start managing your BNPL offering from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — manage captures and refunds without logging into the Kueski dashboard
- **Customer Support** — instantly check a customer's BNPL order status or remaining credit limits
- **Developers** — simulate installment pricing dynamically for product pages


## Available Tools
- **cancel_order**: This releases the credit hold on the customer's Kueski account.

Cancel a pending or authorized order
- **capture_order**: This should be called when you fulfill or ship the items. Can capture the full or partial amount.

Capture an authorized order
- **check_eligibility**: Check BNPL eligibility for a phone number
- **create_order**: Returns a checkout URL where the customer can complete their credit application to pay in quincenas (fortnightly installments).

Create a new Kueski Pay BNPL order
- **create_webhook**: approved, order.declined, refund.completed.

Create a webhook subscription
- **get_customer_limits**: Check customer credit limits
- **get_merchant_profile**: View Merchant profile settings
- **get_order**: g., pending, approved, declined, captured). Used to check if the customer successfully completed the Kueski Pay checkout process.

Get details of a specific BNPL order
- **get_settlement**: Get details of a specific settlement payout
- **list_orders**: Can filter by status.

List recent Kueski Pay orders
- **list_settlements**: List merchant payout settlements
- **list_webhooks**: List active webhook subscriptions
- **refund_order**: Kueski will adjust the customer's remaining quincena payment schedule accordingly.

Refund a captured order
- **simulate_installments**: g., 4, 6, 8 quincenas), interest rates, and estimated fortnight payment amounts for a specific purchase price. Useful for displaying pricing info on product pages.

Simulate quincena payment terms for an amount


## Installation & Usage

To install and use the **Kueski Pay** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kueski-pay](https://vinkius.com/mcp/kueski-pay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
