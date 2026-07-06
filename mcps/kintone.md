# Kintone MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kintone)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage custom business apps, records, and workflows via Kintone.

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


## Available Tools (10)
- **list_form_fields**: List form fields for an app
- **get_app_details**: Get details for a specific app
- **add_record**: Requires a JSON object mapping field codes to values.

Add a new record to an app
- **get_app_layout**: Get the field layout of an app
- **list_apps**: Use this to identify App IDs for record operations.

List all Kintone apps
- **delete_records**: Requires an array of record IDs.

Delete records from an app
- **get_record**: Get a specific record from an app
- **list_records**: You can optionally provide a query string for filtering.

List records from an app
- **list_space_members**: List members of a Kintone space
- **update_record**: Update an existing record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kintone** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Kintone apps."

**🤖 AI Agent:**
> I've retrieved your apps. You have 5 applications, including 'Sales Pipeline' (ID: 10), 'Employee Directory' (ID: 12), and 'Project Tracker' (ID: 15).

---

**👤 You:**
> "Show records from app ID 10 where status is 'Pending'."

**🤖 AI Agent:**
> I found 3 records in app 10 with 'Pending' status: 'Opportunity A', 'Opportunity B', and 'Opportunity C'. Would you like to see details for any of them?

---

**👤 You:**
> "Add a new record to app 12 with name 'Jane Doe' and role 'Designer'."

**🤖 AI Agent:**
> Successfully added the record for 'Jane Doe' to app 12. The new record ID is '105'.


## ❓ FAQ

**Q: How do I find the App ID for a specific application?**
Use the `list_apps` tool to see a comprehensive list of all applications in your environment along with their unique App IDs.

**Q: Can I filter records using custom criteria?**
Yes, the `list_records` tool accepts an optional Kintone query string, allowing you to filter data based on field values, status, and more.

**Q: Is it possible to update an existing record via the agent?**
Absolutely. Use the `update_record` tool with the App ID and Record ID, providing a JSON object with the fields you wish to modify.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kintone](https://vinkius.com/mcp/kintone)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kintone** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kintone` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kintone** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kintone": {
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
