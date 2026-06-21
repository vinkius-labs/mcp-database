# HelloAsso MCP Server

Automate association management via HelloAsso — manage payments, forms, and orders for French non-profits directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/helloasso)

## Overview
**Category:** event-management
**Tools Count:** 11

## Description
Connect your **HelloAsso** account to any AI agent and take full control of your French non-profit management workflows through natural conversation.

### What you can do

- **Organization Oversight** — List and inspect all organizations where you have administrative rights.
- **Campaign Management** — List all active and past forms (Donations, Memberships, Events, Shop).
- **Payment Monitoring** — Access your financial history, track donations, and retrieve detailed payment metadata.
- **Order Handling** — List and inspect orders to understand payer behavior and item distribution.
- **Checkout Intents** — Generate redirect links for payments directly from the chat interface.
- **Member & Subscription Tracking** — Manage your membership base and monitor recurring donation plans.

### How it works

1. Subscribe to this server
2. Enter your HelloAsso Client ID and Client Secret
3. Start managing your association from Claude, Cursor, or any MCP-compatible client

No more manual exporting of transaction CSVs. Your AI assistant acts as a dedicated Association Coordinator or Financial Manager.

### Who is this for?

- **Non-Profit Directors** — instantly retrieve donation totals and campaign progress without digging through the dashboard.
- **Community Managers** — check membership statuses and event registration counts in real-time.
- **Financial Officers** — automate the oversight of payments and subscriptions across multiple associations.


## Available Tools
- **create_checkout_intent**: Pass the amount in cents (EUR) and other required fields as a JSON string in "body_json". Returns a redirect URL for the payer.

Generate a checkout link to receive a payment
- **get_member_details**: Get details for a specific member ID
- **get_order_details**: Get details for a specific order ID
- **get_organization_details**: Get detailed information about a specific organization by its slug
- **get_payment_details**: Get details for a specific payment ID
- **list_forms**: Each form has a "formType" and "formSlug" used for detailed lookups.

List all campaigns/forms (Donations, Memberships, Events) for an organization
- **list_sold_items**: g., ticket, membership tier) that were part of orders.

List all individual items sold/distributed by an organization
- **list_my_organizations**: Use this to find the "slug" required for other tools.

List all organizations where the user has administrative rights
- **list_orders**: An order represents one or more items purchased or donated by a user in a single session.

List all orders (group of items/payments) for an organization
- **list_payments**: Returns amounts in cents (EUR). Use this to track donations or membership payments.

List all payments received by an organization
- **list_subscriptions**: List recurring payments (subscriptions) for an organization


## Installation & Usage

To install and use the **HelloAsso** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/helloasso](https://vinkius.com/mcp/helloasso)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
