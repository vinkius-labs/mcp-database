# Kintone MCP Server

Manage custom business apps, records, and workflows via Kintone.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kintone)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Kintone** platform to any AI agent to automate your business operations. This MCP server enables your agent to interact with custom apps, manage data records, and query organizational metadata directly.

### What you can do

- **Record Management** — List, retrieve, add, and update records in any of your Kintone apps
- **App Discovery** — List all available applications and retrieve detailed configurations and field mappings
- **Data Querying** — Use Kintone's powerful query language to filter records based on complex criteria
- **Form Inspection** — Access form field settings and layouts to understand data structures
- **Space Visibility** — List members and participants within your Kintone collaboration spaces

### How it works

1. Subscribe to this server
2. Enter your Kintone Subdomain and API Token
3. Start managing your business data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Teams** — Automate data entry and record updates via natural language commands
- **Project Managers** — Quickly query project statuses and task records from your IDE
- **Business Analysts** — Retrieve and analyze app data without manually exporting CSV files


## Available Tools
- **add_record**: Requires a JSON object mapping field codes to values.

Add a new record to an app
- **get_app_layout**: Get the field layout of an app
- **list_apps**: Use this to identify App IDs for record operations.

List all Kintone apps
- **delete_records**: Requires an array of record IDs.

Delete records from an app
- **list_form_fields**: List form fields for an app
- **get_app_details**: Get details for a specific app
- **get_record**: Get a specific record from an app
- **list_records**: You can optionally provide a query string for filtering.

List records from an app
- **list_space_members**: List members of a Kintone space
- **update_record**: Update an existing record


## Installation & Usage

To install and use the **Kintone** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kintone](https://vinkius.com/mcp/kintone)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
