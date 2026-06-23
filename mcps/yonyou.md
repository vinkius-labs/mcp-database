# Yonyou / 用友 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yonyou)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Leading enterprise ERP and cloud services platform in China — manage purchase orders, sales, and inventory via AI.

## Description
Empower your AI agent to orchestrate your entire enterprise operations with **Yonyou** (用友), the dominant ERP and cloud services provider in China. By connecting Yonyou to your agent, you transform complex business management, supply chain tracking, and financial auditing into a natural conversation. Your agent can instantly list purchase and sales orders, retrieve detailed material metadata, monitor inventory levels, and even browse financial vouchers without you ever needing to navigate the comprehensive YonBIP interface. Whether you are conducting a procurement audit or monitoring sales performance across multiple regions, your agent acts as a real-time operations assistant, keeping your ERP data accurate and your business moving.

### What you can do

- **Supply Chain Orchestration** — List and retrieve detailed information about purchase and sales orders.
- **Master Data Control** — Browse materials, customers, and suppliers to identify key business entities.
- **Inventory Monitoring** — Query real-time inventory levels for items across different warehouses.
- **Financial Auditing** — Browse accounting vouchers and retrieve high-level organizational metadata.
- **Operational Insights** — Retrieve high-level summaries of organization-wide business activity and performance.

### How it works

1. Subscribe to this server
2. Enter your Yonyou App Key, App Secret, and Tenant ID
3. Start managing your enterprise operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — monitor supply chain progress and audit order fulfillment through natural language queries.
- **Procurement Teams** — coordinate with suppliers and monitor material availability directly from your AI-powered workspace.
- **Finance Leads** — oversee financial vouchers and audit organizational structures via a unified AI interface.
- **Yonyou Power Users** — integrate your existing ERP workflows into your AI-driven daily routines.


## Available Tools (10)
- **get_inventory**: Query ERP inventory
- **get_org_info**: Get organization metadata
- **get_purchase_order**: Get purchase order details
- **get_sales_order**: Get sales order details
- **list_customers**: List ERP customers
- **list_materials**: List master data materials
- **list_purchase_orders**: List ERP purchase orders
- **list_sales_orders**: List ERP sales orders
- **list_suppliers**: List ERP suppliers
- **list_vouchers**: List financial vouchers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yonyou / 用友** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 purchase orders in Yonyou."

**🤖 AI Agent:**
> I've retrieved your recent purchase orders. They include transactions for 'Steel Sheets' and 'Industrial Connectors'. Total value for these orders is ¥450,000. Would you like to check the fulfillment status?

---

**👤 You:**
> "What is the current inventory for material ID 'MAT-8821'?"

**🤖 AI Agent:**
> The current inventory for MAT-8821 is 1,200 units. There are 800 units in the 'East Warehouse' and 400 in the 'West Logistics Center'. Would you like me to notify you if stock falls below 500 units?

---

**👤 You:**
> "Show me the organization structure defined in our ERP."

**🤖 AI Agent:**
> I've retrieved the organizational metadata. Your ERP environment is structured into 3 main branches: 'Headquarters', 'Manufacturing Division', and 'Global Sales'. Would you like a detailed breakdown of the legal entities under each branch?


## ❓ FAQ

**Q: How do I find my Yonyou Tenant ID?**
Log in to your Yonyou YonBIP administration backend, go to [Digital Modeling] → [My Enterprise] → [Enterprise Information], and you will find your Tenant ID there.

**Q: Can I query inventory levels through this server?**
Yes. Use the `get_inventory` tool to retrieve real-time stock information. You can filter by material ID or warehouse to get precise availability data.

**Q: Is it possible to list financial vouchers?**
Yes! Use the `list_vouchers` tool to retrieve a history of accounting vouchers, allowing your agent to audit financial movements across the organization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yonyou](https://vinkius.com/mcp/yonyou)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Yonyou / 用友** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `yonyou` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Yonyou / 用友** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "yonyou": {
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
