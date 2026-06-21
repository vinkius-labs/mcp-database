# Retable MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/retable)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize data in smart spreadsheets with relational views, team collaboration, and workflow automation that goes beyond basic tables.

## Description
Connect your **Retable** account to any AI agent and manage your spreadsheet data through natural conversation.

### What you can do

- **Project Management** — List and inspect projects
- **Table Access** — Browse tables and view schemas
- **Record Operations** — List, get, create, update, and delete records
- **Health Check** — Verify API connectivity


## Available Tools
- **check_retable_status**: Verify API connectivity
- **create_record**: Create a new record
- **delete_record**: Delete a record
- **get_project**: Get project details
- **get_record**: Get record details
- **get_table**: Get table details
- **list_projects**: List all projects
- **list_records**: List records in a table
- **list_tables**: List tables in a project
- **update_record**: Update a record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Retable** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Retable projects."

**🤖 AI Agent:**
> You have 3 projects: 'CRM Pipeline' (4 tables), 'Inventory' (2 tables), 'HR Tracker' (3 tables).

---

**👤 You:**
> "Show all records in table tbl_001."

**🤖 AI Agent:**
> Table 'Leads' has 47 records. Top entries: 'Acme Corp' (Status: Qualified), 'TechCo' (Status: New), 'GlobalFin' (Status: Won).

---

**👤 You:**
> "Add a new record to table tbl_001 with name 'NewClient' and status 'New'."

**🤖 AI Agent:**
> Record created! ID: rec_8291 in table 'Leads'. Fields: name='NewClient', status='New'. Would you like to update any fields?


## ❓ FAQ

**Q: Can my AI create and update records in Retable?**
Yes. Use `create_record` to add new rows and `update_record` to modify existing ones. Both accept a JSON string with field values.

**Q: How do I query records from a specific table?**
Use `list_records` with the table ID. The agent returns all rows with their field values.

**Q: Can I delete records through the AI?**
Yes. The `delete_record` tool permanently removes a row from a table by table ID and record ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/retable](https://vinkius.com/mcp/retable)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Retable** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `retable` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Retable** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "retable": {
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
