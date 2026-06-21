# Nabis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nabis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Cannabis wholesale and distribution — manage orders, inventory, and retailers via Nabis.

## Description
Connect your **Nabis** account to empower your AI agents with wholesale and distribution capabilities. This server interfaces with the **Nabis Platform V2 API** for real-time visibility into the cannabis supply chain.

### What you can do

- **Order Management** — List and inspect wholesale orders across markets like CA and NY
- **Inventory Visibility** — Track stock levels across different warehouses in real-time
- **Retailer Insights** — Access detailed information about retailers and their license status
- **Financial Monitoring** — Track invoices, aging reports, and payment statuses
- **Logistics Coordination** — Stay updated on warehouse locations and delivery schedules

### How it works

1. Subscribe to this server
2. Enter your **Nabis Access Token** from the developer portal
3. Start managing your cannabis operations from Claude, Cursor, or any MCP client


## Available Tools
- **get_days_off**: Get Nabis days off
- **get_invoice**: Get invoice details
- **get_order**: Get details for a specific order
- **get_retailer**: Get retailer details
- **get_warehouse_count**: Get warehouse stock counts
- **list_inventory**: List inventory quantities
- **list_invoices**: List invoices
- **list_orders**: List Nabis wholesale orders
- **list_retailers**: List retailers
- **list_warehouses**: List warehouses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nabis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pending Nabis orders."

**🤖 AI Agent:**
> Fetching orders... I've found 8 pending orders. Here are the most recent ones...

---

**👤 You:**
> "What is the stock level for product 'Blue Dream' in the LA warehouse?"

**🤖 AI Agent:**
> Checking inventory... 'Blue Dream' currently has 150 units available in the Los Angeles warehouse.


## ❓ FAQ

**Q: How do I get a Nabis Access Token?**
Log in to the Nabis Platform, navigate to the Developer settings, and generate a new V2 Access Token.

**Q: Which markets are supported?**
The API supports all active Nabis markets, including California and New York.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nabis](https://vinkius.com/mcp/nabis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nabis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nabis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nabis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nabis": {
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
