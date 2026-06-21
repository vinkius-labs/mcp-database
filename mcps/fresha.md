# Fresha MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fresha)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Query and analyze your Fresha salon data — list appointments, clients, locations, services, staff, and sales transactions directly from any AI agent.

## Description
Connect your **Fresha** workspace to any AI agent and gain deep insights into your salon or spa operations through natural conversation using OData-powered queries.

### What you can do

- **Appointments & Bookings** — List scheduled appointments and detailed appointment services to track your calendar
- **Client Management** — Retrieve customer profiles, contact details, and saved history from your workspace
- **Sales & Financials** — Query sales transactions, invoices, and individual line items generated at checkout
- **Business Structure** — Inspect physical locations, service menus, and staff/professional profiles

### How it works

1. Subscribe to this server
2. Enter your Fresha Data Connector Token
3. Start querying your salon data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Salon & Spa Owners** — instantly analyze booking trends, check daily sales, and monitor staff schedules without manual exports
- **Operations Managers** — track client retention, service performance, and multi-location metrics through simple questions
- **Data Analysts** — run advanced OData filters and queries to build custom reports on appointments and revenue


## Available Tools (11)
- **list_appointment_services**: List Fresha appointment services via OData
- **list_appointments**: List Fresha appointments via OData
- **list_clients**: List Fresha clients via OData
- **list_inventory**: List Fresha inventory via OData
- **list_locations**: List Fresha locations via OData
- **list_products**: List Fresha products via OData
- **list_reviews**: List Fresha reviews via OData
- **list_sale_items**: List Fresha sale items via OData
- **list_sales**: List Fresha sales via OData
- **list_services**: List Fresha services via OData
- **list_staff**: List Fresha staff via OData


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fresha** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 completed appointments with client details."

**🤖 AI Agent:**
> I will query `list_appointments` with `$filter=Status eq 'Completed'`, `$orderby=StartTime desc`, `$top=5`, and `$expand=Client`. Here are the 5 most recent completed bookings, including appointments for Sarah M. (Haircut) and John D. (Massage).

---

**👤 You:**
> "Show me our physical business locations and active staff members."

**🤖 AI Agent:**
> Retrieving data... Using `list_locations` and `list_staff`, I found 2 active locations ('Downtown Salon' and 'Westside Spa') and 8 registered staff members. Would you like to see which staff members are assigned to a specific location?

---

**👤 You:**
> "Find all sales transactions from today."

**🤖 AI Agent:**
> Running the query on `list_sales` with a filter for today's date... I found 12 sales transactions totaling $1,450. The largest transaction was Invoice #1042 for $220. Would you like me to list the individual items for that invoice using `list_sale_items`?


## ❓ FAQ

**Q: Can I filter appointments by status or date using this server?**
Yes! The `list_appointments` tool supports standard OData `$filter` parameters. For example, you can pass `Status eq 'Completed'` or filter by start times to isolate specific booking periods.

**Q: How do I retrieve the specific services booked within an appointment?**
You can use the `list_appointment_services` tool, or use the `$expand` parameter in `list_appointments` to load related service details in a single query.

**Q: Can I view financial transactions and checkout details?**
Yes. Use the `list_sales` tool to query invoices and transactions, and the `list_sale_items` tool to inspect individual line items, products, or services sold during checkout.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fresha](https://vinkius.com/mcp/fresha)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fresha** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fresha` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fresha** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fresha": {
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
