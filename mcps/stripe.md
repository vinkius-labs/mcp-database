# Stripe MCP Server

Manage payments, customers, subscriptions, invoices, and account balance via Stripe — all from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/stripe)

## Overview
**Category:** industry-titans
**Tools Count:** 13

## Description
Take full control of your payment operations with **Stripe**, the global payments platform trusted by millions of businesses. Your AI agent becomes your financial operations assistant — listing customers, checking payment statuses, reviewing subscriptions, pulling invoices, and monitoring your account balance.

### What you can do

- **Customer Management** — List, search, and create customers with names, emails, and metadata.
- **Payment Tracking** — Monitor payment intents with status, amounts, and currency across all transactions.
- **Subscription Overview** — Check active, past-due, and canceled subscriptions with billing intervals and plan details.
- **Invoice Monitoring** — Review open, paid, and overdue invoices with hosted payment links.
- **Account Balance** — Instantly check available and pending balances across all currencies.

### How it works

1. Subscribe to this server
2. Enter your Stripe Secret Key (from Dashboard → Developers → API keys)
3. Start querying your Stripe data from Claude, Cursor, or any MCP client

### Who is this for?

- **Finance Teams** — audit payments, reconcile subscriptions, and chase overdue invoices from a single conversation.
- **SaaS Founders** — monitor MRR, track customer churn, and review billing status without opening the Stripe dashboard.
- **Support Teams** — quickly look up customer payment status and share invoice links during support tickets.


## Available Tools
- **customers_list**: Optionally filter by email. Returns customer details including name, email, balance, and delinquency status.

List Stripe customers
- **refunds_list**: List Stripe refunds
- **customers_create**: Name and email are required. Returns the created customer with their Stripe ID.

Create a new Stripe customer
- **payments_list**: Optionally filter by customer ID. Amounts are in the smallest currency unit (e.g., 1000 = $10.00).

List Stripe payment intents
- **subscriptions_list**: Optionally filter by customer or status.

List Stripe subscriptions
- **invoices_list**: Optionally filter by customer or status (draft, open, paid, uncollectible, void).

List Stripe invoices
- **balance_get**: Shows available and pending amounts by currency. Amounts are in smallest currency unit (divide by 100 for dollars).

Get Stripe account balance
- **products_list**: Use to browse your product offerings.

List Stripe products
- **product_create**: Use before creating prices.

Create a new Stripe product
- **prices_list**: Filter by product to see all price tiers.

List Stripe prices
- **refund_create**: Specify amount in cents for partial refunds.

Create a refund for a payment
- **charges_list**: Filter by customer ID.

List Stripe charges
- **payouts_list**: List Stripe payouts


## Installation & Usage

To install and use the **Stripe** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stripe](https://vinkius.com/mcp/stripe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
