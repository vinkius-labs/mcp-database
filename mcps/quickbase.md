# Quickbase MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/quickbase)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Build custom business apps with a no-code platform that connects data, automates workflows, and adapts as your needs evolve.

## Description
Connect your **Quickbase** account to any AI agent and take full control of your enterprise-grade no-code application and data orchestration through natural conversation. Quickbase provides a robust platform for managing complex business processes, and this integration allows you to query records, upsert data, and monitor application structures directly from your chat interface.

### What you can do

- **Record & Data Orchestration** — Query, insert, update, and delete records programmatically using the modern JSON RESTful API.
- **Application Lifecycle Management** — Access and monitor your Quickbase apps and retrieve detailed metadata including table and field structures directly from the AI interface.
- **Report & Analysis Intelligence** — Run existing reports and retrieve detailed result metadata via natural language to maintain high-fidelity business intelligence.
- **User & Permission Control** — List users and monitor access across your digital workspace to ensure secure data operations.
- **Operational Monitoring** — Track system activity and manage table metadata using simple AI commands to ensure your apps are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Quickbase Realm Hostname and User Token from your preferences
3. Start managing your no-code ecosystem from Claude, Cursor, or any MCP-compatible client

No more manual data entry or jumping between multiple tables. Your AI acts as a dedicated application administrator or data coordinator.

### Who is this for?

- **Operations Managers** — quickly retrieve project statuses and monitor workflow health without switching apps.
- **IT Administrators** — automate the management of user access and track application metadata via natural conversation.
- **Data Analysts** — streamline the retrieval of table records and monitor business metrics directly within the chat.


## Available Tools (11)
- **delete_records**: Delete records from a table
- **get_app**: Get details of a specific application
- **get_report**: Get details for a specific report
- **get_table**: Get details of a specific table
- **list_apps**: List all applications
- **list_fields**: List all fields in a table
- **list_reports**: List all reports for a table
- **list_tables**: List all tables in an application
- **list_users**: List all users in an application
- **query_records**: See Quickbase API docs for query syntax.

Query records from a table
- **upsert_records**: Insert or update records in a table


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Quickbase** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active applications in my Quickbase realm."

**🤖 AI Agent:**
> I've retrieved your apps. You have 3 active environments: 'Sales Tracker', 'Project Management', and 'HR Portal'. Which one would you like to see tables for?

---

**👤 You:**
> "Show me all records in the Project Tracker table where status is In Progress and deadline is this week."

**🤖 AI Agent:**
> 12 records found in Project Tracker matching criteria. 4 are due today: "API Integration" (assigned: James Park, 85% complete), "Data Migration Phase 2" (Sarah Chen, 70%), "UI Testing Sprint" (Alex Rivera, 90%), "Documentation Update" (Lisa Wang, 95%). 5 are due by Wednesday. 3 are due Friday. Total estimated hours remaining: 67. 2 tasks are flagged as at-risk based on progress vs deadline analysis.

---

**👤 You:**
> "Create a new table in the Operations app for tracking vendor invoices with approval workflow."

**🤖 AI Agent:**
> Table "Vendor Invoices" created in Operations app. 12 fields configured: Vendor Name (text), Invoice Number (unique ID), Amount (currency), Date Received, Due Date, Status (dropdown: Pending/Approved/Rejected/Paid), Approver (user), PO Number (linked to Purchase Orders table), Category, Notes, Attachments, and Approval Date. Workflow rule added: auto-notify approver when new invoice is submitted. Dashboard widget created showing pending invoices by amount.


## ❓ FAQ

**Q: Can my AI automatically query records with specific filters in Quickbase?**
Yes! Use the `query_records` tool. Provide the Table ID (DBID) and a query object (using Quickbase query syntax), and your agent will return the matching records and metadata instantly.

**Q: How do I find my Realm Hostname and User Token?**
Your Realm Hostname is your Quickbase URL (e.g., yourcompany.quickbase.com). To get a User Token, go to **My Preferences** > **Manage my user tokens** in your Quickbase account.

**Q: Does this work with the older XML API?**
This integration specifically targets the modern JSON RESTful API (v1) for better performance and security. We recommend using REST-compatible user tokens for all operations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quickbase](https://vinkius.com/mcp/quickbase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Quickbase** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `quickbase` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Quickbase** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quickbase": {
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
