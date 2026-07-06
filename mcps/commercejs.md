# Commerce.js MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/commercejs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your e-commerce store via Commerce.js — list products, manage carts, and handle orders directly from any AI agent.

## Description
Connect your **Commerce.js** (Chec) account to any AI agent and take full control of your e-commerce operations through natural conversation.

### What you can do

- **Product Catalog** — List all products, filter by category, and fetch detailed metadata for specific items using IDs.
- **Cart Management** — Create new carts, add products with specific quantities, and update line items seamlessly.
- **Checkout Flow** — Generate checkout tokens from carts to prepare for secure transactions and capture orders with customer details.
- **Order Processing** — List recent orders, retrieve specific order details, and manage fulfillment data.
- **Category Organization** — Browse store categories to understand your product hierarchy and improve navigation.

### How it works

1. Subscribe to this server
2. Enter your Chec Public Key and Secret Key
3. Start managing your store from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Store Managers** — quickly check inventory levels and order statuses without logging into the dashboard
- **Developers** — test cart and checkout logic directly from the terminal or code editor
- **Support Teams** — look up customer order details instantly to provide faster assistance


## Available Tools (10)
- **get_order**: Requires Secret Key.

Retrieve a specific order
- **get_product**: Retrieve a specific product
- **list_categories**: List categories
- **list_orders**: Requires Secret Key.

List orders
- **list_products**: Can be filtered by category or paginated.

List products in the store
- **update_cart_item**: Update a cart item
- **add_to_cart**: Add an item to a cart
- **capture_order**: Capture an order
- **create_cart**: Create or retrieve a cart
- **generate_checkout_token**: Generate a checkout token


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Commerce.js** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 5 products in my store."

**🤖 AI Agent:**
> I've retrieved your products. Your top items include 'Wireless Headphones' (prod_123) and 'Smart Watch' (prod_456). Would you like more details on any of these?

---

**👤 You:**
> "Create a cart and add 2 units of product prod_Q123."

**🤖 AI Agent:**
> Cart created successfully (ID: cart_abc123). I have added 2 units of 'Organic Coffee Beans' to it. The current subtotal is $30.00.

---

**👤 You:**
> "Show me the details for order ord_987."

**🤖 AI Agent:**
> Order ord_987 was placed by John Doe. It contains 1x 'Gaming Mouse' and is currently marked as 'Fulfilled'. Shipping was handled via Standard Delivery.


## ❓ FAQ

**Q: Can I filter products by a specific category?**
Yes! You can use the `list_products` tool and provide a `category_id` to retrieve only the products belonging to that specific group.

**Q: How do I view the details of a customer's order?**
Use the `get_order` tool with the specific Order ID. Note that viewing orders requires your Secret Key to be configured in the server settings.

**Q: Can the AI help me manage shopping carts for customers?**
Absolutely. The agent can use `create_cart`, `add_to_cart`, and `update_cart_item` to build and modify shopping sessions dynamically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/commercejs](https://vinkius.com/mcp/commercejs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Commerce.js** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `commercejs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Commerce.js** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "commercejs": {
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
