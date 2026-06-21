# Xsolla MCP Server

Manage game commerce via Xsolla — handle payments, search transactions, and manage virtual item catalogs directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/xsolla)

## Overview
**Category:** gaming-entertainment
**Tools Count:** 30

## Description
Connect your **Xsolla** merchant account to any AI agent to streamline your gaming commerce and payment workflows through natural conversation.

### What you can do

- **Payment Processing** — Generate Pay Station tokens using `create_token` and manage saved payment accounts with `get_payment_accounts`.
- **Transaction Auditing** — Search through transaction history using `search_transactions` and retrieve granular data with `get_transaction_details`.
- **Catalog Management** — List all available `get_virtual_items` and `get_bundles` to monitor your store's offerings.
- **Refunds & Orders** — Process `refund_transaction` requests and create new orders via `create_order` seamlessly.
- **User Carts** — Inspect active user shopping sessions with `get_user_cart`.

### How it works

1. Subscribe to this server
2. Enter your Xsolla Merchant ID, Project ID, and API Key
3. Start managing your game economy from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Game Developers** — check item availability and transaction statuses without leaving the code editor.
- **Customer Support Leads** — quickly find transaction details and process refunds via chat to resolve player issues faster.
- **Product Managers** — monitor catalog performance and bundle listings in real-time through simple queries.


## Available Tools
- **get_promotions_admin**: Get promotions (Admin)
- **get_social_login_url**: Get social login URL
- **get_subscription_plans**: Get subscription plans
- **get_transaction_details**: Get transaction details
- **get_user_attributes**: Requires User JWT.

Get user attributes
- **get_user_cart**: Requires User JWT.

Get user cart
- **get_user_profile**: Requires User JWT.

Get user profile
- **activate_promotion**: Activate a promotion
- **get_user_subscription**: Get user subscription
- **create_order**: Requires User JWT.

Create an order for an item
- **get_virtual_items**: Get virtual items
- **invalidate_token**: Invalidate a Pay Station token
- **create_payment**: Create a payment using a saved account
- **create_subscription_plan**: Create a subscription plan
- **create_token**: Create a Pay Station token
- **create_virtual_item_admin**: Create a virtual item (Admin)
- **get_bundles**: Get bundles
- **get_events**: Get events
- **get_payment_accounts**: Get user payment accounts
- **link_account**: Requires User JWT.

Link user account
- **login_user**: Login user
- **mark_event_processed**: Mark event as processed
- **redeem_coupon**: Requires User JWT.

Redeem a coupon
- **refund_transaction**: Refund a transaction
- **register_user_oauth**: 0 protocol.

Register a new user (OAuth 2.0)
- **register_user**: Register a new user
- **search_transactions**: Search transactions
- **update_subscription_plan**: Update a subscription plan
- **update_virtual_item_admin**: Update a virtual item (Admin)
- **verify_promo_code**: Requires User JWT.

Verify a promo code


## Installation & Usage

To install and use the **Xsolla** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/xsolla](https://vinkius.com/mcp/xsolla)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
