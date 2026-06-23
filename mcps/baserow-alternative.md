# Baserow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/baserow-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Build no-code databases, create custom views, and collaborate on structured data with an open-source Airtable alternative.

## Description
Connect your **Baserow** account to any AI agent and take full control of your no-code relational databases and automated data management workflows through natural conversation.

### What you can do

- **Workspace & Database Orchestration** — List and monitor your entire Baserow ecosystem programmatically, from high-level workspaces to individual database applications
- **Schema Intelligence** — Access and manage tables and fields within your databases to maintain a perfectly coordinated high-fidelity data structure in real-time
- **Row Lifecycle Management** — Programmatically list, create, update, and delete rows in any table, retrieving detailed high-fidelity records using custom field names
- **Search & Discovery** — Use semantic keywords to search for specific records across your tables to maintain a perfectly coordinated digital ledger
- **Infrastructure Monitoring** — Retrieve metadata for database tokens and verify account-level permissions directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Database Token** from your Baserow settings (Settings > Database Tokens)
3. Start managing your no-code backend from Claude, Cursor, or any MCP client

No more manual entry into spreadsheet-like tables or digging through complex relations. Your AI acts as your dedicated database engineer and data architect.

### Who is this for?

- **Project Teams** — instantly retrieve project records and update statuses using natural language commands
- **Data Analysts** — automate the collection of structured information and manage relational tables without leaving your workspace
- **Developers** — integrate high-speed no-code backends into custom business workflows through simple AI queries


## Available Tools (9)
- **list_applications**: List all Baserow applications (databases)
- **create_row**: Provide data as a JSON string of field names and values.

Create a new row in a table
- **delete_row**: Delete a specific row
- **list_fields**: List fields in a table
- **get_row**: Get details for a specific row
- **list_rows**: Supports search and pagination.

List rows in a table
- **list_tables**: List tables in a database
- **update_row**: Provide data as a JSON string.

Update an existing row
- **list_workspaces**: List all Baserow workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Baserow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active database applications in my Baserow account."

**🤖 AI Agent:**
> I've retrieved your database directory. You currently have 3 applications: 'Project Tracker' (ID: 123), 'Customer CRM', and 'Inventory'. Which one would you like to explore for tables?

---

**👤 You:**
> "Show the records in table ID '456' from the 'Customer CRM' database."

**🤖 AI Agent:**
> Accessing records... I found 15 entries in table 456, including @user1 and @user2. I've retrieved their detailed field metadata for you. Shall I filter for a specific record?

---

**👤 You:**
> "Search for 'John Doe' in table '456'."

**🤖 AI Agent:**
> Searching... I found one match: 'John Doe' (Row ID: 789). His profile includes high-fidelity data like 'Email' and 'Plan Type'. Would you like to update any of these fields?


## ❓ FAQ

**Q: How do I find my Baserow Database Token?**
Log in to your account, navigate to **Settings** > **Database Tokens**, and create a new token with appropriate workspace permissions.

**Q: Can I search for records via AI?**
Yes! The `search_rows` tool allows your agent to find records across a specific table matching your search criteria programmatically.

**Q: How do I find Table and Database IDs?**
Use the `list_applications` tool to find Database IDs, and `list_database_tables` to find Table IDs within a specific application.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baserow-alternative](https://vinkius.com/mcp/baserow-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Baserow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `baserow-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Baserow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "baserow-alternative": {
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
