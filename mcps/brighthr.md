# BrightHR MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brighthr)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Simplify people management with holiday tracking, shift scheduling, and absence management built for UK and ANZ businesses.

## Description
Connect your **BrightHR** account to any AI agent and take full control of your workforce management and employee lifecycle through natural conversation.

### What you can do

- **Employee Orchestration** — List and manage all employee profiles programmatically, including job roles, departments, and high-fidelity compensation metadata
- **Absence & Leave Intelligence** — Monitor sickness, lateness, and planned holiday requests in real-time to maintain a perfectly coordinated team schedule
- **Benefits & Training Monitoring** — Access complete directories of employee benefits and retrieve training history to oversee organizational development
- **Operational Visibility** — Access high-fidelity metadata for your organization and monitor active webhooks directly through your agent for instant reporting
- **Connectivity Verification** — Verify API health and check connectivity status programmatically to ensure a perfectly coordinated integration ecosystem

### How it works

1. Subscribe to this server
2. Retrieve your **Access Token** from your BrightHR dashboard (Settings > API or Developer Portal)
3. Start managing your human resources from Claude, Cursor, or any MCP client

No more manual toggling between HR dashboards or digging through complex holiday tables. Your AI acts as your dedicated HR administrator and team coordinator.

### Who is this for?

- **HR Managers** — instantly retrieve employee summaries and log absences using natural language commands
- **Team Leaders** — monitor holiday schedules and verify team availability without leaving your workspace
- **Business Owners** — automate the oversight of organizational structure and compensation through simple AI queries


## Available Tools
- **check_api_health**: Verify BrightHR API status
- **record_absence**: g., sickness) for an employee.

Log a new employee absence
- **get_organization_info**: Get company details
- **get_employee_details**: Get details for a specific employee
- **get_employee_job_details**: Get job metadata
- **get_employee_salary_info**: Get salary information
- **list_absences**: Can be filtered by employee ID.

List employee absences
- **list_employee_benefits**: List benefits for an employee
- **list_employees**: List all employees
- **list_holiday_requests**: Can be filtered by employee ID.

List holiday/leave requests
- **list_training_records**: List training history
- **list_configured_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BrightHR** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active employees in my organization."

**🤖 AI Agent:**
> I've retrieved your employee directory. You currently have 25 active staff members, including @user1 and @user2. Would you like to see the detailed job metadata for any of them?

---

**👤 You:**
> "Show the holiday requests for employee ID 'emp_123'."

**🤖 AI Agent:**
> Fetching leave records... Employee emp_123 has 2 upcoming holiday requests: a 1-week trip in June (Approved) and a 3-day break in August (Pending). Shall I retrieve the high-fidelity absence history for them?

---

**👤 You:**
> "Record a sickness absence for @user1 starting from tomorrow."

**🤖 AI Agent:**
> Absence recorded! I've successfully registered the sickness absence for @user1 in BrightHR. The start date is set for tomorrow. Shall I notify the team lead about this update?


## ❓ FAQ

**Q: How do I find my BrightHR Access Token?**
Log in to your account, navigate to **Settings** > **API**, or visit the **BrightHR Developer Portal** to generate a Personal Access Token.

**Q: Can I record a sickness absence via AI?**
Yes! The `record_absence` tool allows you to log an absence by providing the employee ID, reason, and start date programmatically.

**Q: How do I check upcoming holidays?**
Use the `list_holiday_requests` tool to retrieve all planned leave, with the option to filter by specific employee IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brighthr](https://vinkius.com/mcp/brighthr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BrightHR** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `brighthr` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BrightHR** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brighthr": {
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
