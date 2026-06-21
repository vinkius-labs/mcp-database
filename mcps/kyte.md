# Kyte MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kyte)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your POS store — list products, track orders, and audit inventory.

## Description
Connect your AI agent to **Kyte**, the mobile-first POS system designed for small businesses to manage inventory and sales anywhere.

### Key Features

- **Catalog Auditing** — List all products and categories to maintain your digital storefront
- **Order Tracking** — Access and monitor sales orders, status updates, and customer history
- **Inventory Management** — Check stock levels in real-time to prevent sell-outs
- **Customer CRM** — View profiles and transaction history for your store's buyers
- **Financial Visibility** — List transactions and casher logs to monitor store performance

### Simple Setup

1. Subscribe to this server
2. Log in to Kyte, go to **Settings** > **API**, and generate an API Key
3. Enter your key in the configuration panel
4. Start managing your store via natural language


## Available Tools (10)
- **list_kyte_products**: Returns product IDs, names, and current prices.

List all products in the store
- **get_product_details**: Get details for a specific product
- **list_kyte_orders**: Use this to audit recent transactions and delivery statuses.

List recent store orders
- **get_order_details**: Get details for a specific order
- **list_kyte_customers**: List store customers
- **get_customer_profile**: Get details for a specific customer
- **list_product_categories**: List product categories
- **get_inventory_status**: Check current inventory levels
- **list_financial_transactions**: List financial transactions
- **get_kyte_store_status**: Get current store operational status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kyte** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my Kyte store"

**🤖 AI Agent:**
> I've retrieved your product catalog. You have 25 items across 3 categories. Notable products include 'Organic Coffee' ($15.00) and 'Ceramic Mug' ($12.50). Would you like to check inventory levels for these?

---

**👤 You:**
> "Show the last 5 orders"

**🤖 AI Agent:**
> Retrieving recent sales… The last 5 orders total $350.50. 3 are 'Completed', 1 is 'Pending Payment', and 1 is 'Cancelled'. Would you like the details for the pending order?

---

**👤 You:**
> "Which products are low on stock?"

**🤖 AI Agent:**
> Checking inventory… 2 products are below your warning level: 'Artisanal Honey' (2 left) and 'Handmade Soap' (0 left). Should I list these for your next supplier order?


## ❓ FAQ

**Q: Where do I find my Kyte API Key?**
Log in to the Kyte web dashboard or app, navigate to **Settings**, and look for the **API** or **Developer** section to generate a key.

**Q: Can I see stock levels for specific products?**
Yes, use the `get_inventory_status` tool to see quantities for all products in your catalog.

**Q: Does this support multiple store locations?**
The API key is typically linked to a specific store account. Ensure you are using the correct key for the desired store.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kyte](https://vinkius.com/mcp/kyte)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kyte** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kyte` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kyte** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kyte": {
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
