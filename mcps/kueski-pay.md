# Kueski Pay MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kueski-pay)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kueski-pay-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kueski-pay-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Integrate Kueski Pay to offer Buy Now, Pay Later (BNPL) at checkout. Manage BNPL orders, captures, refunds, and quincena simulations from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kueski Pay** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Simulate payment plans for a $3,500 MXN jacket on Kueski Pay."

**🤖 AI Agent:**
> For a $3,500 MXN purchase, Kueski Pay offers the following plans: 4 quincenas (0% interest) = $875 MXN / fortnight. 6 quincenas = $625 MXN / fortnight. 8 quincenas = $510 MXN / fortnight. (Standard Kueski fees apply to plans over 4 quincenas).

---

**👤 You:**
> "Capture order K-ABC-123. The items have been shipped."

**🤖 AI Agent:**
> Order K-ABC-123 has been successfully captured. The full amount of $2,100 MXN is now in the settlement queue. The customer's first quincena payment will be due in 15 days.

---

**👤 You:**
> "Check eligibility for phone 55-1234-5678 for a $5,000 cart."

**🤖 AI Agent:**
> Phone 55-1234-5678 is PRE-APPROVED for a BNPL loan of $5,000 MXN. They have an active Kueski Pay account with good standing. Would you like to generate a checkout session for them?


## Installation & Usage

To install and use the **Kueski Pay** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kueski-pay](https://vinkius.com/mcp/kueski-pay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
