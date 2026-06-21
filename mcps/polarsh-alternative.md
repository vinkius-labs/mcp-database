# Polar.sh MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/polarsh-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Monetize your open-source projects. Manage products, orders, subscriptions, and invoices directly through your AI agent.

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


## Available Tools (36)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Polar.sh** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active products on Polar."

**🤖 AI Agent:**
> I've retrieved your products. You have 3 active items: 'Developer Pro' (ID: prod_1), 'Sponsorship' (ID: prod_2), and 'API Access' (ID: prod_3). Would you like to see the details for any of these?

---

**👤 You:**
> "Get the details for order ID 'ord_123' and generate an invoice."

**🤖 AI Agent:**
> Order 'ord_123' was placed by user@example.com for $50.00. I have successfully triggered the `generate_invoice` action for this order. You can now retrieve the invoice data using `get_invoice`.

---

**👤 You:**
> "Revoke subscription 'sub_999' immediately."

**🤖 AI Agent:**
> I have successfully revoked subscription 'sub_999'. The customer's access to the associated product benefits has been terminated.


## ❓ FAQ

**Q: Can I cancel a user's subscription through the AI?**
Yes, you can use the `revoke_subscription` tool by providing the specific Subscription ID to terminate access immediately.

**Q: How do I generate an invoice for a specific order?**
Simply use the `generate_invoice` tool with the Order ID. The agent will trigger the invoice generation process on Polar.sh.

**Q: Is it possible to update the benefits of an existing product?**
Yes, the `update_product_benefits` tool allows you to modify the array of benefit IDs associated with any of your products.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/polarsh-alternative](https://vinkius.com/mcp/polarsh-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Polar.sh** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `polarsh-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Polar.sh** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "polarsh-alternative": {
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
