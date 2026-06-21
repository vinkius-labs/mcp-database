# Dynamics 365 Finance & Operations MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dynamics-365-finance-operations)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI agent to manage enterprise resources, track sales orders, and monitor financial journals via the D365 F&O API.

## Description
Integrate **Microsoft Dynamics 365 Finance & Operations**, the comprehensive ERP platform, directly into your AI workflow. Manage your enterprise supply chain, track sales orders and customers, monitor financial journals and ledger activity, and oversee real-time inventory on-hand using natural language.

### What you can do

- **ERP Oversight** — List and retrieve detailed information and status for all your sales orders, vendors, and customers.
- **Financial Intelligence** — Monitor ledger journals, posting statuses, and organizational financial metadata across your legal entities.
- **Inventory Management** — Access real-time inventory on-hand quantities across all warehouses and released products.
- **Enterprise Auditing** — Retrieve high-level summaries of sales activity, stock levels, and organizational environment metadata instantly.

### How it works

1. Connect the D365 F&O integration to your AI assistant.
2. Authorize using your Azure AD Client ID, Client Secret, Tenant ID, and environment URL.
3. Orchestrate your enterprise resource planning and financial analysis through intuitive conversation.

### Who is this for?

- **Finance Managers** — Quickly check ledger statuses and daily sales order volumes on the go.
- **Supply Chain Leads** — Monitor inventory levels and vendor activity across multiple warehouses via chat.
- **Operations Teams** — Research specific order details and organizational ERP metadata instantly.


## Available Tools (10)
- **get_d365_fo_metadata**: Retrieve metadata for the current authenticated environment
- **get_inventory_on_hand**: Retrieve real-time inventory on-hand quantities across all warehouses
- **quick_finance_health_audit**: Retrieve a high-level summary of recent orders and inventory (mock logic)
- **get_sales_order_details**: Get detailed information for a specific sales order
- **list_d365_customers**: List all customers registered in your enterprise account
- **list_ledger_journals**: List ledger journals and their headers
- **list_released_products**: List all released products in your enterprise catalog
- **list_d365_sales_orders**: List all sales order headers in your D365 F&O environment
- **list_d365_vendors**: List all vendors in your Dynamics 365 Finance & Operations account
- **search_sales_orders**: Search for sales orders using an order number or customer keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dynamics 365 Finance & Operations** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all sales orders for customer 'C0001'."

**🤖 AI Agent:**
> I've found 12 sales orders for customer 'C0001', including 'SO-101' (Open) and 'SO-105' (Invoiced). Would you like to see the line items for the most recent open order?

---

**👤 You:**
> "Show me the current inventory on-hand for product 'P001'."

**🤖 AI Agent:**
> Product 'P001' (High-Speed Hub) has 45 units on-hand across all warehouses. 30 units are in 'Warehouse East' and 15 in 'Warehouse West'. Should I check for any pending arrivals for this product?

---

**👤 You:**
> "Search for sales orders with 'Pending' status."

**🤖 AI Agent:**
> I've retrieved 8 sales orders with a 'Pending' or 'Backordered' status. High-priority orders include 'SO-9988' for 'Tech Corp' and 'SO-7766' for 'Global Logistics'. Would you like the detailed status for SO-9988?


## ❓ FAQ

**Q: How do I get D365 F&O API credentials?**
You must register an application in the **Azure Portal (App registrations)**, obtain a Client ID, Secret, and Tenant ID, and then register that Client ID in the **Microsoft Dynamics 365 Finance** instance under **System administration > Microsoft Entra ID applications**.

**Q: Can the agent post ledger journals?**
This integration currently focuses on listing and auditing records via the OData API. Posting journals or triggering complex business logic should be managed via the D365 F&O client or specific custom service endpoints.

**Q: Does the integration support multiple legal entities?**
Yes, the agent can retrieve data from any legal entity exposed via your environment URL and authorized for your Azure AD application user.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dynamics-365-finance-operations](https://vinkius.com/mcp/dynamics-365-finance-operations)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dynamics 365 Finance & Operations** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dynamics-365-finance-operations` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dynamics 365 Finance & Operations** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dynamics-365-finance-operations": {
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
