# Printify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/printify)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate your print-on-demand business — manage shops, create products, and track orders directly from any AI agent.

## Description
Connect your **Printify** account to any AI agent and manage your entire print-on-demand workflow through natural conversation.

### What you can do

- **Shop Management** — List all connected shops and manage their configurations directly from the cloud
- **Catalog Exploration** — Browse the extensive Printify catalog of blueprints, print providers, and available variants (size/color)
- **Product Lifecycle** — Create, update, and publish products by applying your artwork to specific blueprints and providers
- **Order & Shipping** — Retrieve order details, calculate shipping costs, and send orders to production with ease
- **Webhook Integration** — Manage real-time notifications for order updates and product changes

### How it works

1. Subscribe to this server
2. Enter your Printify Personal Access Token
3. Start managing your e-commerce empire from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Entrepreneurs** — quickly check order statuses and manage product listings without leaving your workspace
- **Designers** — explore the catalog and create new product drafts directly while discussing design ideas
- **Developers** — integrate print-on-demand capabilities into custom workflows or automated agents


## Available Tools
- **calculate_shipping_cost**: Calculate shipping costs for an order
- **create_order**: Create a new order
- **create_product**: Create a new product in a shop
- **create_webhook**: Create a new webhook
- **delete_product**: This is a destructive action.

Delete a product from a shop
- **delete_webhook**: Delete a webhook
- **disconnect_shop**: This is a destructive action.

Disconnect a shop from the Printify account
- **get_blueprint**: Get details for a specific blueprint
- **get_order**: Get details for a specific order
- **get_product**: Get details for a specific product
- **get_shipping**: Get shipping costs and handling times
- **list_blueprints**: List all available blueprints in the Printify catalog
- **list_orders**: List orders in a shop
- **list_print_providers**: List print providers for a specific blueprint
- **list_products**: List products in a shop
- **list_shops**: List all shops in the Printify account
- **list_variants**: List variants for a blueprint and print provider
- **list_webhooks**: List webhooks in a shop
- **publish_product**: Publish a product to a connected store
- **send_order_to_production**: Send a pending order to production
- **update_product**: Update an existing product
- **update_webhook**: Update an existing webhook


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Printify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Printify shops."

**🤖 AI Agent:**
> I've found 2 shops in your account: 'My Awesome Merch' (ID: 12345) and 'Summer Collection' (ID: 67890). Which one would you like to manage?

---

**👤 You:**
> "Show me available t-shirt blueprints in the catalog."

**🤖 AI Agent:**
> Fetching blueprints... I found several options, including the 'Unisex Jersey Short Sleeve Tee' (ID: 6) and the 'Heavy Cotton Tee' (ID: 2). Would you like to see the print providers for one of these?

---

**👤 You:**
> "What are the shipping costs for blueprint 6 from print provider 45?"

**🤖 AI Agent:**
> Checking shipping details... For the Unisex Jersey Tee (ID: 6) via Monster Digital (ID: 45), shipping starts at $4.75 for the US with an estimated handling time of 2-5 business days.


## ❓ FAQ

**Q: How can I see which blank products are available to customize?**
You can use the `list_blueprints` tool. It retrieves the full catalog of available blank items (blueprints) that you can use to create your custom products.

**Q: Is it possible to check shipping costs for a specific product and provider?**
Yes! Use the `get_shipping` tool by providing the Blueprint ID and Print Provider ID. It will return the exact shipping costs and handling times for that combination.

**Q: Can I list all the products currently in one of my shops?**
Absolutely. Use the `list_products` tool with your Shop ID to fetch all products created within that specific shop, including their status and details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/printify](https://vinkius.com/mcp/printify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Printify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `printify` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Printify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "printify": {
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
