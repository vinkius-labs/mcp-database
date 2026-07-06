# Xsolla MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/xsolla)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming-entertainment](../categories/gaming-entertainment.md)

Manage game commerce via Xsolla — handle payments, search transactions, and manage virtual item catalogs directly from any AI agent.

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


## Available Tools (30)
- **create_order**: Requires User JWT.

Create an order for an item
- **get_bundles**: Get bundles
- **get_events**: Get events
- **get_payment_accounts**: Get user payment accounts
- **get_promotions_admin**: Get promotions (Admin)
- **invalidate_token**: Invalidate a Pay Station token
- **register_user_oauth**: 0 protocol.

Register a new user (OAuth 2.0)
- **register_user**: Register a new user
- **search_transactions**: Search transactions
- **update_subscription_plan**: Update a subscription plan
- **update_virtual_item_admin**: Update a virtual item (Admin)
- **verify_promo_code**: Requires User JWT.

Verify a promo code
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
- **get_virtual_items**: Get virtual items
- **create_payment**: Create a payment using a saved account
- **create_subscription_plan**: Create a subscription plan
- **create_token**: Create a Pay Station token
- **create_virtual_item_admin**: Create a virtual item (Admin)
- **link_account**: Requires User JWT.

Link user account
- **login_user**: Login user
- **mark_event_processed**: Mark event as processed
- **redeem_coupon**: Requires User JWT.

Redeem a coupon
- **refund_transaction**: Refund a transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Xsolla** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all completed transactions from the last 24 hours."

**🤖 AI Agent:**
> I've searched your transactions. I found 12 completed transactions in the last 24 hours, totaling $450.00. Would you like to see the details for the most recent ones?

---

**👤 You:**
> "List all virtual items and bundles in our store catalog."

**🤖 AI Agent:**
> Fetching catalog... I found 25 virtual items (including 'Gold Pouch' and 'Epic Sword') and 3 active bundles ('Starter Pack', 'Warrior Set'). Which one should I inspect further?

---

**👤 You:**
> "Get the full details for transaction ID 987654321."

**🤖 AI Agent:**
> Retrieving details for transaction 987654321... This was a payment of $19.99 for 'Season Pass' by user 'Gamer123'. Status: Completed. Payment method: Credit Card.


## ❓ FAQ

**Q: Can I search for specific transactions based on their status?**
Yes. Use the `search_transactions` tool. You can filter by status (e.g., 'completed', 'canceled') and date ranges to find exactly what you need.

**Q: How do I view the virtual items currently available in my catalog?**
Simply use the `get_virtual_items` tool. It will retrieve the full list of virtual items configured in your project catalog.

**Q: Is it possible to issue a refund through the AI agent?**
Yes. By using the `refund_transaction` tool with a valid Transaction ID and an optional reason, the agent can initiate the refund process directly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/xsolla](https://vinkius.com/mcp/xsolla)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Xsolla** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `xsolla` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Xsolla** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "xsolla": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
