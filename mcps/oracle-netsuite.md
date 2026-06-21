# Oracle NetSuite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/oracle-netsuite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage financials, sales orders, inventory, and customer records on Oracle NetSuite — the leading cloud ERP.

## Description
Connect your **Oracle NetSuite** account to any AI agent and manage your unified ERP operations through natural conversation.

### What you can do

- **Financial Management** — Query G/L account balances, post journal entries, and retrieve trial balance reports across subsidiaries
- **Sales Orders** — Create and manage sales orders, check fulfillment status, and view invoice history
- **Purchase Orders** — Create POs, track receipt status, and manage vendor bill matching
- **Inventory & Items** — Query item records, stock levels by location, and inventory valuations
- **Customer Records** — Create, read, and update customer master data including contacts and credit limits
- **Saved Searches** — Execute NetSuite saved searches to retrieve complex, pre-filtered datasets
- **SuiteQL Queries** — Run advanced SQL-like queries against any NetSuite record type using SuiteQL

### How it works

1. Subscribe to this server
2. Enter your NetSuite TBA credentials (Account ID, Consumer Key, Consumer Secret, Token ID, Token Secret)
3. Start managing your ERP through Claude, Cursor, or any MCP-compatible client

37,000+ organizations across 219 countries run on NetSuite. Now your AI agent runs on it too.

### Who is this for?

- **Controllers & CFOs** — query real-time financial data and run saved searches without opening NetSuite
- **Order Management Teams** — create sales orders and track fulfillment through simple chat commands
- **Procurement Teams** — manage POs and vendor data through conversation
- **NetSuite Administrators** — execute SuiteQL queries and audit record configurations rapidly


## Available Tools
- **execute_suiteql**: SuiteQL supports SELECT, JOIN, WHERE, GROUP BY, ORDER BY, and aggregate functions. Example: SELECT id, companyname FROM customer WHERE isinactive = 'F' ORDER BY companyname

Execute a SuiteQL query
- **get_record**: Common types: customer, vendor, salesOrder, purchaseOrder, invoice, employee, item, inventoryItem.

Get a specific NetSuite record
- **create_record**: Provide the record type and a JSON body with field values. Example record types: customer, salesOrder, purchaseOrder, journalEntry.

Create a new NetSuite record
- **update_record**: Only specify the fields you want to change.

Update an existing NetSuite record
- **delete_record**: This action is irreversible.

Delete a NetSuite record
- **list_records**: Common types: customer, vendor, employee, salesOrder, purchaseOrder, invoice, inventoryItem.

List NetSuite records by type
- **list_customers**: List NetSuite customers
- **list_sales_orders**: List recent sales orders
- **get_record_metadata**: Useful for understanding what fields are available before creating or updating records.

Get metadata for a NetSuite record type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Oracle NetSuite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the revenue breakdown by subsidiary for March 2026."

**🤖 AI Agent:**
> Revenue by Subsidiary (March 2026): 1. US Operations — $2,340,000 (+12% MoM), 2. EU Operations — €1,150,000 (+8% MoM), 3. APAC — ¥89,500,000 (+15% MoM). Total consolidated revenue: $4,120,000. Want me to drill down into any subsidiary?

---

**👤 You:**
> "Find all customers with overdue invoices above $10,000."

**🤖 AI Agent:**
> Found 12 customers with overdue invoices > $10K: 1. GlobalTech Inc — $45,200 (32 days overdue), 2. Pinnacle Corp — $28,750 (18 days overdue), 3. Summit Holdings — $22,100 (45 days overdue)... Total overdue amount: $312,400. Want me to generate a collections follow-up list?

---

**👤 You:**
> "Create a sales order for customer 'CUST-1045' with 100 units of item 'SKU-2024-A' at $45 each."

**🤖 AI Agent:**
> Sales Order SO-2026-04567 created successfully! Customer: CUST-1045, Item: SKU-2024-A, Qty: 100, Unit Price: $45.00, Total: $4,500.00. Status: Pending Fulfillment. Would you like me to check stock availability or generate the pick ticket?


## ❓ FAQ

**Q: What credentials do I need for NetSuite authentication?**
You need 5 values for Token-Based Authentication (TBA): Account ID, Consumer Key, Consumer Secret, Token ID, and Token Secret. All are generated within your NetSuite account under Setup > Integration.

**Q: Can I run custom SuiteQL queries?**
Yes. The `execute_suiteql` tool executes SQL-like queries against the SuiteQL endpoint. You can query any record type, join tables, and use aggregation functions — all through natural language that the agent translates to SuiteQL.

**Q: Does it support NetSuite saved searches?**
Absolutely. Use the `run_saved_search` tool with the saved search ID to retrieve its results. This works with any existing saved search in your account — transactions, customers, items, or custom records.

**Q: Can I create sales orders through the agent?**
Yes. The `create_record` tool with the `salesOrder` record type lets you create full sales orders with line items, pricing, shipping addresses, and payment terms — all through conversation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oracle-netsuite](https://vinkius.com/mcp/oracle-netsuite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Oracle NetSuite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `oracle-netsuite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Oracle NetSuite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oracle-netsuite": {
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
