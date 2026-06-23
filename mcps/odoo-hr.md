# Odoo HR MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/odoo-hr)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Search employees, manage leaves, track attendance and expenses — Odoo HR through natural conversation.

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


## Available Tools (9)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Odoo HR** MCP server using an AI Agent (Claude, ChatGPT, etc.).

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

1. View installation instructions and explore the server: [https://vinkius.com/mcp/odoo-hr](https://vinkius.com/mcp/odoo-hr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Odoo HR** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `odoo-hr` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Odoo HR** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "odoo-hr": {
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
