# Kizeo Forms MCP Server

Manage mobile forms, data submissions, and users via the Kizeo Forms API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kizeo-forms)

## Overview
**Category:** productivity
**Tools Count:** 9

## Description
Connect your **Kizeo Forms** account to any AI agent to automate your field data collection and operational workflows. This MCP server enables your agent to interact with mobile forms, manage data submissions, and query user permissions directly from natural language interfaces.

### What you can do

- **Form Oversight** — List all available mobile forms and retrieve their hierarchical structures and field definitions
- **Data Management** — Retrieve specific form entries and perform advanced searches using custom field filters
- **Push Operations** — Pre-fill and push new data entries into forms to streamline field work assignments
- **User Administration** — Manage account users, update profiles, and control permissions across your organization
- **Operational Auditing** — Read unread data submissions and monitor field activity in real-time

### How it works

1. Subscribe to this server
2. Enter your Kizeo Forms Authorization Token
3. Start managing your mobile forms from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — Monitor field data submissions and assign tasks via natural language commands
- **Field Supervisors** — Quickly query form definitions and entry data without opening the web interface
- **Developers** — Integrate mobile form logic and data pushing into your custom operational tools


## Available Tools
- **search_form_data**: Search form data with advanced filters
- **create_new_user**: Requires name, email, and password.

Add a new user to the account
- **delete_account_user**: Remove a user from the account
- **list_all_forms**: List all available forms
- **get_form_entry_data**: Get data for a specific form submission
- **get_form_definition**: Get the definition of a specific form
- **push_data_to_form**: Requires a JSON body with field values.

Push a new data entry into a form
- **update_existing_user**: Update details for an existing user
- **list_account_users**: List all users in the account


## Installation & Usage

To install and use the **Kizeo Forms** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kizeo-forms](https://vinkius.com/mcp/kizeo-forms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
