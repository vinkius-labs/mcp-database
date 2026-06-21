# Oracle NetSuite MCP Server

Manage financials, sales orders, inventory, and customer records on Oracle NetSuite — the leading cloud ERP.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/oracle-netsuite)

## Overview
**Category:** industry-titans
**Tools Count:** 9

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


## Installation & Usage

To install and use the **Oracle NetSuite** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oracle-netsuite](https://vinkius.com/mcp/oracle-netsuite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
