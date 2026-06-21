# Odoo Project MCP Server

Create projects, manage tasks, log timesheets — Odoo Project Management through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/odoo-project)

## Overview
**Category:** productivity
**Tools Count:** 7

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


## Installation & Usage

To install and use the **Odoo Project** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/odoo-project](https://vinkius.com/mcp/odoo-project)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
