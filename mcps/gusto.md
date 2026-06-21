# Gusto MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gusto)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage employees, run payroll, view benefits and time-off policies — HR automation for AI agents.

## Description
Connect **Gusto** to any AI agent and streamline your entire HR and payroll operation.

### What you can do

- **Employee Management** — List and view employee profiles with compensation details
- **Payroll Operations** — View payroll runs with earnings, taxes, and deductions
- **Company Info** — Access company details, EIN, and configuration
- **Benefits Administration** — Browse health, dental, 401k, and other benefit plans
- **Time-Off Policies** — View PTO, sick leave, and vacation accrual rates
- **Departments & Locations** — Organizational structure and office locations


## Available Tools
- **list_companies**: List managed companies
- **list_time_off_policies**: List time-off policies
- **get_company**: Get company details
- **list_employees**: List employees in a company
- **get_employee**: Get employee details
- **list_payrolls**: List payroll runs
- **get_payroll**: Get payroll run details
- **list_locations**: List company locations
- **list_departments**: List company departments
- **list_benefits**: ) with enrollment info.

List company benefits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gusto** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all employees in the engineering department."

**🤖 AI Agent:**
> Found 12 engineers:

| Name | Title | Start Date |
|------|-------|------------|
| Sarah Chen | Senior Engineer | Jan 2024 |
| Alex Rivera | Staff Engineer | Mar 2023 |
...

---

**👤 You:**
> "Show me the last payroll run details."

**🤖 AI Agent:**
> 📊 Payroll Run — March 31, 2026

| Metric | Value |
|--------|-------|
| Total Gross | $245,000 |
| Federal Tax | -$48,500 |
| State Tax | -$12,200 |
| Net Pay | $184,300 |
| Employees | 34 |

---

**👤 You:**
> "List all time-off policies."

**🤖 AI Agent:**
> 3 policies configured:

1. **Unlimited PTO** — Salaried employees
2. **Sick Leave** — 10 days/year, accrual-based
3. **Parental Leave** — 12 weeks paid


## ❓ FAQ

**Q: Can I view payroll details?**
Yes! Use `list_payrolls` to see all runs, then `get_payroll` for detailed breakdowns per employee.

**Q: Can I see employee benefits?**
Yes! Use `list_benefits` with a company ID to see all configured benefit plans including health, dental, and retirement.

**Q: Can I list all employees?**
Yes! Use `list_employees` with a company ID to get the full roster with names, departments, and roles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gusto](https://vinkius.com/mcp/gusto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gusto** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gusto` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gusto** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gusto": {
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
