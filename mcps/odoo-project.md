# Odoo Project MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/odoo-project)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Create projects, manage tasks, log timesheets — Odoo Project Management through natural conversation.

## Description
Connect **Odoo ERP** to any AI agent — manage your entire business without switching tabs.

### What you can do
- **CRM** — Search and create leads, track opportunities through your pipeline
- **Contacts** — Find individual contacts and companies, create new partners
- **Sales** — List and manage sales orders with full order details
- **Notes** — Add comments and notes to any record in your Odoo instance

### Who is this for?
- **Sales Teams** — CRM pipeline at your fingertips through AI
- **Account Managers** — Quick access to contact and company information
- **Operations** — Monitor sales orders without switching screens
- **Odoo Administrators** — Query any module through natural conversation


## Available Tools
- **odoo_create_project**: project record. The name is the project title. Optionally link it to an existing customer/partner using their res.partner ID. Use when the user wants to set up a new project for internal work, a client engagement, or a product initiative.

Create a new project in Odoo, optionally linked to a customer or partner
- **odoo_create_task**: task record in the specified project. Requires the project.project ID (use odoo_list_projects to find it). Optionally assign to a res.users ID and set a deadline in YYYY-MM-DD format. Use when the user wants to add a to-do item, delegate work, or plan project deliverables.

Create a new task within an Odoo project, optionally assigning it to a user with a deadline
- **odoo_list_projects**: project records showing all active projects. Returns project name, project manager, linked customer/partner, total task count, start date, and end date. Use when the user asks about ongoing projects, wants a project overview, or needs to find a project ID for task creation.

List all projects in Odoo with responsible person, customer, task count, and date range
- **odoo_list_tasks**: task records. Optionally filter by project ID to see tasks for a specific project, or omit to see tasks across all projects. Returns task name, project, assigned users, kanban stage (e.g., New/In Progress/Done), priority (0=normal, 1=important), progress percentage, deadline, and creation date. Use when the user asks about to-do lists, task assignments, project progress, or upcoming deadlines.

List project tasks in Odoo with assignee, kanban stage, priority, progress, and deadlines
- **odoo_list_timesheets**: analytic.line records where project_id is set — these are timesheet entries that track hours worked. Returns description, project, task, employee, hours logged (unit_amount), and date. Use when the user asks about time tracking, billable hours, employee workload, or project time allocation.

List timesheet entries in Odoo showing employee, project, task, hours logged, and date
- **odoo_log_timesheet**: analytic.line record linking hours to a specific project and task. Requires project.project ID, project.task ID, hours worked, and a description of the work performed. Optionally specify a date (defaults to today). Use when the user wants to log time spent, track billable hours, or record daily work activities.

Log a timesheet entry — record hours worked on a specific project task with a description
- **odoo_update_task**: task record. You can change the task name, priority (0=normal, 1=important/starred), deadline (YYYY-MM-DD), or any other writable field. Use when the user wants to rename a task, change its priority, reschedule the deadline, or modify task details.

Update an existing task in Odoo — change name, priority, deadline, or other properties


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Odoo Project** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for leads from the website"

**🤖 AI Agent:**
> 👥 **CRM Leads — Website**
| Name | Email | Stage | Revenue |
|---|---|---|---|
| Acme Corp | info@acme.com | Qualification | $15,000 |
| Beta Inc | hello@beta.io | Proposition | $8,500 |

---

**👤 You:**
> "Show recent sales orders"

**🤖 AI Agent:**
> 📋 **Sales Orders**
| SO# | Customer | Amount | Status |
|---|---|---|---|
| S00042 | Acme Corp | $12,500 | Confirmed |
| S00041 | Beta Inc | $3,200 | Draft |


## ❓ FAQ

**Q: Which Odoo versions are supported?**
This server uses the JSON-RPC protocol, which is compatible with Odoo 14, 15, 16, 17, and 18. Both Odoo Community and Enterprise editions are supported.

**Q: Does it work with Odoo.com (SaaS)?**
Yes! Works with both Odoo.com hosted instances and self-hosted Odoo servers. Just provide your instance URL and API key.

**Q: How do I generate an API Key?**
Go to Settings → Users → select your user → API Keys tab → New API Key. Give it a descriptive name and copy the generated key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/odoo-project](https://vinkius.com/mcp/odoo-project)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Odoo Project** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `odoo-project` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Odoo Project** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "odoo-project": {
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
