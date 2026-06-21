# PrestaShop MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/prestashop)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Bring your PrestaShop store to your AI — orchestrate orders, extract deep product metadata, and track inventory stock levels natively via chat.

## Description
Empower your AI agents to directly manage and analyze your **PrestaShop** eCommerce operations. Using the official Webservice API, your LLMs can scan live orders, inspect nested product XMLs, and monitor available stock without touching the back-office dashboard.

### What you can do

- **Order Logistics** — Instruct the AI to fetch `list_orders` or dig into a specific cart dropping absolute constraints via `get_order` to understand what was purchased
- **Product Catalog** — Pull arrays containing precise SKU data, category mappings, and pricing logic (`list_products`, `get_product`)
- **Stock Management** — Find out exactly how many units are permitted for checkout operations by retrieving native stock arrays (`list_stock`)
- **CRM & Addresses** — Query your database identifying customer histories (`list_customers`) correlated with absolute dispatch matrices (`list_addresses`)

### How it works

1. Subscribe to this MCP server
2. Provide your PrestaShop URL and your Webservice Key
3. Start mapping your e-commerce operations in Claude, Cursor, or any compatible client

No exporting CSVs or navigating XML trees manually. When a customer complains about an order, ask 'Retrieve Order ID 452 and list its items'. The AI reads the native integration flawlessly.

### Who is this for?

- **E-commerce Managers** — evaluate order volumes, check inventory depths, and read category structures instantly
- **Frontend Developers** — ask the AI to map specific product IDs into JSON arrays when building headless frontends
- **Support Teams** — track physical delivery addresses mapping direct customer disputes without accessing the admin panel


## Available Tools (10)
- **list_products**: Use the `limit` parameter string to bound results (e.g., `0,20`). Native XML responses are parsed and converted to structured arrays.

List PrestaShop products with full details, retrieving items from the open-source eCommerce catalog
- **get_product**: Get an individual PrestaShop product by ID, returning full pricing, descriptions, and category associations
- **list_orders**: Limits response arrays via bounds (e.g., `0,20`). Critical for scanning recent sales history mapped directly against specific customer IDs.

List PrestaShop active orders retrieving order references, current fulfillment statuses, and totals
- **get_order**: Maps raw Webservice XML nodes into consumable arrays.

Get PrestaShop nested order by explicit ID, tracing line items, billing/shipping boundaries, and payment success paths
- **list_customers**: Limits response arrays via bounds (e.g., `0,20`). Maps basic CRM points for subsequent order correlations.

List PrestaShop customers tracking emails, first and last names, and account creation dates
- **list_categories**: List all PrestaShop root and child categories dictating store navigation geometry
- **list_addresses**: Limits response arrays via bounds (e.g., `0,20`). Used to analyze spatial destination data linked implicitly to customers and orders.

List physical PrestaShop customer/order addresses mapping delivery logistics lines
- **list_stock**: Resolves specific stock trace items which dictate the physical inventory logic overriding standard product rules.

List PrestaShop available stock quantities mapping exact units over specific complex item structures
- **get_stock**: Get PrestaShop specific stock quantity node explicitly by constrained resource ID
- **list_currencies**: List all active currencies configured and accepted implicitly within the target store interface


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PrestaShop** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 orders placed on the store. Are there any pending ones?"

**🤖 AI Agent:**
> Querying `list_orders` with limit `0,5`. I found 5 recent purchases. Orders 101 through 104 are marked 'Shipped'. However, Order 105 (Total 145 USD) is currently held under 'Awaiting Bank Wire Payment'.

---

**👤 You:**
> "Get the product details linked to ID 42. Tell me its exact category bindings."

**🤖 AI Agent:**
> I extracted `get_product` for ID 42 ('Wireless Headphones v2'). Inside its nested `associations>categories` array, it is bound to Category ID 3 ('Electronics') as well as the default Home category (ID 2). Its base price is set at 99.99.

---

**👤 You:**
> "Check our current stock level constraints available at Stock ID '15'."

**🤖 AI Agent:**
> Via `get_stock` targeting ID 15, the structural array dictates that there are exactly `7` physical units physically authorized for checkout operations, tied implicitly to Product ID `42`.


## ❓ FAQ

**Q: Can the AI handle PrestaShop's complex XML responses?**
Yes. While PrestaShop's Core API sends XML trees, the AI parses nodes extracting items, IDs, and pricing fluidly, eliminating the need for you to read tag-heavy formats manually.

**Q: Is there a way to limit the amount of products or orders I query?**
Absolutely. Functions like `list_products` and `list_orders` accept a `limit` parameter string in bounds format (like `0,20`). Just ask the AI to 'show me the first 5 orders'.

**Q: Can it inspect how many physical items are in stock?**
Yes. Under the hood, PrestaShop splits stock models. Using `list_stock` and `get_stock`, the AI retrieves the exact array nodes managing physical stock overriding quantities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prestashop](https://vinkius.com/mcp/prestashop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PrestaShop** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `prestashop` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PrestaShop** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prestashop": {
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
