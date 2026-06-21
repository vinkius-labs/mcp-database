# Polar.sh MCP Server

Monetize your open-source projects. Manage products, orders, subscriptions, and invoices directly through your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/polarsh)

## Overview
**Category:** developer-tools
**Tools Count:** 36

## Description
Connect your **Polar.sh** account to any AI agent to manage your open-source monetization and SaaS billing directly through natural language.

### What you can do

- **Product Management** — List, create, and update products or digital goods. Manage benefits and recurring pricing models using `list_products` and `create_product`.
- **Order & Invoice Tracking** — Monitor sales, retrieve specific order details with `get_order`, and generate professional invoices using `generate_invoice`.
- **Subscription Lifecycle** — List active subscribers, create free subscriptions for community members, and revoke access when necessary with `revoke_subscription`.
- **Checkout Insights** — List and inspect checkout sessions to understand your conversion funnel via `list_checkouts`.

### How it works

1. Subscribe to this server
2. Enter your Polar Personal Access Token
3. Start managing your developer business from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Open Source Maintainers** — manage sponsorships and digital products without leaving your terminal or editor.
- **SaaS Founders** — quickly check MRR, list new orders, and handle subscription support via AI.
- **Developer Relations** — grant product benefits and free subscriptions to community contributors instantly.


## Available Tools
- **confirm_checkout_client**: Confirm a session from the client
- **create_benefit**: Create a benefit
- **create_checkout**: Create a checkout session
- **create_customer_session**: Generate a customer session token
- **create_customer**: Create a customer
- **create_product**: Create a product
- **create_subscription**: Create a subscription (free products only)
- **create_webhook_endpoint**: Create a webhook endpoint
- **delete_benefit**: Delete a benefit (revokes all associated grants)
- **generate_invoice**: Generate an invoice for an order
- **get_benefit**: Get benefit details
- **get_checkout**: Get session details
- **get_customer_state**: Get full overview of customer active subscriptions and benefits
- **get_invoice**: Retrieve generated invoice data
- **get_order**: Get order details
- **get_portal_me**: Get authenticated customer info
- **get_product**: Get product details
- **get_subscription**: Get subscription details
- **list_benefits**: List benefits
- **list_checkouts**: List checkout sessions
- **list_customers**: List customers
- **list_orders**: List orders
- **list_portal_benefit_grants**: List benefits granted to the customer
- **list_portal_license_keys**: List customer license keys
- **list_portal_orders**: List customer orders
- **list_portal_subscriptions**: List customer subscriptions
- **list_products**: Filter by organization_id, is_recurring, etc.

List products
- **list_subscriptions**: List subscriptions
- **list_webhook_deliveries**: List and monitor webhook deliveries
- **revoke_subscription**: Revoke/cancel a subscription immediately
- **update_checkout**: Update a session
- **update_order**: Update order (e.g., billing details)
- **update_product_benefits**: Update benefits granted by a product
- **update_product**: Update a product
- **update_subscription**: Update a subscription
- **validate_portal_license_key**: Validate a license key


## Installation & Usage

To install and use the **Polar.sh** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/polarsh](https://vinkius.com/mcp/polarsh)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
