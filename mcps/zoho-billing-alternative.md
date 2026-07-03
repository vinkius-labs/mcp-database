# Zoho Billing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-billing-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate your subscription management with Zoho Billing — manage organizations, products, and plans directly from your AI agent.

## Description
Connect your **Zoho Billing** account to any AI agent to streamline your recurring revenue operations. Manage your entire product catalog and subscription infrastructure through natural language.

### What you can do

- **Organization Management** — List, retrieve, and update organizational details to keep your business profile synchronized.
- **Product Catalog** — Create and manage products, toggle their active status, or remove them from your inventory.
- **Plan Configuration** — Handle subscription plans by creating new offerings, updating pricing structures, or retrieving specific plan codes.
- **Lifecycle Control** — Instantly mark products or plans as active/inactive to control what is available to your customers.

### How it works

1. Subscribe to this server
2. Provide your Zoho Billing Access Token and Organization ID
3. Start managing your billing logic from Claude, Cursor, or any MCP client

### Who is this for?

- **Finance Teams** — Quickly audit plans and product statuses without navigating the Zoho dashboard.
- **Product Managers** — Update plan details and product availability directly from the conversation.
- **Developers** — Integrate billing metadata into your workflow to verify plan codes and product IDs while coding.


## Available Tools (101)
- **accept_estimate**: Mark an estimate as accepted
- **apply_credit_note_to_invoices**: Apply credits to multiple invoices
- **associate_coupon**: Associate a coupon with a subscription
- **buy_onetime_addon**: Buy a one-time addon for a subscription
- **cancel_subscription**: Cancel a subscription
- **collect_invoice**: Collect charge via card/bank for an invoice
- **create_addon**: Create an addon
- **create_contact_person**: Create a contact person
- **create_coupon**: Create a coupon
- **create_credit_note**: Create a credit note
- **create_customer**: Create a customer
- **create_estimate**: Create a quote/estimate
- **create_hosted_page_subscription**: Create a subscription via hosted page
- **create_invoice**: Create an invoice
- **create_item**: Create an item
- **create_organization**: Create a new organization
- **create_payment**: Create a payment
- **create_plan**: Create a plan
- **create_product**: Create a product
- **create_subscription**: Create a subscription
- **decline_estimate**: Mark an estimate as declined
- **delete_addon**: Delete an addon
- **delete_card**: Delete a card
- **delete_contact_person**: Delete a contact person
- **delete_coupon**: Delete a coupon
- **delete_credit_note**: Delete a credit note
- **delete_customer**: Delete a customer
- **delete_estimate**: Delete a quote/estimate
- **delete_invoice**: Delete an invoice
- **delete_item**: Delete an item
- **delete_payment**: Delete a payment
- **delete_plan**: Delete a plan
- **delete_product**: Delete a product
- **delete_subscription**: Delete a subscription
- **get_addon**: Retrieve an addon
- **get_card**: Retrieve card info
- **get_contact_person**: Retrieve a contact person
- **get_coupon**: Retrieve a coupon
- **get_credit_note**: Retrieve a credit note
- **get_customer_by_reference**: Retrieve a customer using CRM reference
- **get_customer**: Retrieve a customer
- **get_estimate**: Retrieve a quote/estimate
- **get_event**: Retrieve an event
- **get_hosted_page**: Retrieve hosted page details
- **get_invoice**: Retrieve an invoice
- **get_item**: Retrieve an item
- **get_organization**: Get organization details
- **get_payment**: Retrieve a payment
- **get_plan**: Retrieve a plan
- **get_product**: Retrieve a product
- **get_refund**: Retrieve refund details
- **get_subscription**: Retrieve a subscription
- **list_addons**: List all addons
- **list_cards**: List all active cards for a customer
- **list_contact_persons**: List all contact persons for a customer
- **list_coupons**: List all coupons
- **list_customers**: List all customers
- **list_estimates**: List quotes/estimates
- **list_events**: List of events (last 180 days)
- **list_hosted_pages**: List hosted pages
- **list_invoices**: List all invoices
- **list_items**: List items
- **list_organizations**: List organizations
- **list_payments**: List payments
- **list_plans**: List all plans
- **list_products**: List all products
- **list_subscriptions**: List all subscriptions
- **mark_addon_active**: Mark an addon as active
- **mark_addon_inactive**: Mark an addon as inactive
- **mark_coupon_active**: Mark a coupon as active
- **mark_coupon_inactive**: Mark a coupon as inactive
- **mark_customer_active**: Mark a customer as active
- **mark_customer_inactive**: Mark a customer as inactive
- **mark_item_active**: Mark an item as active
- **mark_item_inactive**: Mark an item as inactive
- **mark_plan_active**: Mark a plan as active
- **mark_plan_inactive**: Mark a plan as inactive
- **mark_product_active**: Mark a product as active
- **mark_product_inactive**: Mark a product as inactive
- **pause_subscription**: Pause a subscription
- **reactivate_subscription**: Reactivate a subscription
- **refund_credit_note**: Refund a credit note
- **refund_payment**: Refund a payment
- **resume_subscription**: Resume a subscription
- **update_addon**: Update an addon
- **update_contact_person**: Update a contact person
- **update_coupon**: Update a coupon
- **update_customer**: Update a customer
- **update_estimate**: Update a quote/estimate
- **update_hosted_page_card**: Update card via hosted page
- **update_hosted_page_subscription**: Update a subscription via hosted page
- **update_invoice**: Update an invoice
- **update_item**: Update an item
- **update_organization**: Update an organization
- **update_payment**: Update a payment
- **update_plan**: Update a plan
- **update_product**: Update a product
- **update_subscription**: Update a subscription
- **void_credit_note**: Void a credit note
- **void_invoice**: Void an invoice
- **writeoff_invoice**: Write off an invoice


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho Billing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my Zoho Billing account."

**🤖 AI Agent:**
> I've retrieved your product list. You have 3 active products: 'Cloud Storage Pro' (ID: prd_123), 'API Access Tier' (ID: prd_456), and 'Legacy Support' (ID: prd_789).

---

**👤 You:**
> "Show me the details for the plan with code 'GOLD-MONTHLY'."

**🤖 AI Agent:**
> Fetching plan details... The 'GOLD-MONTHLY' plan is currently active, priced at $49.00/month, and includes 500GB of storage and priority support.

---

**👤 You:**
> "Create a new plan for the product 'prd_123' using this JSON configuration."

**🤖 AI Agent:**
> I've successfully created the new plan for 'Cloud Storage Pro'. The new plan code is 'SILVER-ANNUAL' and it is now available in your catalog.


## ❓ FAQ

**Q: Can I check the details of a specific subscription plan using its code?**
Yes. Use the `get_plan` tool by providing the unique Plan Code. The agent will return the full configuration, including pricing and billing frequency.

**Q: Is it possible to deactivate a product that is no longer being sold?**
Absolutely. You can use the `mark_product_inactive` tool with the Product ID to hide it from your active catalog without deleting the historical data.

**Q: How do I see all the organizations linked to my account?**
Simply ask the agent to run the `list_organizations` query. It will provide a list of all organizations you have access to within Zoho Billing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-billing-alternative](https://vinkius.com/mcp/zoho-billing-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho Billing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zoho-billing-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho Billing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-billing-alternative": {
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
