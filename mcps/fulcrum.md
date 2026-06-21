# Fulcrum MCP Server

Manage field data collection, track form records, and query datasets via AI agents with Fulcrum.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fulcrum)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Fulcrum** environment to any AI agent to automate your field data collection and mobile inspection workflows through the Model Context Protocol (MCP). Fulcrum is a no-code mobile data collection platform used to build custom apps for field inspections, surveys, and inventory management. This MCP server enables you to retrieve dynamic form schemas, list collected records, and query massive datasets directly through natural conversation.

### Key Features

- **Form Discovery** — List all data collection apps (forms) and fetch detailed schemas including field definitions and validation logic.
- **Record Management** — Access and retrieve collected field data, or create new records programmatically to keep your database updated.
- **Data Querying** — Execute powerful SQL queries against the Fulcrum Query API to instantly retrieve and filter large datasets.
- **Team Oversight** — List all organization members and system roles to manage user access and field workforce deployment.
- **Webhook Integration** — Monitor configured webhooks to ensure your downstream systems are receiving real-time data syncs.
- **Real-time Synchronization** — Keep your field intelligence accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Fulcrum API Token (found in your Settings)
3. Start managing your field data collection from Claude, Cursor, or any MCP client

### Who is this for?

- **GIS & Field Operations Managers** — quickly check collected records or query survey datasets without manual exports.
- **Data Analysts** — use natural language to prompt SQL queries against field data for instant reporting.
- **System Administrators** — automate the retrieval of form schemas and member lists while auditing workforce permissions.


## Available Tools
- **create_record**: Create data record
- **check_api_status**: Verify API connection
- **get_form_schema**: Get form schema
- **get_record_details**: Get record metadata
- **list_data_forms**: List apps/forms
- **list_organization_members**: List team members
- **list_field_records**: Can be filtered by form ID.

List field data records
- **list_member_roles**: g. Owner, Manager, Standard).

List roles
- **list_webhooks**: List webhook configs
- **query_records_sql**: Query data with SQL


## Installation & Usage

To install and use the **Fulcrum** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fulcrum](https://vinkius.com/mcp/fulcrum)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
