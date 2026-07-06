# MOBIDI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mobidi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage your mobile advertising campaigns with real-time bidding, audience targeting, and performance analytics for app installs.

## Description
Connect your **MOBIDI** platform to any AI agent and manage business intelligence data.

### What you can do

- **Data Queries** — Run custom queries and count matching records
- **CRUD Operations** — Create, read, update, and delete records of any entity type
- **Reports** — List, inspect, and execute BI reports
- **Data Model** — Explore available entity types
- **System Services** — View available platform services


## Available Tools (12)
- **delete_record**: Delete a record
- **execute_report**: Execute a report
- **get_record_by_id**: Get record by ID
- **get_record_count**: Count records
- **get_report**: Get report details
- **get_services**: List system services
- **list_entity_types**: List entity types
- **list_records**: Query records
- **list_reports**: List reports
- **update_record**: Update a record
- **check_mobidi_status**: Verify API connectivity
- **create_record**: Create a record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MOBIDI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Query all records where status is active."

**🤖 AI Agent:**
> Found 1,234 active records. Top entity types: Customer (456), Order (389), Product (234), Invoice (155).

---

**👤 You:**
> "Execute the monthly sales report."

**🤖 AI Agent:**
> Monthly Sales Report: Total revenue ,567. Top products: Widget A (), Widget B (). Growth: +12% vs last month.

---

**👤 You:**
> "List all entity types in the data model."

**🤖 AI Agent:**
> 12 entity types: Customer, Order, Product, Invoice, Supplier, Employee, Project, Task, Report, Category, Department, Location.


## ❓ FAQ

**Q: Can my AI run custom queries?**
Yes. `list_records` accepts a query object to filter and retrieve specific records from the database.

**Q: Can I create and update data?**
Yes. `create_record`, `update_record`, and `delete_record` provide full CRUD operations on any entity type.

**Q: Can I run BI reports?**
Yes. `execute_report` runs any configured report and returns the results. Use `list_reports` to see what is available.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mobidi](https://vinkius.com/mcp/mobidi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MOBIDI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mobidi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MOBIDI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mobidi": {
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
