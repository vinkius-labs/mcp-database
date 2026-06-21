# BigCommerce MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bigcommerce)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate eCommerce native workflows via BigCommerce — manage full catalogs, orders, customers, and active coupons directly from your AI agent.

## Description
Connect your **BigCommerce** account to any AI agent and empower it to operate your entire storefront backend, analyzing transaction metrics, verifying inventory structures, and managing live customer payloads natively.

### What you can do

- **Catalog & Products** — Browse product pages, retrieve deep dimensional variations explicitly, and trace active brand/category mappings
- **Orders & Transactions** — Fetch macro native lists of live orders, dive into specific payloads, and dissect physical line-items independently
- **Customers & Profiles** — Explore natively attached user profiles extracting precise lifetime order impact and structural routing paths
- **Coupons & Rules** — Evaluate distinctly mapped active discounting strategies, validating constraints securely inside boundaries
- **Store Information** — Audit high-level enterprise configuration bounds capturing localized active settings intuitively

### How it works

1. Subscribe to this server
2. Enter your BigCommerce API Token and Store Hash
3. Start fetching operational logistics from Claude, Cursor, or any MCP-compatible environment

Command your sales terminal directly without logging into complex control panels and drilling into submenus. Your AI retrieves exact order details the moment you request them.

### Who is this for?

- **E-Commerce Managers** — oversee gross transactional behavior checking specific line-items and discounting validity fluidly
- **Backend Developers** — prototype custom cart endpoints ensuring product variants match the catalog logic quickly via chat
- **Customer Support** — locate explicit order problems, verify exact shipping details, and pull underlying customer data in seconds


## Available Tools
- **list_products**: List paginated BigCommerce catalog products
- **get_order**: Retrieve the exact payload for a BigCommerce native order
- **list_customers**: List paginated explicitly registered BigCommerce customers
- **list_categories**: List BigCommerce native hierarchy categories
- **list_brands**: List all explicitly mapped BigCommerce Brands
- **get_order_products**: Get line items constrained to an explicit Order
- **list_coupons**: List all configured BigCommerce coupons logically
- **get_product**: Get complete details of an explicit BigCommerce product
- **list_orders**: List paginated BigCommerce native orders
- **get_store_info**: Retrieve macroscopic BigCommerce store mapping metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BigCommerce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List standard product endpoints matching page 1 in the active catalog."

**🤖 AI Agent:**
> Scanning catalog logic globally: Extracted 25 root products from page 1 securely. Top variants included 'Ergo Office Chair' (ID: 981, $299.00) and 'Standing Desk Model X' cleanly indexed alongside live inventory levels natively.

---

**👤 You:**
> "Fetch strictly explicitly details of BigCommerce Order ID 1420."

**🤖 AI Agent:**
> Loaded Order #1420 structurally. The state reflects 'Awaiting Shipment' mapped via standard Visa processing yielding a subtotal baseline summing exactly $1,402. Shipping route addresses correctly matched to physical regions.

---

**👤 You:**
> "Report active coupon arrays dynamically to understand limitations natively."

**🤖 AI Agent:**
> Auditing active logic constraints. Pulled explicit coupon data revealing 'HOLIDAY20' discounting rigidly 20% strictly bounded excluding digital categories and retaining an expiration cap naturally.


## ❓ FAQ

**Q: Can my agent see exactly what items are inside a specific order?**
Yes. While `get_order` yields the financial macro parameters, executing `get_order_products` descends specifically into the transaction to parse independent line items, variants, and precise inventory counts attached directly.

**Q: Are promotional coupons and discounts strictly observable?**
Absolutely. You can request `list_coupons` to explicitly audit exact active promo codes mapping boundaries like expiration constraints implicitly inside the logic.

**Q: Can my AI automatically complete refunds or modify orders?**
No. To ensure absolute data governance regarding financial boundaries, endpoints are firmly scoped to retrieving live operational states recursively and reading inventory without risking active payment mutation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bigcommerce](https://vinkius.com/mcp/bigcommerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BigCommerce** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bigcommerce` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BigCommerce** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bigcommerce": {
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
