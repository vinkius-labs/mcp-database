# Spocket MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spocket)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate dropshipping via Spocket — browse catalogs, check real-time inventory, and manage customer orders directly from any AI agent.

## Description
Connect your **Spocket** account to any AI agent to streamline your dropshipping and e-commerce operations through natural conversation.

### What you can do

- **Product Discovery** — List the Spocket catalog and fetch detailed metadata for specific products using `list_products` and `get_product`.
- **Inventory Monitoring** — Check real-time stock levels for products and variants to ensure availability with `get_inventory`.
- **Order Management** — Create new customer orders and track their fulfillment status using `create_order` and `get_order`.
- **Catalog Filtering** — Search for products by category or use pagination to browse large inventories efficiently.

### How it works

1. Subscribe to this server
2. Enter your Spocket API Key
3. Start managing your store from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Store Owners** — quickly check stock and place orders without leaving your workspace.
- **Dropshippers** — automate product research and order tracking through simple chat commands.
- **Developers** — integrate Spocket data into custom workflows or dashboards without building complex integrations.


## Available Tools
- **create_order**: Create a new order in Spocket
- **get_inventory**: Check stock levels for a Spocket product
- **get_order**: Get Spocket order status
- **get_product**: Get details for a specific Spocket product
- **list_products**: Supports pagination and category filtering.

Get all products from Spocket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spocket** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in the 'Electronics' category from Spocket."

**🤖 AI Agent:**
> I've found several products in the Electronics category. Here are the top items: 'Wireless Earbuds' (ID: sp_789) and 'Smart Watch' (ID: sp_456). Would you like more details on any of these?

---

**👤 You:**
> "Check the inventory level for product ID sp_123."

**🤖 AI Agent:**
> The current inventory for product sp_123 is 45 units. It is currently in stock and available for ordering.

---

**👤 You:**
> "Create an order for John Doe at 123 Main St, New York, NY 10001, US for product sp_456 with quantity 1."

**🤖 AI Agent:**
> Order successfully created! The Order ID is ord_556677. You can track its status using this ID.


## ❓ FAQ

**Q: Can I check the current stock level for a specific product?**
Yes! Use the `get_inventory` tool with the product ID. The agent will return the real-time stock levels for that item or its variants.

**Q: How do I track the status of a customer's order?**
Simply provide the Order ID to the `get_order` tool. Your AI agent will retrieve the current fulfillment status and order details from Spocket.

**Q: Can I filter products by a specific category?**
Yes, the `list_products` tool allows you to pass a `category` parameter to narrow down the results to only the items you are interested in.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spocket](https://vinkius.com/mcp/spocket)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spocket** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `spocket` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spocket** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spocket": {
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
