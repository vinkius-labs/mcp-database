# Jestor MCP Server

Manage data, workflows, and records via Jestor low-code API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/jestor)

## Overview
**Category:** business-operations
**Tools Count:** 10

## Description
Empower your AI agents with Jestor's low-code internal tools platform. This MCP server allows you to list objects (tables), retrieve and list records, manage users, and monitor workflows and dashboards directly through the Jestor API. Ideal for automating internal operations and database management.


## Available Tools
- **get_me**: Use this to verify connection status and current permissions.

Gets current authenticated user info
- **get_object**: Useful for understanding field types and relationships within a specific table.

Retrieves details/schema for a specific object
- **get_record**: Essential for deep-diving into a specific entry in the database.

Retrieves details for a specific record
- **list_apps**: Useful for discovering high-level toolsets available to the user.

Lists all installed internal apps
- **list_dashboards**: Use this to identify where aggregated data visualizations are located.

Lists all configured dashboards
- **list_objects**: Returns object names and labels. Use this to discover available datasets before querying specific records.

Lists all objects (tables) in your Jestor account
- **list_records**: This is the primary tool for browsing data within a table (e.g., listing all "Tasks" or "Clients").

Lists records for a specific object
- **list_users**: Returns names, emails, and IDs. Useful for identifying record owners or system administrators.

Lists all users in the organization
- **list_webhooks**: Use this to audit third-party integrations.

Lists all configured webhooks
- **list_workflows**: Useful for auditing system logic and event-driven actions.

Lists all automated workflows


## Installation & Usage

To install and use the **Jestor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jestor](https://vinkius.com/mcp/jestor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
