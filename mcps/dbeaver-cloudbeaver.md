# DBeaver (CloudBeaver) MCP Server

Manage database connections, users, and server configurations via CloudBeaver's API — inspect drivers, manage teams, and query server status directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dbeaver-cloudbeaver)

## Overview
**Category:** developer-tools
**Tools Count:** 19

## Description
Connect your **CloudBeaver** (DBeaver Cloud) instance to any AI agent to streamline database administration and server management through natural language.

### What you can do

- **User & Team Management** — Create, delete, and inspect user accounts and teams for granular access control using `create_user` and `create_team`.
- **Connection Insights** — Fetch detailed configuration and status for specific database connections across projects with `get_connection_info`.
- **Driver & Export Discovery** — List supported database drivers and available data transfer formats (CSV, JSON, XLSX) via `get_driver_list` and `data_transfer_available_stream_processors`.
- **Server Health & Licensing** — Monitor active product licenses, server settings, and AI assistant configurations with `get_active_product_license` and `get_ai_settings`.
- **Authentication Control** — Query available auth providers and manage session logins via `get_auth_providers` and `auth_login`.

### How it works

1. Subscribe to this server
2. Provide your CloudBeaver Server URL and API Token
3. Start managing your database infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **Database Administrators** — quickly audit user permissions and connection statuses without the web UI
- **DevOps Engineers** — automate user provisioning and verify server configurations
- **Data Engineers** — check available drivers and export capabilities for data pipelines


## Available Tools
- **add_connections_access**: Grants users or teams access to specific connections
- **auth_login**: Authenticates a session using a provider and credentials
- **configure_server**: Updates the main server configuration
- **create_team**: Creates a new team for access management
- **create_user**: Creates a new user account (Admin only)
- **data_transfer_available_stream_processors**: Lists available export formats (CSV, JSON, XLSX, etc.)
- **data_transfer_export_data_from_container**: Starts an async task to export data from a table/schema
- **data_transfer_export_data_from_results**: Exports data from a specific SQL query result set
- **db_sm_terminate**: Terminates active database sessions for a connection
- **delete_team**: Removes a team
- **delete_user**: Removes a user account
- **get_active_product_license**: Returns details of the active server license
- **get_active_user**: Returns information about the currently authorized user
- **get_admin_user_info**: Returns detailed admin-level info for a specific user
- **get_ai_settings**: Returns global AI assistant configurations
- **get_all_product_licenses**: Lists all licenses installed on the server
- **get_auth_providers**: Lists all available authentication providers (local, SAML, etc.)
- **get_connection_info**: Returns configuration and status for a specific database connection
- **get_driver_list**: Lists all database drivers supported by the server


## Installation & Usage

To install and use the **DBeaver (CloudBeaver)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dbeaver-cloudbeaver](https://vinkius.com/mcp/dbeaver-cloudbeaver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
