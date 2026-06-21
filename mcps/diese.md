# Diese MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/diese)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/diese-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/diese-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [project-management](../categories/project-management.md)

Equip your AI agent to manage ERP projects, track invoices, and monitor resource planning via the Diese API.

## Description
Integrate **Diese**, the comprehensive cloud-based ERP software, directly into your AI workflow. Manage your business projects, monitor sales invoices and expenses, track resource planning and tasks, and research business partners using natural language.

### What you can do

- **Project Oversight** — List and retrieve detailed configuration for all active and archived projects in your ERP.
- **Billing & Expense Tracking** — Monitor sales invoices and business expenses, tracking their status and organizational approval.
- **Resource Intelligence** — Access scheduled planning entries and resource allocations to ensure project efficiency.
- **Task Management** — List pending project tasks and identify items that have passed their deadline.

### How it works

1. Connect the Diese integration to your AI assistant.
2. Authorize using your Diese API Key and portal Subdomain.
3. Orchestrate your enterprise operations and planning through intuitive conversation.

### Who is this for?

- **Project Managers** — Quickly check project statuses and resource availability on the go.
- **Operations Leaders** — Monitor invoice processing and expense approvals via chat.
- **Finance Teams** — Audit billing cycles and project budgets during planning sessions.


## Available Tools
- **get_account_metadata**: Retrieve metadata and usage limits for your Diese account
- **get_project_details**: Get detailed information for a specific ERP project
- **list_erp_contacts**: List all business contacts and partners in the system
- **list_business_expenses**: List all recorded business expenses and their approval status
- **list_sales_invoices**: List all generated sales invoices and their payment status
- **list_overdue_erp_tasks**: Identify project tasks that have passed their deadline (mock logic)
- **list_resource_planning**: List scheduled planning entries and resource allocations
- **list_erp_projects**: List all active and archived projects in your Diese account
- **list_project_tasks**: List pending and completed tasks across all projects
- **search_projects_by_name**: Search for a project using a name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Diese** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active ERP projects."

**🤖 AI Agent:**
> I've found 5 active projects in your account, including 'Product Launch Phase 2' and 'Client X Onboarding'. Would you like to see the assigned resources for any of these?

---

**👤 You:**
> "Show me the unpaid invoices from last month."

**🤖 AI Agent:**
> I've retrieved 3 unpaid invoices from last month, totaling $4,500. The largest is for 'Alpha Corp' ($2,200). Should I check the contact details for their finance department?

---

**👤 You:**
> "Are there any project tasks overdue?"

**🤖 AI Agent:**
> Yes, I found 2 overdue tasks: 'Document Final Review' (Deadline: June 10th) and 'Server Migration' (Deadline: June 12th). Would you like to see who is assigned to these tasks?


## Installation & Usage

To install and use the **Diese** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/diese](https://vinkius.com/mcp/diese)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
