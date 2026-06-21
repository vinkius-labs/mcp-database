# Polar MCP Server

Manage digital products, subscriptions, orders and customers via Polar — create checkouts, manage discounts and track revenue from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/polar)

## Overview
**Category:** ecommerce
**Tools Count:** 10

## Description
Connect your **Polar** account to any AI agent and take full control of your digital commerce operations through natural conversation.

### What you can do

- **Product Management** — List, retrieve and audit all products (one-time, subscription, free) with pricing and metadata
- **Subscription Tracking** — Monitor active, canceled and past_due subscriptions with billing periods and customer info
- **Order & Revenue** — List completed orders with amounts, currency, payment status and customer details
- **Customer Discovery** — Browse customers by email, name and purchase history
- **Discount Management** — List, create and audit discount codes with percentage or fixed-amount types
- **Checkout Operations** — Create checkout sessions for products and track open, expired and confirmed checkouts
- **Webhook Audit** — Review configured webhook endpoints and their subscribed events

### How it works

1. Subscribe to this server
2. Enter your Polar Personal Access Token
3. Start managing your commerce from Claude, Cursor, or any MCP-compatible client

No more clicking through the Polar dashboard to check subscriptions or create discount codes. Your AI acts as a dedicated commerce engineer.

### Who is this for?

- **Indie Developers** — quickly check subscription status, review orders and create discount codes without leaving your IDE
- **Commerce Teams** — audit product catalog, track revenue via orders and manage customer data
- **Marketing** — create promotional discounts, track checkout conversion and review webhook integrations


## Available Tools
- **create_checkout**: Requires the product ID. Optionally associate with an existing customer and apply a discount. Returns the checkout session with its URL that you can redirect customers to for payment.

Create a new checkout session in Polar
- **create_discount**: Requires the name, code, type (percentage or fixed_amount), and amount. Optionally set the duration (once, forever, repeating). The discount can be applied during checkout.

Create a new discount code in Polar
- **get_product**: Provide the product ID (UUID format).

Get details for a specific Polar product
- **list_checkouts**: Each checkout shows its status (open, expired, confirmed), associated product, customer, and creation date. Useful for tracking abandoned and completed checkouts.

List checkout sessions in your Polar store
- **list_customers**: Each customer shows their email, name, billing address, and metadata. Optionally filter by email to find a specific customer.

List customers in your Polar store
- **list_discounts**: Each discount shows its code, type (percentage, fixed_amount), amount, duration (once, forever, repeating), and active status. Use this to audit your promotional offers.

List discount codes in your Polar store
- **list_orders**: Each order shows the customer, product, amount, currency, payment status, and creation date. Useful for tracking revenue and verifying successful transactions.

List orders in your Polar store
- **list_products**: Each product includes its name, description, price, type (one-time, subscription, free), and metadata. Use this to audit your product catalog and see what you are selling.

List products in your Polar store
- **list_subscriptions**: Each subscription shows the customer, product, status (active, past_due, canceled, expired, incomplete, trialing), current period start/end dates, and amount. Optionally filter by status and set a limit.

List subscriptions in your Polar store
- **list_webhooks**: Each webhook shows its URL, subscribed events (order.created, subscription.active, etc.), and status. Use this to audit your event integrations.

List webhook endpoints in your Polar store


## Installation & Usage

To install and use the **Polar** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/polar](https://vinkius.com/mcp/polar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
