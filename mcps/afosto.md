# Afosto MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/afosto)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Retail and e-commerce engine — manage orders, inventory, products, and customers via AI.

## Description
Connect your **Afosto Retail Engine** account to your AI agent to unlock enterprise-grade e-commerce orchestration. From managing multi-channel orders to monitoring real-time inventory across warehouses and auditing product catalogs, your agent handles your retail stack through natural conversation.

### What you can do

- **Order Orchestration** — List and audit multi-channel orders, check fulfillment statuses, and retrieve technical metadata
- **Inventory Management (WMS)** — Monitor real-time stock levels across multiple locations and identify replenishment needs
- **Product Catalog Oversight** — List products, variants, and pricing to ensure your storefront is always synchronized
- **Customer Intelligence** — Retrieve centralized customer profiles and interaction history to support sales and support
- **Retail Insights** — Quickly identify sales trends or inventory bottlenecks directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Afosto Client ID and Client Secret
3. Start managing your retail operations and monitoring performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — automate order audits and monitor storefront health across multiple regions
- **Operations & WMS Leads** — check real-time inventory levels and manage warehouse movements effortlessly
- **Customer Support Teams** — quickly look up customer history and order details to resolve inquiries
- **Business Analysts** — retrieve granular retail data for sales reporting and performance analysis


## Available Tools
- **list_orders**: Retrieve recent multi-channel eCommerce orders aggregated by Afosto
- **list_inventory**: Retrieve real-time inventory and stock levels aggregated by warehouse distribution
- **list_products**: Retrieve the complete product catalog, highlighting active variants and their pricing
- **list_customers**: Retrieve centralized customer profile data and their historic eCommerce behavior


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Afosto** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pending orders from the last 24 hours."

**🤖 AI Agent:**
> I've retrieved your pending orders. You have 15 new orders awaiting fulfillment from your Web Store and Amazon channels. Would you like to see the inventory status for the items in these orders?

---

**👤 You:**
> "What is the current stock level for 'Wireless Headphones' in all warehouses?"

**🤖 AI Agent:**
> I've checked the inventory. You have 120 units of 'Wireless Headphones' available: 80 in Main Warehouse and 40 in Northern Hub. There are 10 units currently reserved for pending orders.

---

**👤 You:**
> "Search for a customer profile with email 'john.doe@example.com'."

**🤖 AI Agent:**
> I've found the profile for John Doe. He is a 'Gold' tier customer with 5 lifetime orders. His last order was 2 weeks ago. Would you like to see his full interaction history?


## ❓ FAQ

**Q: How do I find my Afosto API credentials?**
Log in to the Afosto Admin App, navigate to **Company** > **API Settings**. You can create a new integration there to generate your Client ID and Client Secret.

**Q: Can I check stock levels across multiple warehouses?**
Yes! Use the `list_inventory` tool. It provides real-time stock data aggregated by location, helping you manage omnichannel fulfillment.

**Q: Does this support multi-channel orders?**
Absolutely. The `list_orders` tool retrieves orders from all connected sales channels, including B2B, B2C, and integrated marketplaces.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/afosto](https://vinkius.com/mcp/afosto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Afosto** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `afosto` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Afosto** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "afosto": {
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
