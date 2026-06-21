# Stripe MCP Server

Manage payments, customers, products and subscriptions via Stripe — create payment intents, track invoices and audit refunds from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/stripe-alternative)

## Overview
**Category:** money-moves
**Tools Count:** 13

## Description
Connect your **Stripe** account to any AI agent and take full control of your payment infrastructure through natural conversation.

### What you can do

- **Customer Management** — List, retrieve and create customers with email, name and metadata
- **Product & Pricing** — Browse products and their prices (one-time and subscription) with currency and amount details
- **Payment Tracking** — Monitor payment intents with status (succeeded, pending, failed) and associated customers
- **Charge & Refund Audit** — Review all charges and refunds with amounts, statuses and timestamps
- **Subscription Oversight** — Track active subscriptions, their billing cycles and associated prices
- **Invoice Review** — List invoices with amounts due, status (draft, paid, open) and customer details
- **Balance Monitoring** — Check available and pending balances across currencies
- **Coupon Management** — List discount coupons with percent-off, amount-off and duration settings

### How it works

1. Subscribe to this server
2. Enter your Stripe Secret Key
3. Start managing your payments from Claude, Cursor, or any MCP-compatible client

No more switching to the Stripe dashboard to check a payment status or audit refunds. Your AI acts as a dedicated payments engineer.

### Who is this for?

- **Finance Teams** — quickly check balances, review invoices and audit refunds without opening the Stripe dashboard
- **Developers** — create payment intents, list customers and inspect product pricing without leaving your IDE
- **Product Managers** — monitor subscription statuses, track customer growth and review coupon usage via conversation


## Available Tools
- **create_customer**: Optionally set the email, name and description. Returns the created customer with its ID.

Create a new Stripe customer
- **create_payment_intent**: Requires the amount (in smallest currency unit, e.g. cents for USD) and currency (e.g. "usd"). Optionally associate with a customer. Returns the payment intent with its client_secret for use with Stripe.js.

Create a new payment intent in Stripe
- **get_balance**: Returns available and pending balances broken down by currency and type (card, bank_transfer, etc.). Useful for checking your Stripe payout status.

Get current Stripe account balance
- **get_customer**: Provide the customer ID (starts with "cus_").

Get details for a specific Stripe customer
- **list_charges**: Each charge has an ID, amount, currency, status (succeeded, pending, failed), customer, payment method and creation date. Optionally filter by customer and set a limit.

List charges in Stripe
- **list_coupons**: Each coupon has an ID, name, percent_off or amount_off, duration (once, repeating, forever) and active status. Optionally set a limit.

List coupons in Stripe
- **list_customers**: Each customer has an ID, email, name, description and metadata. Optionally filter by email to find a specific customer and set a limit on the number of results returned.

List customers in Stripe
- **list_invoices**: Each invoice has an ID, customer, amount due, status (draft, open, paid, uncollectible), creation date and line items. Optionally filter by customer and set a limit.

List invoices in Stripe
- **list_payment_intents**: Each intent has an ID, amount, currency, status (requires_payment_method, requires_confirmation, requires_action, processing, succeeded, canceled) and associated customer. Optionally filter by customer and set a limit.

List payment intents in Stripe
- **list_prices**: Each price has an ID, unit amount, currency, recurring interval (if subscription) and associated product. Optionally filter by product ID, active status and limit.

List prices in Stripe
- **list_products**: Each product has an ID, name, description, images and active status. Products are used with Prices to define what you sell. Optionally filter by active status and set a limit.

List products in Stripe
- **list_refunds**: Each refund has an ID, amount, charge ID, status (succeeded, pending, failed, canceled) and creation date. Optionally set a limit.

List refunds in Stripe
- **list_subscriptions**: Each subscription has an ID, customer, status (trialing, active, past_due, canceled, unpaid, incomplete), items (prices) and billing cycle details. Optionally filter by customer, status and set a limit.

List subscriptions in Stripe


## Installation & Usage

To install and use the **Stripe** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stripe-alternative](https://vinkius.com/mcp/stripe-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
