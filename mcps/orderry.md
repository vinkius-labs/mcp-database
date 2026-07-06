# Orderry MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/orderry)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your repair shop, orders, and inventory with Orderry and AI agents.

## Description
### What you can do
- List and track repair orders and job tickets in real-time.
- Manage your CRM database, including individual clients and organizations.
- Monitor stock levels and inventory across multiple warehouses.
- Create new work orders and sales leads directly from your AI agent.

### How it works
1. Obtain your API Key from the Orderry dashboard under Settings > API.
2. Enter your credentials in Vinkius platform.
3. Start chatting with your Orderry agent to automate your service center operations.

### Who is it for?
- Repair shops and service center owners needing automated workflow control.
- Field service managers tracking jobs and technicians.
- Inventory managers syncing stock levels across retail and service locations.


## Available Tools (12)
- **create_order**: Create a new work order
- **create_client**: Add a new individual client
- **get_me**: Get account profile information
- **get_order_details**: Get details of a specific order
- **list_employees**: List staff members
- **list_leads**: List sales leads
- **list_orders**: List Orderry work orders
- **list_organizations**: List business clients (organizations)
- **list_clients**: List individual clients (people)
- **list_inventory_stock**: List products in stock
- **list_warehouses**: List facility warehouses
- **create_lead**: Record a new sales lead


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Orderry** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active work orders in Orderry."

**🤖 AI Agent:**
> I've found 5 active orders: 1. iPhone Screen Repair (ID: 101), 2. Oil Change (ID: 102), etc.

---

**👤 You:**
> "Show me all open work orders assigned to the repair team this week."

**🤖 AI Agent:**
> The repair team has 18 open work orders this week. 7 are iPhone screen replacements (average turnaround: 2 hours), 4 are laptop diagnostics, 3 are printer maintenance contracts, and 4 are custom device repairs. Total estimated revenue: $3,420. 3 orders are marked as urgent with same-day SLA commitments.

---

**👤 You:**
> "Create a new work order for a MacBook Pro battery replacement for customer ID cust_2847."

**🤖 AI Agent:**
> Work order #WO-5923 created successfully. Service: MacBook Pro Battery Replacement. Customer: James Wilson (cust_2847). Estimated cost: $189. Parts required: 1x A2141 battery module (in stock). Assigned to technician: David Park. Estimated completion: May 13th. Customer has been notified via email.


## ❓ FAQ

**Q: Can I check stock levels across warehouses?**
Yes, the list_inventory_stock tool provides real-time availability across all configured storage locations.

**Q: How do I create a new repair ticket?**
Use the create_order tool and provide a detailed description of the problem or task.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/orderry](https://vinkius.com/mcp/orderry)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Orderry** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `orderry` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Orderry** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "orderry": {
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
