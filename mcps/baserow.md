# Baserow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/baserow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage no-code databases via Baserow — list tables, query rows, create records and manage schemas from any AI agent.

## Description
Connect your **Baserow** databases to any AI agent and take full control of your data through natural conversation.

### What you can do

- **Database Discovery** — List all databases and tables the token has access to with their schemas
- **Schema Exploration** — Browse table fields (columns) with their types (text, number, boolean, date, select, etc.)
- **Row Operations** — List, create, update and delete rows with full CRUD support
- **Filtered Queries** — Query rows with pagination, ordering and field-based filtering
- **View Management** — List configured views (grid, gallery, kanban, form, calendar) with their filter and sort rules

### How it works

1. Subscribe to this server
2. Enter your Baserow Database Token
3. Start managing your data from Claude, Cursor, or any MCP-compatible client

No more clicking through the Baserow UI to find a record or update a field value. Your AI acts as a dedicated database administrator.

### Who is this for?

- **Product Teams** — quickly query project tracking databases, update task statuses and review sprint data
- **Developers** — discover table schemas, create records programmatically and manage database content via conversation
- **Data Analysts** — explore data schemas, run filtered queries and export row data for analysis


## Available Tools (10)
- **create_row**: Requires the table ID and a JSON object with field_name: value pairs matching the table schema. Use list_fields to discover available field names. Returns the created row with its ID and all field values.

Create a new row in a Baserow table
- **delete_row**: Provide the table ID and row ID. WARNING: this action is irreversible.

Delete a row from a Baserow table
- **get_row**: Field names are returned in user-readable format. Provide the table ID and row ID.

Get a specific row from a Baserow table
- **get_table**: Provide the table ID from list_tables.

Get details for a specific Baserow table
- **list_databases**: Each database shows its ID, name, workspace and creation date. Use this to discover available databases before querying their tables.

List all Baserow databases
- **list_fields**: Each field shows its ID, name, type (text, number, boolean, date, single_select, long_text, link_row, file, etc.), order and required status. Use this to understand the data schema before querying or creating rows.

List fields (columns) of a Baserow table
- **list_rows**: Optionally filter by field values (using user_field_names) and set page/size for pagination. Results include count, next/previous page URLs and the rows array. Use field names (not IDs) for readable results.

List rows in a Baserow table
- **list_tables**: Each table shows its ID, name, database, field count and creation date. Use this to discover the data schema before querying rows.

List all tables accessible in Baserow
- **list_views**: Each view shows its ID, name, type, filter settings and sort rules. Useful for understanding how data is organized and filtered in the UI.

List views configured for a Baserow table
- **update_row**: Requires the table ID, row ID and a JSON object with field_name: value pairs for the fields to update. Only provided fields will be modified. Use list_fields to discover available field names.

Update an existing row in a Baserow table


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Baserow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all tables in my Baserow workspace."

**🤖 AI Agent:**
> I found 5 tables: 'Projects' (42 rows, 12 fields), 'Tasks' (156 rows, 10 fields), 'Team Members' (8 rows, 7 fields), 'Sprints' (24 rows, 6 fields) and 'Bug Reports' (89 rows, 9 fields).

---

**👤 You:**
> "Show me all rows in the Tasks table where Status is 'In Progress'."

**🤖 AI Agent:**
> I found 12 tasks with 'In Progress' status. The highest priority items are 'Implement OAuth integration' (assigned to Alice, due Friday), 'Fix checkout payment bug' (assigned to Bob, due today) and 'Design new dashboard layout' (assigned to Carol, due next week).

---

**👤 You:**
> "Create a new task called 'Review PR #234' assigned to Alice with status 'To Do'."

**🤖 AI Agent:**
> Done! I've created a new row in the Tasks table with title 'Review PR #234', assigned to Alice, status 'To Do'. The row ID is 157 and it was created just now.


## ❓ FAQ

**Q: How do I get a Baserow API Token?**
Log in to your Baserow workspace, go to **Database Settings > API Tokens** (or Workspace Settings > API Tokens), click **Create Token**, give it a name and set the permissions (create, read, update, delete) for specific tables. Copy the token immediately — it won't be shown again.

**Q: Can I create and update rows programmatically?**
Yes! Use `create_row` with the table ID and a JSON object of field_name: value pairs. Use `update_row` with the table ID, row ID and the fields to update. First use `list_fields` to discover the available field names and their types for the table.

**Q: Can I filter rows by field values?**
Yes! The `list_rows` tool supports pagination and ordering. Use the `page` and `size` parameters for pagination, and `order_by` to sort by any field (prefix with `-` for descending). The underlying API also supports field-level filtering through the filter parameter.

**Q: What field types does Baserow support?**
Baserow supports: text, number, boolean, date, long_text, email, url, single_select, multiple_select, link_row (relationships), file, rating, formula, lookup, rollup, last_modified and created_on fields. Use `list_fields` to see the exact types in your table.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baserow](https://vinkius.com/mcp/baserow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Baserow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `baserow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Baserow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "baserow": {
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
