# Lemon Squeezy (Merchant of Record & Payments) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lemon-squeezy-merchant-of-record-payments)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your Lemon Squeezy store, products, and customers directly through AI — handle payments and subscriptions via natural conversation.

## Description
Connect your **Lemon Squeezy** account to any AI agent to manage your Merchant of Record and payment workflows through natural conversation.

### What you can do

- **Store Management** — Retrieve details and list all your active stores to monitor your business hubs
- **Customer Operations** — Create, update, and list customers with ease, including filtering by email or store
- **Product Catalog** — Fetch specific product details and list your entire inventory directly from the cloud
- **User Insights** — Access your authenticated user profile information and account status

### How it works

1. Subscribe to this server
2. Enter your Lemon Squeezy API Key
3. Start managing your SaaS business from Claude, Cursor, or any MCP-compatible client

No more switching between tabs to find a customer's ID or check a product's status. Your AI acts as a dedicated billing assistant and store manager.

### Who is this for?

- **SaaS Founders** — quickly check product details or customer lists without leaving your development or management workflow
- **Support Teams** — find and update customer information instantly to resolve billing queries faster
- **Operations Leads** — automate store reporting and inventory checks through simple AI queries


## Available Tools
- **activate_license**: Activate a license key
- **cancel_subscription**: Cancel a subscription
- **create_checkout**: Create a checkout
- **create_customer**: Create a new customer
- **create_discount**: Create a discount
- **create_usage_record**: Create a usage record
- **create_webhook**: Create a webhook
- **deactivate_license**: Deactivate a license key
- **delete_discount**: Delete a discount
- **delete_webhook**: Delete a webhook
- **generate_order_invoice**: Generate an invoice for an order
- **generate_subscription_invoice**: Generate a subscription invoice
- **get_affiliate**: Retrieve a specific affiliate
- **get_checkout**: Retrieve a specific checkout
- **get_customer**: Retrieve a specific customer
- **get_discount_redemption**: Retrieve a specific discount redemption
- **get_discount**: Retrieve a specific discount
- **get_file**: Retrieve a specific file
- **get_license_key_instance**: Retrieve a specific license key instance
- **get_license_key**: Retrieve a specific license key
- **get_me**: Retrieve the currently authenticated user
- **get_order_item**: Retrieve a specific order item
- **get_order**: Retrieve a specific order
- **get_price**: Retrieve a specific price
- **get_product**: Retrieve a specific product
- **get_store**: Retrieve a specific store
- **get_subscription_invoice**: Retrieve a specific subscription invoice
- **get_subscription_item_current_usage**: Retrieve current usage for a subscription item
- **get_subscription_item**: Retrieve a specific subscription item
- **get_subscription**: Retrieve a specific subscription
- **get_usage_record**: Retrieve a specific usage record
- **get_variant**: Retrieve a specific variant
- **get_webhook**: Retrieve a specific webhook
- **list_affiliates**: List all affiliates
- **list_checkouts**: List all checkouts
- **list_customers**: List all customers
- **list_discount_redemptions**: List all discount redemptions
- **list_discounts**: List all discounts
- **list_files**: List all files
- **list_license_key_instances**: List all license key instances
- **list_license_keys**: List all license keys
- **list_order_items**: List all order items
- **list_orders**: List all orders
- **list_prices**: List all prices
- **list_products**: List all products
- **list_stores**: List all stores
- **list_subscription_invoices**: List all subscription invoices
- **list_subscription_items**: List all subscription items
- **list_subscriptions**: List all subscriptions
- **list_usage_records**: List all usage records
- **list_variants**: List all variants
- **list_webhooks**: List all webhooks
- **refund_order**: Issue a refund for an order
- **refund_subscription_invoice**: Issue a refund for a subscription invoice
- **update_customer**: Update a customer
- **update_license_key**: Update a license key
- **update_subscription_item**: Update a subscription item
- **update_subscription**: Update a subscription
- **update_webhook**: Update a webhook
- **validate_license**: Validate a license key


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lemon Squeezy (Merchant of Record & Payments)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Lemon Squeezy stores."

**🤖 AI Agent:**
> I've retrieved your stores. You have one active store: 'My Digital Shop' (ID: 45678). Would you like to see the products or customers for this store?

---

**👤 You:**
> "Create a new customer named Alice Smith with email alice@example.com for store 45678."

**🤖 AI Agent:**
> Processing... Alice Smith has been successfully created as a customer in store 45678 with ID 987654.

---

**👤 You:**
> "Get the details for product ID 12345."

**🤖 AI Agent:**
> Fetching product data... Product 'SaaS Pro Plan' (ID: 12345) is active. It is priced at $49.00 and currently has 152 active subscribers.


## ❓ FAQ

**Q: Can I check my own account details and authentication status?**
Yes! Use the `get_me` tool to retrieve information about the currently authenticated Lemon Squeezy user profile.

**Q: How do I find a specific customer by their email address?**
You can use the `list_customers` tool and provide the `filter_email` parameter. The agent will return matching customer records from your store.

**Q: Is it possible to update a customer's information like their name or location?**
Yes. The `update_customer` tool allows you to modify attributes such as name, email, city, region, and country for an existing customer ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lemon-squeezy-merchant-of-record-payments](https://vinkius.com/mcp/lemon-squeezy-merchant-of-record-payments)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lemon Squeezy (Merchant of Record & Payments)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `lemon-squeezy-merchant-of-record-payments` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lemon Squeezy (Merchant of Record & Payments)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lemon-squeezy-merchant-of-record-payments": {
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
