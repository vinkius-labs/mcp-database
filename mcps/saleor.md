# Saleor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/saleor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Connect your AI to your headless Saleor e-commerce store. Seamlessly manage products, audit recent orders, and assist customers natively through your chat.

## Description
Empower your conversational AI with deep access to **Saleor**, the highly scalable, headless GraphQL-first e-commerce engine designed around high performance experiences. Connect your environment to actively manage your daily retail store operations, inspect products, or troubleshoot customer inquiries natively from chat.

### What you can do

- **Inventory & Catalogs** — Quickly inspect your store's entire directory (`list_products`). Retrieve detailed specifics such as available variants, pricing, and precise stock configurations per individual product ID (`get_product`).
- **Category Orchestration** — Browse how your catalog is organized internally by fetching collections (`list_collections`) and sub-categories (`list_categories`) without toggling through web dashboards.
- **Order Fulfillment Auditing** — Easily review a list of the latest purchases happening on your platform (`list_orders`) and quickly grab comprehensive snapshots of individual receipts, line items, or billing addresses (`get_order`).
- **Customer Assistance** — Query your database to find registered profiles globally (`list_customers`) or drill down into specific shopper's order details and status natively (`get_customer`).
- **Architecture Inspection** — Inspect high-level configuration such as default currencies and active regions by utilizing `list_channels` or retrieving global details via `get_shop_info`.

### How it works

1. Authorize the Saleor mapping tools within your workspace integrations.
2. Access your main Saleor backend dashboard.
3. Generate a dedicated internal App Token containing adequate reading/managing authorizations.
4. Enter the Saleor Cloud GraphQL API Endpoint and the generated access token simultaneously into the connection securely.
5. Ask the AI: "Find out order specifics and shipping details for order number '334'."


## Available Tools (10)
- **get_customer**: Retrieves profile information and order history for a specific customer
- **get_order**: Retrieves details for a specific order
- **get_product**: Retrieves details for a specific product by ID
- **get_shop_info**: Retrieves global shop configuration
- **list_categories**: Lists all product categories
- **list_channels**: Lists all configured sales channels
- **list_collections**: Lists all product collections
- **list_customers**: Lists all customers/users registered in the shop
- **list_orders**: Lists recent customer orders
- **list_products**: Lists all products in the Saleor store


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Saleor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my store."

**🤖 AI Agent:**
> I've carefully queried the Saleor GraphQL endpoint and successfully retrieved the top 20 verified product listings natively currently published within the e-commerce directory mapped accurately here.

---

**👤 You:**
> "Find out order specifics and shipping details for order number '334'."

**🤖 AI Agent:**
> I checked order '334'. It was placed cleanly by 'customer@example.com'. The exact billing address covers CA, and unfortunately the fulfillment standing reveals it's listed strictly as unfulfilled currently.

---

**👤 You:**
> "What currencies does the store utilize in the available sales channels?"

**🤖 AI Agent:**
> I queried the high-level Sales Channels settings securely. You maintain three active pipelines functioning flawlessly: USD for the primary US store, GBP representing the UK environment, and EUR cleanly implemented on the continental node.


## ❓ FAQ

**Q: Can the AI forcefully complete, modify, or delete existing customer orders in my Saleor shop?**
No. The integration focuses securely on read-only queries. It fetches critical information such as stock numbers, recent sales, and product characteristics without actively overwriting, resolving, or destroying records to protect e-commerce transactional integrity.

**Q: Does it require a specific Saleor Cloud paid plan to use this integration?**
A specific plan is not heavily mandated by the tool itself as long as your environment successfully exposes the standard backend GraphQL endpoint and permits the creation of standard administrative App Tokens within your environment policies.

**Q: Why do some commands ask for a 'GraphQL ID' specifically?**
Saleor’s core architecture uses unique Base64-encoded strings (like 'UHJvZHVjdDoxMjM=') as identifiers natively, rather than typical numeric database IDs. Always use the `list_orders` or `list_products` tools first to discover these exact encoded IDs natively, then seamlessly pass them to the exact fetching tools to pull their full snapshots.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/saleor](https://vinkius.com/mcp/saleor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Saleor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `saleor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Saleor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "saleor": {
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
