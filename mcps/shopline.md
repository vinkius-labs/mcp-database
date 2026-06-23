# Shopline MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shopline)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to autonomously manage your Shopline store. Audit products, track order fulfillment, fetch customer profiles, and monitor store collections seamlessly.

## Description
Grant your AI agent (like Claude or Cursor) absolute administrative dominion over your custom Shopline commerce operations. The **Shopline MCP** equips your LLM to act as a fully autonomous moderator and store operations manager. Forget navigating complex vendor panels—now you can manage supply, audit order pipelines, and track your customer community exclusively via natural conversational prompts interacting deeply with your Admin API.

### What you can do

- **Inventory & Listing Moderation** — Crawl through product catalogs via `list_products`. Found a low-stock alert or need details? Drill down seamlessly with `get_product_details` directly from your IDE
- **Live Transaction Steering** — Audit ongoing orders and fulfillment pipelines with `list_orders` and `get_order_details`. Automatically extract revenue and check what customers bought without logging in
- **Customer Profiling & Catalog Curation** — Interrogate the platform using `list_customers` to investigate VIP accounts or analyze demographics, while scanning categorized inventory using `list_collections`

### How it works

1. Anchor this core interface directly within your native MCP agent framework
2. Safely entrench your `SHOPLINE_ACCESS_TOKEN` matrix inside the workspace to lock down security boundaries
3. Engage your agent pragmatically: "List all recent orders, analyze their total value, and tell me if we are low on the latest collection products!"


## Available Tools (7)
- **list_products**: Lists all products in the Shopline store
- **get_product_details**: Retrieves details for a specific product
- **list_orders**: Lists all store orders
- **get_order_details**: Retrieves details for a specific order
- **list_customers**: Lists store customers
- **list_collections**: Lists all product collections
- **get_shop_info**: Retrieves information about the Shopline store


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shopline** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the 10 most recent orders and summarize the total value and items purchased."

**🤖 AI Agent:**
> Aggregating the `list_orders` query. I have parsed the latest 10 transactional blocks. The sum of the finalized captures amounts to $145.90. Items dispersed primarily included variable SKUs targeting "Deluxe Dog Collar" variants predominantly acquired across 4 unique client interactions safely tracked.

---

**👤 You:**
> "Examine product ID '20410' and tell me if any variants are out of stock."

**🤖 AI Agent:**
> Running the precise interrogation matrix using `get_product_details` for product '20410'... Found 3 associated variant IDs. SKU 'SL-VAB-M' (Medium sized) reports 0 quantity explicitly across the aggregated node. Both Small and Large variants possess strong buffer reserves remaining actively published.


## ❓ FAQ

**Q: Can the AI forcefully transition or edit an order status directly?**
Currently, the integration specifically implements reading mechanisms (`list_orders`, `get_order_details`) as a query matrix tailored explicitly around monitoring and auditing. It does not actively expose a write mutation structurally to alter or destroy existing operational orders.

**Q: Why do I need a Custom Admin API integration token and not a public one?**
Because the `Admin API` is the unadulterated backend context designed primarily for secure backend logic rather than client storefront interfaces. This token permits your integration to run system-level monitoring, extraction over raw orders, and sensitive customer profiles natively.

**Q: Is this tool accessing the Shopline GraphQL portal or REST architecture limitlessly?**
By structural intent, we implement targeted endpoints using Shopline's scalable endpoints to parse specifically filtered responses like single pagination segments to avoid massive latency. You interact efficiently bypassing raw structural limits naturally via these curated `list_x` and `get_x` procedures.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shopline](https://vinkius.com/mcp/shopline)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shopline** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shopline` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shopline** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shopline": {
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
