# Amazon Selling Partner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amazon-selling-partner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

E-commerce and marketplace orchestration — manage orders, FBA inventory, and catalogs via AI.

## Description
Connect your **Amazon Selling Partner (SP-API)** account to your AI agent to unlock professional e-commerce and marketplace orchestration. From managing incoming orders and auditing FBA inventory to researching the Amazon product catalog and requesting asynchronous reports, your agent handles your seller operations through natural conversation.

### What you can do

- **Order Management** — List incoming orders and retrieve detailed item lists for fulfillment
- **FBA Inventory Auditing** — Retrieve inventory summaries and monitor stock levels across Amazon fulfillment centers
- **Catalog Research** — Search the Amazon catalog by ASIN or keywords to retrieve technical product metadata
- **Reporting Orchestration** — Request asynchronous seller reports and monitor their processing statuses
- **Financial Insights** — Retrieve financial event groups and marketplace participation details directly from chat

### How it works

1. Subscribe to this server
2. Enter your LwA Client ID, Client Secret, Refresh Token, Region, and Marketplace ID
3. Start managing your Amazon Seller Central operations and monitoring performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Amazon Sellers** — automate order audits and monitor FBA inventory levels effortlessly
- **E-commerce Managers** — retrieve catalog details and research competitors' ASINs on the fly
- **Logistics Operations** — track fulfillment requirements and manage stock replenishment alerts
- **Financial Analysts** — request financial event reports and monitor revenue across global marketplaces


## Available Tools
- **list_orders**: List Amazon orders
- **get_order_items**: Get order items
- **list_fba_inventory**: List FBA inventory
- **search_catalog**: Search Amazon catalog
- **get_catalog_item**: Get catalog item
- **create_report**: g. GET_MERCHANT_LISTINGS_ALL_DATA).

Request a report
- **get_report_status**: Check report status
- **list_financial_events**: List financial events
- **list_marketplaces**: List marketplaces
- **list_product_types**: List product types


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amazon Selling Partner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent Amazon orders."

**🤖 AI Agent:**
> I've retrieved your recent orders. There are 5 pending orders waiting for fulfillment. Would you like me to retrieve the order items for the first order in the list?

---

**👤 You:**
> "Show the FBA inventory summary for my top products."

**🤖 AI Agent:**
> I've checked your FBA inventory. Your top selling item currently has 120 units available, with 25 units inbound. One of your items is out of stock. Let me list the details for you.

---

**👤 You:**
> "Search the Amazon catalog for ASIN 'B012345678'."

**🤖 AI Agent:**
> I've retrieved the catalog details for ASIN B012345678. It's a 'Wireless Bluetooth Headset' currently listed in the Electronics category. Would you like to see the pricing and dimensions metadata?


## ❓ FAQ

**Q: How do I get my Amazon SP-API credentials?**
You need to register a private application in the Amazon Seller Central (Partner Network > Develop Apps). You will get an LwA Client ID and Secret. You then self-authorize the app to get a long-lived Refresh Token.

**Q: Which region should I choose?**
Select the region that matches your target marketplace: **NA** (North America - US, CA, MX, BR), **EU** (Europe - UK, DE, FR, IT, ES, etc.), or **FE** (Far East - JP, AU, SG).

**Q: Can I request PII data like customer names?**
This MCP server uses standard SP-API tokens. Some PII data (Personally Identifiable Information) in orders requires a Restricted Data Token (RDT), which must be specifically requested in the API call and authorized in your app's roles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazon-selling-partner](https://vinkius.com/mcp/amazon-selling-partner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amazon Selling Partner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `amazon-selling-partner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amazon Selling Partner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amazon-selling-partner": {
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
