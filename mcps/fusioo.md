# Fusioo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fusioo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage collaborative workspaces, track records, and oversee custom apps via AI agents with Fusioo.

## Description
Connect your **Fusioo** workspace to any AI agent to automate your project management and database workflows through the Model Context Protocol (MCP). Fusioo is a highly customizable workspace platform that allows you to build your own apps to manage everything from CRM to project tracking. This MCP server enables you to retrieve app schemas, manage individual records, and monitor workspace activity directly through natural conversation.

### Key Features

- **Custom App Oversight** — List all apps in your workspace and fetch detailed schemas including field definitions and unique IDs.
- **Record Management** — Access and retrieve data from any of your custom apps, or create and update records programmatically.
- **Data Quantification** — Get real-time record counts for specific apps to track project volume or lead growth.
- **Teammate Collaboration** — List workspace users and teammates to maintain full context of who is involved in each app.
- **Dashboard Insights** — Access configured widgets and saved reports to get high-level snapshots of your data.
- **User Identity** — Fetch profile information for the authenticated API identity to verify access levels.
- **Real-time Synchronization** — Keep your custom database records accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Fusioo Client ID and Client Secret (found in Integrations > Custom Integrations)
3. Start managing your custom apps from Claude, Cursor, or any MCP client

### Who is this for?

- **Project Managers** — quickly check project statuses or record counts without manual dashboard navigation.
- **CRM Admins** — get a real-time overview of leads and customer profiles via simple AI commands.
- **Operations Teams** — automate the creation of new records and verify field schemas seamlessly.


## Available Tools (12)
- **create_app_record**: Add a new record
- **get_app_schema**: Get app metadata
- **get_my_identity**: Get current user
- **get_app_record_count**: Get total record count
- **get_record_details**: Get record metadata
- **list_apps**: List all Fusioo apps
- **list_app_records**: List records in app
- **list_workspace_reports**: List available reports
- **list_workspace_users**: List teammates
- **list_dashboard_widgets**: List widgets
- **update_app_record**: Modify a record
- **verify_api_connection**: Check connection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fusioo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the custom apps in my Fusioo workspace."

**🤖 AI Agent:**
> Retrieving apps... I found 4 custom apps: 'Projects' (ID: app_123), 'Clients' (ID: app_456), 'Tasks', and 'Inventory'. Which one would you like to explore?

---

**👤 You:**
> "Get the last 5 records from the 'Projects' app (ID: app_123)."

**🤖 AI Agent:**
> Fetching records... For 'Projects', I found 5 recent entries, including 'Q4 Marketing Campaign' (Status: In Progress) and 'Server Migration' (Status: Completed).

---

**👤 You:**
> "How many records are currently in my 'Leads' app (ID: app_789)?"

**🤖 AI Agent:**
> Calculating records... There are currently 156 records in your 'Leads' app. Would you like to see the most recent ones?


## ❓ FAQ

**Q: How do I get a Client ID and Secret for Fusioo?**
Log in to your Fusioo workspace, navigate to Integrations > Custom Integrations, and create a new integration to retrieve your Client ID and Client Secret.

**Q: Where do I find my App ID or Record ID?**
Open any record in your Fusioo app, click the options menu (three dots), and select 'Developer Information' to see the IDs for the App, Record, and Fields.

**Q: Can I filter records through the agent?**
The 'list_app_records' tool retrieves the most recent records. For advanced filtering, ensure you have the correct App ID or use the 'get_record_details' if you have the specific ID.

**Q: What is the difference between an App and a Record?**
In Fusioo, an App is a collection or database table (e.g., 'Projects'), while a Record is a specific entry in that collection (e.g., 'Website Launch').


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fusioo](https://vinkius.com/mcp/fusioo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fusioo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fusioo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fusioo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fusioo": {
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
