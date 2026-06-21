# Feishu Bitable MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/feishu-bitable)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Collaborative multi-dimensional table platform by Lark — manage bases, tables, and records via AI.

## Description
Empower your AI agent to orchestrate your data with **Feishu Bitable** (Lark), the leading multi-dimensional table platform for modern collaboration. By connecting Feishu Bitable to your agent, you transform complex database management and record tracking into a natural conversation. Your agent can instantly list your tables, retrieve field schemas, manage records (create, update, delete), and even search through your data without you needing to navigate the web interface. Whether you are managing a project tracker, a customized CRM, or an asset database, your agent acts as a real-time data assistant, keeping your bases organized and your team aligned.

### What you can do

- **Base Orchestration** — Retrieve metadata about your Bitable bases and list all tables within them.
- **Data Operations** — Manage table records with full support for batch creation, listing, and granular updates.
- **View & Field Auditing** — Browse defined views and field schemas to understand your data structures.
- **Advanced Search** — Search through records using filter expressions to find exactly what you need.
- **Team Alignment** — Access base information to ensure your AI agent has the correct context for your collaboration.

### How it works

1. Subscribe to this server
2. Enter your Feishu/Lark App ID and App Secret
3. Start managing your Bitable bases through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Managers** — automate record entry and monitor database consistency through natural language.
- **Project Leads** — track milestones and update project tables directly from your AI-powered workspace.
- **Operations Teams** — oversee multiple Bitable bases and data structures through a unified AI interface.
- **Lark/Feishu Users** — integrate your existing Bitable workflows into your AI-driven daily routines.


## Available Tools
- **create_records**: Batch create records in a table
- **delete_record**: Delete a record from a table
- **get_base_info**: Get Bitable base information
- **get_record_details**: Get record detailed data
- **list_fields**: List fields in a table
- **list_records**: List records in a table
- **list_tables**: List tables in a Bitable app
- **list_views**: ) defined for a table.

List views in a table
- **search_records**: Search records with filter
- **update_record**: Update an existing record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Feishu Bitable** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all tables in Bitable base 'AppbcbWCzen6D8dezhoCH2RpMAh'."

**🤖 AI Agent:**
> I've retrieved the tables for the specified Bitable base. There are 3 tables: 'Inventory', 'Suppliers', and 'Orders'. Which one would you like to view records for?

---

**👤 You:**
> "Add a new record to the 'Inventory' table with fields: Name='MacBook Pro', Quantity=5."

**🤖 AI Agent:**
> Done! I've added the new record to the 'Inventory' table. The entry for 'MacBook Pro' with a quantity of 5 has been successfully created.

---

**👤 You:**
> "Search for records in table 'tblsRc9GRRXKqhvW' where 'Status' equals 'Shipped'."

**🤖 AI Agent:**
> I've performed the search and found 8 records matching your criteria. Would you like me to list their details or summarize the results?


## ❓ FAQ

**Q: How do I find my Feishu/Lark App ID and Secret?**
Log in to the [Feishu Open Platform](https://open.feishu.cn/), create a new application or select an existing one, and you will find your App ID and App Secret in the 'Credentials' section.

**Q: Where can I find the 'appToken' for my Bitable base?**
The `appToken` is the unique identifier found in the URL of your Bitable base. It typically looks like `AppbcbWCzen6D8dezhoCH2RpMAh` and appears after `/base/` in the browser address bar.

**Q: Does my application need specific permissions?**
Yes. Ensure your application has the 'View, comment, edit and manage Bitable' (bitable:app) permission enabled in the Developer Console and that the bot is added as a collaborator to the base.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/feishu-bitable](https://vinkius.com/mcp/feishu-bitable)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Feishu Bitable** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `feishu-bitable` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Feishu Bitable** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "feishu-bitable": {
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
