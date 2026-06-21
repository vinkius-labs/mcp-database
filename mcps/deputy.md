# Deputy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deputy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage employee rosters, track timesheets, and monitor leave requests via the Deputy API.

## Description
Integrate **Deputy**, the ultimate workforce management solution, directly into your AI workflow. Manage your employee directory, monitor real-time shift rosters, track submitted timesheets, and handle leave requests using natural language.

### What you can do

- **Workforce Visibility** — List and retrieve detailed profiles for all employees in your Deputy organization.
- **Roster Monitoring** — Track current and upcoming shift rosters to ensure proper coverage across locations.
- **Timesheet Tracking** — Review submitted timesheets, including actual start and end times and approval statuses.
- **Leave Management** — List and monitor employee leave and time-off requests pending approval.

### How it works

1. Connect the Deputy integration to your AI assistant.
2. Authorize using your Deputy API Token and account Subdomain.
3. Optimize your team operations and scheduling through intuitive conversation.

### Who is this for?

- **Operations Managers** — Quickly check who is currently clocked in and shift coverage on the go.
- **HR & Payroll Teams** — Audit timesheets and monitor leave balances via chat.
- **Team Leads** — Review rosters and manage employee profiles during scheduling meetings.


## Available Tools
- **get_employee_profile**: Get detailed information for a specific employee
- **get_authenticated_user**: Retrieve metadata for the current authenticated API user
- **list_currently_active_shifts**: Identify employees who are currently clocked in (mock logic)
- **list_workforce_employees**: List all employees in your Deputy organization
- **list_leave_requests**: List all employee leave and time-off requests
- **list_business_locations**: List all physical business locations (companies) configured in Deputy
- **list_pending_leave_approvals**: List only the leave requests that are awaiting manager approval
- **list_active_rosters**: List all current and upcoming shift rosters
- **list_completed_timesheets**: List timesheets submitted by employees
- **search_employees_by_name**: Search for an employee by their display name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deputy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees currently clocked in."

**🤖 AI Agent:**
> I've checked the current timesheets and found 12 employees clocked in, including 'Alice Johnson' and 'Bob Miller'. Would you like to see their assigned locations?

---

**👤 You:**
> "Show me the roster for the 'Downtown Kitchen' location tomorrow."

**🤖 AI Agent:**
> Tomorrow at 'Downtown Kitchen', there are 5 shifts scheduled: 2 'Chefs' starting at 8:00 AM and 3 'Servers' starting at 11:00 AM. All shifts are currently assigned. Should I list the assigned employees?

---

**👤 You:**
> "Are there any pending leave requests?"

**🤖 AI Agent:**
> I found 3 pending leave requests: 'Sarah Lee' (Personal Leave, June 12-14) and 2 others. Would you like to see the full list with employee comments?


## ❓ FAQ

**Q: How do I get a Deputy API Token?**
Log in to your Deputy account, navigate to **Account Settings** → **API**, and generate a new Permanent Token for your integration.

**Q: What is the subdomain?**
It is the specific URL part of your Deputy portal, for example: 'mycompany.au.deputy.com'. You need to include the full host string.

**Q: Can the agent approve timesheets?**
This integration currently focuses on listing and auditing workforce data. Approving timesheets or modifying rosters should be managed through the Deputy dashboard or mobile app.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deputy](https://vinkius.com/mcp/deputy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deputy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `deputy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deputy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deputy": {
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
