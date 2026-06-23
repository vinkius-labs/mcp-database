# Jumpseller MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jumpseller)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage products, orders, and customers via Jumpseller API.

## Description
Empower your AI agents with Jumpseller's e-commerce platform. This MCP server allows you to list and retrieve products and orders, manage customers and categories, track store pages, and view general store information directly through the Jumpseller API. Ideal for automating store management and order processing.


## Available Tools (10)
- **get_order**: Returns line items, shipping addresses, payment status, and customer notes. Use this for order troubleshooting or providing customer support.

Retrieves details for a specific order
- **get_product**: Returns descriptions, detailed pricing, variants, and image metadata. Use this when the user needs to analyze a specific item or prepare product listings.

Retrieves details for a specific product
- **get_store_info**: Useful for verifying store configuration.

Retrieves general information about your Jumpseller store
- **list_categories**: Useful for understanding store organization and finding products within specific niches.

Lists all product categories
- **list_customers**: Returns names, emails, and order counts. Use this when the user wants to identify repeat buyers or audit the customer list.

Lists all customers in your store
- **list_orders**: Includes order IDs, totals, and current fulfillment status. Essential for monitoring recent sales activity.

Lists all orders in your store
- **list_pages**: ) from the Jumpseller store. Useful for auditing site content and navigation.

Lists all pages in your store
- **list_payment_methods**: g., PayPal, Stripe) in the store. Useful for auditing checkout options.

Lists configured payment methods
- **list_products**: Returns product names, SKUs, prices, and IDs. Use this to identify items for stock management or product analysis.

Lists all products in your Jumpseller store
- **list_shipping_methods**: Useful for auditing fulfillment logic and carrier configurations.

Lists configured shipping methods


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jumpseller** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active products in my Jumpseller store."

**🤖 AI Agent:**
> I'll fetch the complete list of products from your Jumpseller account.

---

**👤 You:**
> "Show me the last 5 orders received."

**🤖 AI Agent:**
> I'll retrieve the most recent orders from your store for you.

---

**👤 You:**
> "Check the details for customer ID '123'."

**🤖 AI Agent:**
> I'll look up the full profile and history for that specific customer in Jumpseller.


## ❓ FAQ

**Q: How do I get Jumpseller API credentials?**
Log in to your Jumpseller admin panel, navigate to Checkout > API, and find your Login Key and Auth Token.

**Q: Does it support order details?**
Yes, you can list all orders or retrieve full details for any specific order using the corresponding tools.

**Q: Can I see payment and shipping methods?**
Yes, this MCP provides tools to list all configured payment and shipping methods in your Jumpseller store.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jumpseller](https://vinkius.com/mcp/jumpseller)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jumpseller** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jumpseller` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jumpseller** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jumpseller": {
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
