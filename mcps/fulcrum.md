# Fulcrum MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fulcrum)
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


## ❓ FAQ

**Q: How do I get an API Token for Fulcrum?**
Log in to your Fulcrum web app, click the Settings (gear icon), select 'API', and you can generate a new API Token.

**Q: Can I run SQL queries on my field data?**
Yes! Use the 'query_records_sql' tool. Provide a standard SQL statement (e.g., SELECT * FROM "form_id") to instantly retrieve filtered datasets.

**Q: Is it possible to see the schema of a form?**
Absolutely. The 'get_form_schema' tool retrieves the complete JSON definition of a form, including all its field keys, data types, and validation rules.

**Q: Can I programmatically create a new record?**
Yes, you can use the 'create_record' tool. You will need the Form ID, latitude, longitude, and a JSON payload containing the specific form values.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fulcrum](https://vinkius.com/mcp/fulcrum)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fulcrum** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fulcrum` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fulcrum** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fulcrum": {
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
