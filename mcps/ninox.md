# Ninox MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ninox)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ninox-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ninox-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Build custom business databases and apps with a visual platform that replaces spreadsheets with structured, relational data.

## Description
Connect your **Ninox** account to any AI agent and take full control of your low-code database orchestration and business automation through natural conversation. Ninox provides a powerful platform for creating custom business apps, and this integration allows you to retrieve database schemas, manage records across tables, and execute native Ninox scripts directly from your chat interface.

### What you can do

- **Database & Table Orchestration** — List all managed databases within your teams and retrieve detailed table schemas programmatically to ensure your data foundation is always synchronized.
- **Record Lifecycle Management** — Create, update, and delete records across any Ninox table with detailed field metadata directly from the AI interface to maintain high-fidelity business data.
- **Script & Query Intelligence** — Execute native Ninox scripts and complex queries via natural language to perform advanced data manipulation and custom calculations.
- **Team & Workspace Control** — List your organizational teams and monitor workspace access using simple AI commands to maintain a clear overview of your digital infrastructure.
- **Operational Monitoring** — Track system responses and manage data ingestion to ensure your business applications are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Ninox Personal Access Token and Team ID from your account settings
3. Start managing your custom databases from Claude, Cursor, or any MCP-compatible client

No more manual data entry in complex forms. Your AI acts as a dedicated database administrator or business operations lead.

### Who is this for?

- **Business Owners & Ops Leads** — quickly retrieve project statuses and monitor business metrics without switching apps.
- **Data Analysts** — automate the retrieval of table records and execute custom scripts via natural conversation.
- **Developers** — integrate real-time database management and custom business logic directly within the chat.


## Available Tools
- **create_records**: Create or update records
- **delete_record**: Delete a record
- **execute_ninox_script**: Execute a Ninox script/query
- **get_database_schema**: Get database schema
- **get_record**: Get details for a specific record
- **list_databases**: List all databases in the team
- **list_records**: List records from a table
- **update_record**: Update a specific record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ninox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all tables in my Ninox database ID 'db123'."

**🤖 AI Agent:**
> I've retrieved your tables. You have 4 active structures including 'Invoices', 'Customers', and 'Inventory'. Which one would you like to see records for?

---

**👤 You:**
> "Show me the schema and field definitions for the Customers table in database db_main."

**🤖 AI Agent:**
> The Customers table in db_main has 8 fields: Name (text, required), Email (email), Phone (phone), Company (text), Status (choice: Active/Inactive/Lead), Revenue (number, currency), Created Date (date), and Notes (multiline text). There are 342 records currently in this table.

---

**👤 You:**
> "Create a new record in the Orders table with customer Acme Corp, amount 4500, and status Pending."

**🤖 AI Agent:**
> New record created successfully in the Orders table (Record ID: 1847). Customer: Acme Corp, Amount: $4,500.00, Status: Pending. The record was automatically timestamped with today's date and linked to the existing Acme Corp entry in your Customers table.


## Installation & Usage

To install and use the **Ninox** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ninox](https://vinkius.com/mcp/ninox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
