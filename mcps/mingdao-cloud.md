# Mingdao Cloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mingdao-cloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mingdao-cloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mingdao-cloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Enterprise zero-code application and workflow platform — manage worksheets, records, and automations via AI.

## Description
Empower your AI agent to orchestrate your enterprise workflows with **Mingdao Cloud** (HAP), the premier hyper-application platform for modern businesses. By connecting Mingdao Cloud to your agent, you transform complex worksheet management and data orchestration into a natural conversation. Your agent can instantly list your worksheets, retrieve column schemas, manage row data (create, update, delete), and even browse automated workflows without you ever needing to navigate the complex Mingdao interface. Whether you are managing an ERP system, a customized CRM, or internal HR processes, your agent acts as a real-time operations assistant, keeping your data accurate and your business logic moving.

### What you can do

- **Application Management** — List all accessible worksheets and retrieve detailed information about your enterprise applications.
- **Data Operations** — Manage worksheet rows (records) with full support for creating, listing, and granular updates.
- **Workflow Visualization** — Browse defined workflows to understand your automated business logic.
- **Schema Auditing** — Retrieve worksheet field schemas to understand your data structures and control IDs.
- **Team Overview** — List application users to manage collaboration and assignments effectively.

### How it works

1. Subscribe to this server
2. Enter your Mingdao App Key and Sign (App Secret)
3. Start managing your enterprise applications through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Enterprise Operations** — automate data entry and monitor business workflows through natural language.
- **System Integrators** — retrieve and audit worksheet records directly from your AI-powered workspace.
- **Department Managers** — oversee project data and internal requests through a unified AI interface.
- **IT Administrators** — manage application users and monitor automated workflows without manual technical overhead.


## Available Tools
- **add_row**: Add a new record to a worksheet
- **delete_row**: Delete a record from a worksheet
- **get_app_info**: Get application summary
- **get_row_details**: Get row detailed data
- **get_worksheet_schema**: Get worksheet field schema
- **list_rows**: List records in a worksheet
- **list_users**: List application users
- **list_workflows**: List application workflows
- **list_worksheets**: List all worksheets in the application
- **update_row**: Update an existing record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mingdao Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all worksheets in my application."

**🤖 AI Agent:**
> I've retrieved the worksheets for your application. You have 5 active tables, including 'Customer Leads', 'Orders', and 'Product Inventory'. Which one would you like to view data for?

---

**👤 You:**
> "Show me the last 3 rows from the 'Orders' worksheet."

**🤖 AI Agent:**
> I've listed the last 3 rows from the 'Orders' worksheet. They include Order #8821, #8822, and #8823. Would you like to see the detailed field data for any of these orders?

---

**👤 You:**
> "What are the automated workflows defined in this application?"

**🤖 AI Agent:**
> I've found 4 active workflows: 'New Lead Notification', 'Order Fulfillment Sync', 'Weekly Report Generator', and 'Inventory Alert'. Would you like more details on any specific workflow?


## Installation & Usage

To install and use the **Mingdao Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mingdao-cloud](https://vinkius.com/mcp/mingdao-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
