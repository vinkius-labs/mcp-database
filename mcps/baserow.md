# Baserow MCP Server

Manage no-code databases via Baserow — list tables, query rows, create records and manage schemas from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/baserow)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **Baserow** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baserow](https://vinkius.com/mcp/baserow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
