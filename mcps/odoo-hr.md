# Odoo HR MCP Server

Search employees, manage leaves, track attendance and expenses — Odoo HR through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/odoo-hr)

## Overview
**Category:** human-resources
**Tools Count:** 9

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
- **odoo_create_leave**: leave record in "draft" state. Requires the employee ID (from odoo_search_employees), leave type ID (from odoo_list_leave_types), and date range in format "YYYY-MM-DD HH:MM:SS". The request goes through the standard approval workflow. Use when the user wants to request time off for an employee.

Submit a leave request for an employee with specific leave type, start date, and end date
- **odoo_list_attendance**: attendance records ordered by check-in time descending. Returns employee name, check-in timestamp, check-out timestamp (if clocked out), and total worked hours. Use when the user asks about who is currently working, attendance history, or daily hours tracking.

List employee attendance records (check-in/check-out times and worked hours) from Odoo
- **odoo_list_departments**: department records showing the organizational structure. Returns department name, department manager, parent department (for hierarchy), and total employee count. Use when the user asks about org structure, department headcounts, or management hierarchy.

List all departments in Odoo HR with their managers, parent departments, and headcount
- **odoo_list_employees**: employee records — the full employee directory. Returns name, department, job title, work email, and direct manager for each employee. Use for a headcount overview, department composition analysis, or when the user wants to browse the org chart.

List all employees in the Odoo HR directory with departments, job titles, and contact information
- **odoo_list_expenses**: expense records ordered by date. Returns expense description, employee, state (draft/reported/approved/done/refused), total amount, and date. Use when the user asks about pending expense reports, reimbursement requests, or wants to review recent employee expenses.

List employee expense reports in Odoo with amounts, approval status, and submission dates
- **odoo_list_jobs**: job records — the defined job positions in the organization. Returns job title, department, number of open recruitments, and recruitment state. Use when the user asks about open positions, hiring pipeline, or workforce planning.

List open job positions and recruitment status in Odoo HR with department and vacancy count
- **odoo_list_leave_types**: leave.type records — the categories of leave employees can request. Returns type name and configuration. Use to find the correct leave type ID before creating a leave request, or when the user asks what kinds of time off are available.

List available leave types (Paid Time Off, Sick Leave, Unpaid, etc.) configured in Odoo HR
- **odoo_list_leaves**: leave records ordered by date. Returns employee name, department, leave type (e.g., Paid Time Off, Sick Leave), state (draft/confirm/validate/refuse), number of days, and date range. Use when the user asks about upcoming absences, pending leave approvals, vacation schedules, or team availability.

List leave requests (vacation, sick, personal days) in Odoo with approval status and duration
- **odoo_search_employees**: employee records by name. Returns employee name, department, job title/position, work email, direct manager, and hire date. Use when the user wants to find a specific employee, look up their department or manager, or get contact details for an internal team member.

Search employees in Odoo by name, returning their department, job title, email, and manager


## Installation & Usage

To install and use the **Odoo HR** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/odoo-hr](https://vinkius.com/mcp/odoo-hr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
