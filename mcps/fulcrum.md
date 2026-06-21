# Fulcrum MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fulcrum)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fulcrum-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fulcrum-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage field data collection, track form records, and query datasets via AI agents with Fulcrum.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fulcrum** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active forms/apps in my Fulcrum account."

**🤖 AI Agent:**
> Retrieving forms... I found 4 active forms, including 'Site Inspection' (ID: form_123) and 'Asset Inventory' (ID: form_456).

---

**👤 You:**
> "Run a SQL query to get the last 5 records from form 'form_123'."

**🤖 AI Agent:**
> Executing query... I've retrieved the 5 most recent records from the 'Site Inspection' form. Would you like to see the specific data values for these entries?

---

**👤 You:**
> "Show me the field schema for the 'Asset Inventory' form (ID: form_456)."

**🤖 AI Agent:**
> Fetching schema... The form contains 12 fields. Key fields include 'Asset Tag' (Type: Text, Required: Yes) and 'Condition' (Type: Choice).


## Installation & Usage

To install and use the **Fulcrum** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fulcrum](https://vinkius.com/mcp/fulcrum)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
