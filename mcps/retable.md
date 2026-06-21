# Retable MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/retable)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/retable-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/retable-mcp)
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


## Installation & Usage

To install and use the **Retable** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/retable](https://vinkius.com/mcp/retable)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
