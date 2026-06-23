# 13th Month Salary Provision Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/13th-month-salary-provision-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate monthly 13th-month salary accruals, employer taxes, and cumulative payroll liabilities.

## Description
This MCP server provides a specialized calculation engine for managing the financial obligations of 13th-month salary accruals. It allows users to calculate the monthly breakdown of base salary portions (1/12th) plus associated employer burdens, track cumulative liability for specific employees from the start of the fiscal year, and assess the total company-wide financial exposure. Use `get_monthly_accrual_breakdown` to see a month-by-month cost analysis, `get_employee_liability_summary` to monitor individual employee debt, and `get_company_financial_exposure` for a high-level view of all active staff liabilities.


## Available Tools (3)
- **get_employee_liability_summary**: Answers how much total money has been provisioned for a specific employee from the start of the year to date
- **get_monthly_accrual_breakdown**: Provides a detailed breakdown of the specific financial obligation for a single employee for a given month
- **get_company_financial_exposure**: Provides a high-level view of the entire company's total accumulated financial obligation for all employees


## 💬 Prompt Examples

Here are some examples of how you can interact with the **13th Month Salary Provision Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the financial breakdown for employee EMP001 for month 5?"

**🤖 AI Agent:**
> For employee EMP001 in month 5, the base accrual amount is $500.00, the tax burden is $120.00, resulting in a total monthly cost of $620.00.

---

**👤 You:**
> "How much is the total accumulated liability for employee EMP002 so far this year?"

**🤖 AI Agent:**
> The cumulative liability for employee EMP002 from the start of the year to date is $3,450.00, consisting of $3,000.00 in base accruals and $450.00 in employer taxes.

---

**👤 You:**
> "What is the total financial exposure for the entire company?"

**🤖 AI Agent:**
> The aggregate company liability across all 50 active employees is $125,400.00.


## ❓ FAQ

**Q: What is included in the monthly accrual calculation?**
The calculation includes one-twelfth of the employee's monthly base salary plus the applicable employer charges (taxes and social security) based on their employment tier.

**Q: How can I see the total debt for a specific employee?**
You can use the `get_employee_liability_summary` tool by providing the unique employee ID to retrieve the accumulated base total, taxes, and running liability for the current fiscal year.

**Q: Does this tool account for different types of employment contracts?**
Yes, the engine distinguishes between Permanent and Contractual tiers, applying different statutory employer burden rates to each.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/13th-month-salary-provision-calculator](https://vinkius.com/mcp/13th-month-salary-provision-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **13th Month Salary Provision Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `13th-month-salary-provision-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **13th Month Salary Provision Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "13th-month-salary-provision-calculator": {
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
