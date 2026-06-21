# SeaTable MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/seatable)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/seatable-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/seatable-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Build collaborative databases with spreadsheet simplicity and relational power for project management, CRM, and asset tracking.

## Description
Connect your **SeaTable** account to any AI agent and take full control of your database orchestration and collaborative workflows through natural conversation. SeaTable combines the power of a professional database with the ease of use of a spreadsheet, and this integration allows you to retrieve row metadata, append new records, and perform complex SQL queries directly from your chat interface.

### What you can do

- **Database & Row Orchestration** — List, create, and update rows programmatically to keep your collaborative data always synchronized.
- **SQL Query Intelligence** — Perform advanced data filtering and aggregation using standard SQL syntax directly from the AI interface.
- **Table & Metadata Control** — Access base metadata and list tables to maintain a clear overview of your digital workspace via natural language.
- **Automation & Token Oversight** — The integration automatically handles the complex exchange of permanent API tokens for short-lived access tokens to ensure secure data operations.
- **Operational Monitoring** — Track system activity and manage database records using simple AI commands to streamline your business workflows.

### How it works

1. Subscribe to this server
2. Enter your SeaTable API Token and Server URL (optional) from your base settings
3. Start managing your collaborative databases from Claude, Cursor, or any MCP-compatible client

No more manual copy-pasting or complex filter building. Your AI acts as a dedicated database administrator or operations coordinator.

### Who is this for?

- **Project Managers** — quickly retrieve task statuses and update project timelines without switching browser tabs.
- **Operations Teams** — automate the ingestion of new data records and perform aggregate queries via natural conversation.
- **Data Engineers** — streamline the retrieval of base metadata and monitor database structures directly within the chat.


## Available Tools
- **create_row**: Pass row data as a JSON string.

Add a new row to a table
- **create_table**: Create a new table
- **delete_row**: Delete a row from a table
- **get_base_metadata**: Get metadata for the current base
- **get_row**: Get a specific row from a table
- **list_columns**: List all columns in a table
- **list_rows**: List all rows in a table
- **list_tables**: List all tables and columns
- **list_views**: List all views for a table
- **query_sql**: Query data using SQL
- **update_row**: Update an existing row


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SeaTable** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all rows from the 'Inventory' table in SeaTable."

**🤖 AI Agent:**
> I've retrieved the records. You have 15 items in the 'Inventory' table, including 'Laptop Pro' (Stock: 5) and 'Office Chair' (Stock: 12). Would you like me to filter for low stock?

---

**👤 You:**
> "Show me all tables in the project database and pull the data from the Tasks table with filters."

**🤖 AI Agent:**
> Project database has 6 tables. "Tasks" (234 rows): 45 open, 123 in progress, 66 completed. "Team Members" (18 rows). "Milestones" (12 rows, 3 overdue). "Budget" (45 rows, total $234K). "Documents" (89 attachments). "Time Logs" (456 entries, 1,234 hours). Tasks filtered by status=open: 45 tasks. Top priority: "API redesign" (due tomorrow, assigned to Sarah). 8 tasks are blocked. Average completion time: 4.2 days. Overdue: 12 tasks.

---

**👤 You:**
> "Create a new table called Sprint Backlog with columns for story points, assignee, and sprint number."

**🤖 AI Agent:**
> Table "Sprint Backlog" created successfully. Columns configured: "Task Name" (text, primary), "Description" (long text), "Story Points" (number, range 1-13), "Assignee" (collaborator), "Sprint Number" (single select: Sprint 1-10), "Status" (single select: To Do, In Progress, Review, Done), "Priority" (single select: Critical, High, Medium, Low), "Created Date" (date, auto-fill). Default view: grouped by Sprint Number. 3 additional views created: Kanban by Status, Calendar view, and My Tasks filter.


## Installation & Usage

To install and use the **SeaTable** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/seatable](https://vinkius.com/mcp/seatable)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
