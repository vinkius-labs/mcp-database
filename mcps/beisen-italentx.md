# Beisen (iTalentX) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/beisen-italentx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Comprehensive HR cloud platform — manage employees, attendance, and recruitment via AI.

## Description
Empower your AI agent to orchestrate your HR and talent management with **Beisen**, the leading cloud-based human resources platform in China. By connecting Beisen (iTalentX) to your agent, you transform complex employee records, attendance tracking, and recruitment pipelines into a natural conversation. Your agent can instantly list employees, retrieve attendance logs, monitor recruitment interviews, and even provide organization-wide activity summaries without you ever needing to navigate the comprehensive Beisen portal. Whether you are managing payroll processing or auditing employee leave, your agent acts as a real-time HR operations assistant, keeping your data accurate and your workforce managed.

### What you can do

- **Staff Orchestration** — List all employees, departments, and job positions across your organization.
- **Attendance Monitoring** — Retrieve real-time attendance records and manage employee leave requests.
- **Recruitment Control** — Monitor active job applications and scheduled interviews in the recruitment pipeline.
- **Payroll Auditing** — Retrieve high-level payroll summaries for specific processing periods.
- **Organization Insights** — Get real-time summaries of organization-wide HR activity and performance metrics.

### How it works

1. Subscribe to this server
2. Enter your Beisen App Key and App Secret
3. Start managing your HR operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers** — monitor team attendance, audit leave requests, and track hiring progress through natural language.
- **Recruitment Leads** — oversee interview schedules and application pipelines directly from your AI-powered workspace.
- **Operations Directors** — get high-level insights into organization structure and workforce statistics.
- **Payroll Administrators** — retrieve processing summaries and audit employee data for accurate payroll execution.


## Available Tools (10)
- **get_attendance_records**: Get attendance records
- **get_employee**: Get employee details
- **get_org_summary**: Get organization activity summary
- **get_payroll_summary**: Get payroll summary
- **list_departments**: List organization departments
- **list_employees**: List all employees
- **list_interviews**: List recruitment interviews
- **list_leave_requests**: List leave requests
- **list_positions**: List job positions
- **list_recruitment_applications**: List recruitment applications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beisen (iTalentX)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active employees in the Engineering department."

**🤖 AI Agent:**
> I've retrieved the list of employees for the Engineering department. You have 25 active members, including 5 Senior Developers and 12 Junior Engineers. Would you like the details for any specific person?

---

**👤 You:**
> "Show me recent leave requests pending approval."

**🤖 AI Agent:**
> I've found 4 leave requests pending approval, including 2 for 'Annual Leave' and 1 for 'Sick Leave'. Should I list the details or notify the respective managers?

---

**👤 You:**
> "Get a summary of the recruitment pipeline for this month."

**🤖 AI Agent:**
> Across your recruitment modules, there are currently 120 active applications and 15 interviews scheduled for this month. 5 positions were successfully filled last week. Would you like a breakdown by job category?


## ❓ FAQ

**Q: How do I obtain my Beisen App Key and Secret?**
Log in to the Beisen Admin Backend, navigate to [System Integration] → [Connectors], and create a new integration to generate your App Key and App Secret.

**Q: Can I check attendance records for specific employees?**
Yes. Use the `get_attendance_records` tool. You can provide an optional employee ID and date range to retrieve specific punch-in/out data.

**Q: Is it possible to monitor recruitment interviews?**
Yes! The `list_interviews` tool retrieves all scheduled recruitment sessions, allowing you to track interviewers, candidates, and times directly through the agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/beisen-italentx](https://vinkius.com/mcp/beisen-italentx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beisen (iTalentX)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `beisen-italentx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beisen (iTalentX)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beisen-italentx": {
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
