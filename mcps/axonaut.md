# Axonaut MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/axonaut)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/axonaut-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/axonaut-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

All-in-one ERP and CRM automation — manage invoices, quotes, tasks, and company relationships via AI.

## Description
Transform your business administration with **Axonaut**, the all-in-one ERP designed for high-velocity teams. By connecting Axonaut to your AI agent, you turn complex organizational management into a natural conversation. Your agent can instantly audit unpaid invoices, list active quotations, manage CRM contacts, and orchestrate team tasks without you ever navigating through dense financial menus. Whether you're tracking expenses or preparing project reports, your agent acts as a direct bridge to your business data, ensuring your operations stay lean and efficient.

### What you can do

- **CRM Orchestration** — List and search through company and contact records to maintain a complete view of your business relationships.
- **Financial Auditing** — Retrieve and audit lists of invoices, quotations (quotes), and expenses directly through natural language.
- **Task Management** — Create, list, and manage team tasks with deadlines and descriptions to keep projects moving forward.
- **Business Oversight** — Explore your product catalog, active orders, and project milestones without manual dashboard data entry.
- **Connectivity Check** — Instantly verify your account health and retrieve current user context to ensure system integrity.

### How it works

1. Subscribe to this server
2. Enter your Axonaut API Key
3. Start managing your business operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Small Business Owners** — monitor invoices and manage customer relationships through natural conversation.
- **Sales Teams** — quickly list quotations and update contact information without leaving the CRM chat.
- **Operations Managers** — audit expenses and manage team task backlogs directly from your AI agent.
- **Accountants** — retrieve financial document lists and product metadata for rapid auditing.


## Available Tools
- **create_task**: Create a new task
- **get_account_check**: Verify Axonaut connection and get current user info
- **get_company**: Get details for a specific company
- **list_companies**: List all companies in Axonaut
- **list_contacts**: List all contacts
- **list_expenses**: List all expenses
- **list_invoices**: List all invoices
- **list_orders**: List all orders
- **list_products**: List all products
- **list_projects**: List all projects
- **list_quotations**: List all quotations (quotes/devis)
- **list_tasks**: List all tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Axonaut** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my invoices from the last 30 days."

**🤖 AI Agent:**
> I've retrieved your invoices. You have 12 invoices from the last 30 days, totaling €4,500. 3 of them are currently marked as 'Unpaid'.

---

**👤 You:**
> "Create a task called 'Follow up with New Client' due tomorrow."

**🤖 AI Agent:**
> Task 'Follow up with New Client' has been successfully created in Axonaut. I've set the deadline for tomorrow.

---

**👤 You:**
> "Search for a company named 'TechCorp'."

**🤖 AI Agent:**
> I found 'TechCorp' in your Axonaut database. They are currently listed as an 'Active Client' with 2 associated contacts. Would you like to see the details?


## Installation & Usage

To install and use the **Axonaut** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/axonaut](https://vinkius.com/mcp/axonaut)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
