# BrioHR MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/briohr)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrate BrioHR management — retrieve employee profiles, monitor leave, and integrate claim reports directly from any AI agent.

## Description
Connect your AI agents to **BrioHR**, the all-in-one HR software designed to simplify the management of your greatest asset: your people. This MCP provides 10 tools to automate HR data orchestration, from employee record synchronization and leave monitoring to claim report retrieval and recruitment oversight.

### What you can do

- **Employee Insights** — Download main information for all employees and retrieve detailed individual profiles including roles and departments
- **Time-Off Orchestration** — Monitor who is away within specific date ranges and retrieve detailed leave requests for any employee
- **Financial Integration** — Access approved claim reports for external payroll/accounting syncing and monitor monthly payroll summaries
- **Talent Acquisition** — List active job postings and monitor candidates through the recruitment pipeline
- **Performance & Org** — Track performance appraisal cycles and inspect organizational department structures

### How it works

1. Subscribe to this server
2. Contact [**BrioHR Support**](mailto:support@briohr.com) to request API access and whitelist your IP addresses
3. Obtain your **API Username**, **Password**, and **Company ID**
4. Insert your credentials into the fields below to start managing your HR workflows.

### Who is this for?

- **HR Business Partners** — quickly retrieve employee data and monitor leave trends via natural language
- **Finance & Payroll Teams** — automate the extraction of approved claims for accounting reconciliation
- **Operations Managers** — monitor department headcount and active recruitment efforts smoothly


## Available Tools (10)
- **get_employee_details**: Get detailed profile for a specific employee
- **get_payroll_summary**: Get payroll overview for a specific month
- **get_who_is_away**: List employees who are currently away or scheduled for leave
- **list_performance_appraisals**: List performance review cycles
- **list_job_candidates**: List candidates for a specific job
- **list_claim_reports**: Retrieve approved claim reports for payroll integration
- **list_departments**: List organizational departments
- **list_employees**: Download the main information for all employees
- **list_job_postings**: List active job openings in the recruitment module
- **list_leave_requests**: Retrieve leave requests for an employee


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BrioHR** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who is away in my company between 2024-05-01 and 2024-05-15?"

**🤖 AI Agent:**
> Checking BrioHR leave records... I've found 3 employees away during that period: 1. John Doe (Annual Leave), 2. Jane Smith (Sick Leave), 3. Robert Brown (Personal Leave). Would you like to see the specific request details for any of them?

---

**👤 You:**
> "List all active job postings in my BrioHR account."

**🤖 AI Agent:**
> Retrieving job openings... I've found 4 active postings: 1. Senior Frontend Engineer (ID: job_101), 2. Product Marketing Manager (ID: job_102), 3. HR Coordinator (ID: job_103), 4. Customer Support Lead (ID: job_104).

---

**👤 You:**
> "Show the payroll summary for January 2024."

**🤖 AI Agent:**
> Connecting to BrioHR payroll service... For January 2024, the total headcount was 50 employees. Total payroll costs processed: RM 250,000.00. Status: Fully processed. Would you like the department breakdown?


## ❓ FAQ

**Q: How do I get API access for BrioHR?**
You must reach out to the BrioHR support team at support@briohr.com. They will provide your credentials and require your IP addresses for whitelisting before you can connect.

**Q: Can my AI automatically list all active job postings?**
Yes! Use the `list_job_postings` tool. Your agent will retrieve all current vacancies from your BrioHR recruitment module, including titles and IDs.

**Q: How do I retrieve the payroll summary for a specific month?**
Use the `get_payroll_summary` tool with the month (MM) and year (YYYY). The agent will return the headcount and total calculations for that period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/briohr](https://vinkius.com/mcp/briohr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BrioHR** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `briohr` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BrioHR** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "briohr": {
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
