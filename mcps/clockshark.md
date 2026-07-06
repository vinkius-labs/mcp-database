# ClockShark MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clockshark)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track field crew hours with GPS-verified timesheets, job costing, and scheduling that keeps construction teams on budget.

## Description
Connect your **ClockShark** account to any AI agent and take full control of your field service workforce and time-tracking workflows through natural conversation.

### What you can do

- **Timesheet Orchestration** — List and manage individual time tracking entries programmatically, retrieving detailed historical clock-in/out records and location metadata
- **Schedule & Shift Intelligence** — Create and monitor work shifts and job assignments in real-time to maintain a perfectly coordinated field operation
- **Employee Lifecycle Management** — Access complete employee profiles and retrieve directories of active or inactive staff to oversee team distribution
- **Job & Task Architecture** — Programmatically manage your directory of service jobs and project codes to ensure your crew always has the high-fidelity info they need
- **Productivity Monitoring** — Monitor labor costs and project progress by creating new service tasks and tracking work types directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the ClockShark portal (Admin > Integrations > Connect Zapier)
3. Start managing your field workforce from Claude, Cursor, or any MCP client

No more manual following up on missing timesheets or digging through complex scheduling tables. Your AI acts as your dedicated field operations coordinator and labor analyst.

### Who is this for?

- **Operations Managers** — instantly retrieve labor reports and check project timelines using natural language commands
- **HR & Payroll Specialists** — monitor employee timesheets and verify clock-in accuracy without leaving your workspace
- **Construction Supervisors** — automate shift scheduling and job site assignments through simple AI queries


## Available Tools (10)
- **list_jobs**: List all jobs/projects
- **list_schedules**: List employee shifts
- **list_tasks**: List all service tasks
- **list_timesheets**: List time tracking entries
- **create_job**: Add a new job/project
- **create_shift**: Schedule a new shift
- **create_task**: Add a new work task
- **create_timesheet**: Manually add a time entry
- **get_employee_details**: Get details for a staff member
- **list_employees**: List all employees


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClockShark** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active employees in my ClockShark account."

**🤖 AI Agent:**
> I've retrieved your employee directory. You currently have 10 active staff members, including @user1 and @user2. Would you like to check the current timesheet for any of them?

---

**👤 You:**
> "Schedule a shift for 'John' (ID: 123) for tomorrow from 8 AM to 5 PM."

**🤖 AI Agent:**
> Shift scheduled! I've successfully assigned John to a new work shift for tomorrow. The assignment is now visible on your team's schedule. Shall I alert him via notification?

---

**👤 You:**
> "Show the timesheets for 'last_week'."

**🤖 AI Agent:**
> Fetching historical records... Last week, your crew logged a total of 320 hours across 5 active jobs. Highlights include 120 hours on the 'Riverfront Project'. Would you like the breakdown per employee?


## ❓ FAQ

**Q: How do I find my ClockShark API Key?**
Log in as an Admin, navigate to **Admin** > **Integrations**, click on **Connect Zapier**, and copy your unique API Key.

**Q: Can the agent schedule new work shifts?**
Yes! The `create_shift` tool allows the agent to assign a specific employee to a job with start and end times programmatically.

**Q: How do I retrieve a list of all jobs?**
Use the `list_jobs` tool to retrieve your complete directory of active and archived projects directly from the platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clockshark](https://vinkius.com/mcp/clockshark)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ClockShark** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clockshark` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ClockShark** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clockshark": {
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
