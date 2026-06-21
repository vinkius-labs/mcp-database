# KeyPay MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/keypay)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage payroll, employees, and pay runs via the Employment Hero Payroll (KeyPay) API.

## Description
Connect your **KeyPay** (now Employment Hero Payroll) account to any AI agent to streamline your payroll operations. This MCP server enables your agent to interact with businesses, pay runs, employees, and compliance data directly.

### What you can do

- **Payroll Oversight** — List and retrieve detailed information for pay runs and earnings
- **Employee Management** — Query employee profiles, payroll configurations, and metadata
- **Document Access** — List issued payslips for specific employees instantly
- **Leave Tracking** — Monitor historical and pending leave requests across your businesses
- **Compliance & Deductions** — Inspect deduction lines and payroll items to ensure accuracy

### How it works

1. Subscribe to this server
2. Enter your KeyPay API Key and Region Domain
3. Start managing your payroll from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Payroll Administrators** — Quickly check pay run statuses and employee details via natural language
- **HR Managers** — Monitor leave requests and employee payroll profiles effortlessly
- **Business Owners** — Get instant visibility into payroll costs and history


## Available Tools (10)
- **list_businesses**: List all businesses associated with the account
- **list_pay_run_deductions**: List deductions for a specific pay run
- **list_pay_run_earnings**: List earnings for a specific pay run
- **list_employees**: List employees for a business
- **get_business_details**: Get details for a specific business
- **get_employee_details**: Get details for a specific employee
- **get_pay_run_details**: Get details for a specific pay run
- **list_leave_requests**: List leave requests for a business
- **list_pay_runs**: List pay runs for a business
- **list_pay_slips**: List payslips for an employee


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KeyPay** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all businesses in my KeyPay account."

**🤖 AI Agent:**
> I've retrieved your businesses. You have 3 registered entities: 'Acme Australia', 'Acme Global Services', and 'Tech Ventures Pty Ltd'.

---

**👤 You:**
> "Show me the pay runs for business ID '12345'."

**🤖 AI Agent:**
> For business 12345, I found 5 recent pay runs. The latest is 'Fortnightly Pay Period' ending May 15th, currently marked as 'Finalised'.

---

**👤 You:**
> "Find employee 'John Smith' in business '12345'."

**🤖 AI Agent:**
> I've found 'John Smith' (ID: 98765) in business 12345. He is currently active and listed as a 'Senior Developer'.


## ❓ FAQ

**Q: In which regions is the KeyPay API available?**
KeyPay supports multiple regions including Australia, UK, New Zealand, Singapore, and Malaysia. Make sure to provide the correct region domain during setup.

**Q: Can I see my employee's payslips using this agent?**
Yes, the `list_pay_slips` tool allows you to retrieve a list of issued payslips for a specific employee within a business.

**Q: Is it possible to track leave requests?**
Absolutely. Use the `list_leave_requests` tool to fetch all historical and pending leave requests for any of your registered businesses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keypay](https://vinkius.com/mcp/keypay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **KeyPay** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `keypay` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **KeyPay** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "keypay": {
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
