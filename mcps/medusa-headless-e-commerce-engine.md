# Medusa (Headless E-commerce Engine) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/medusa-headless-e-commerce-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage headless commerce via MedusaJS — search products, track orders, and audit customer data.

## Description
Connect your **MedusaJS** store to any AI agent and take full control of your enterprise-grade headless commerce operations, catalog management, and customer CRM through natural conversation.

### What you can do

- **Product Orchestration** — List and retrieve detailed product metadata by ID, including pricing, SKU-level variants, and media galleries directly from your agent
- **Order Monitoring** — List recent commerce orders and retrieve full line-item details, shipping addresses, payment statuses, and fulfillment histories securely
- **Payment Capture** — Trigger manual capture actions for authorized orders to move funds from the customer vault into your store's processing pipeline in real-time
- **Customer CRM** — Manage your registered customer directory, retrieve detailed profiles, and audit internal flags or default shipping addresses natively
- **Regional Auditing** — List configured store regions to understand localized tax rates, currency logic, and enabled payment providers across different geographies
- **Collection Management** — Navigate product collections and taxonomies to verify store organization and group-based product distributions efficiently
- **Store Configuration** — Extract store-level metadata including base URLs and default region settings to ensure accurate cross-border commerce auditing

### How it works

1. Subscribe to this server
2. Enter your Medusa Store URL and Admin API Token
3. Start managing your headless storefront from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Headless Developers** — verify API responses and audit product variant mappings directly from your workspace for rapid debugging
- **E-commerce Managers** — monitor order flows and customer profiles across multiple store regions through natural conversation without manual dashboard exports
- **Store Administrators** — manage collection hierarchies and capture authorized payments efficiently to maintain high-performance commerce operations


## Available Tools
- **capture_payment**: Capture payment for a Medusa order
- **list_collections**: List Medusa product collections
- **list_customers**: List Medusa CRM customers
- **get_customer**: Get Medusa customer explicitly by ID
- **get_order**: Get Medusa order by ID. Returns line items, billing/shipping addresses, payment status, fulfillment status
- **get_product**: Get Medusa product by ID. Returns full details: variants, options, prices
- **list_orders**: List Medusa orders
- **list_products**: List Medusa products. Medusa is a headless open-source commerce engine
- **list_regions**: List Medusa regions (currency, tax rates, payment providers)
- **get_store_config**: Get Medusa store configuration (supported currencies, default region)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Medusa (Headless E-commerce Engine)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my Medusa store"

**🤖 AI Agent:**
> I've retrieved your product list. Highlights include the 'Classic Tee' (ID: prod-123), 'Cargo Pants' (ID: prod-456), and 'Tech Backpack' (ID: prod-789). Would you like to see the inventory levels for any of these?

---

**👤 You:**
> "Show me the last 5 orders placed today"

**🤖 AI Agent:**
> Retrieving latest orders… I've identified 5 new orders. Highlights: Order #1001 ($45.50, Payment: Captured), Order #1002 ($120.00, Payment: Awaiting), and Order #1003 ($15.99, Status: Fulfilled). Would you like to see the shipping address for the pending order?

---

**👤 You:**
> "Capture the payment for order ID 'order-987'"

**🤖 AI Agent:**
> Executing payment capture… Success. For order 'order-987', the funds have been captured from the customer's payment method. The order status has been updated to 'Awaiting Fulfillment' in Medusa.


## ❓ FAQ

**Q: Can I capture a payment for an authorized order using my agent?**
Yes. Use the `capture_payment` tool with a specific Order UUID. Your agent will trigger the action against your payment provider (e.g., Stripe) to finalize the fund transfer for the order immediately.

**Q: How do I check the tax rates and currencies for a specific region?**
The `list_regions` tool retrieves all configured geographical zones in Medusa. Your agent will expose the localized currency logic, tax rates, and enabled payment methods assigned to each region.

**Q: Can my agent retrieve the detailed variants and prices for a product?**
Absolutely. Use the `get_product` tool by providing the Product ID. Your agent will fetch the full object including nested variants, options (size, color), and pricing arrays for all configured regions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/medusa-headless-e-commerce-engine](https://vinkius.com/mcp/medusa-headless-e-commerce-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Medusa (Headless E-commerce Engine)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `medusa-headless-e-commerce-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Medusa (Headless E-commerce Engine)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "medusa-headless-e-commerce-engine": {
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
