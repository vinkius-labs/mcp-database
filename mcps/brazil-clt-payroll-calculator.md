# Brazil CLT Payroll Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brazil-clt-payroll-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Brazil's CLT payroll components including INSS, IRRF, net pay, and employer costs.

## Description
This MCP server provides a specialized engine for calculating all essential components of the Brazilian CLT (Consolidation of Arbitrated Labor Laws) payroll. It allows AI agents to perform precise calculations for progressive Social Security (INSS) deductions, federal Income Tax (IRRF) considering dependents, net monthly salary, and total employer expenditure including statutory charges like FGTS. Use `get_social_security_deduction` to find INSS amounts, `get_income_tax_deduction` for IRRF, `calculate_employee_net_pay` for a full paycheck summary, and `calculate_employer_total_cost` to estimate the total economic impact on the company.


## Available Tools (4)
- **calculate_employer_total_cost**: Calculate the total employer cost
- **get_income_tax_deduction**: Calculate the IRRF deduction
- **get_social_security_deduction**: Calculate the progressive INSS deduction
- **calculate_employee_net_pay**: Calculate the employee net pay


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brazil CLT Payroll Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the INSS deduction for a gross salary of 5000.00?"

**🤖 AI Agent:**
> For a gross salary of $5,000.00, the calculated INSS deduction is $518.82, with the highest applied rate being 14%.

---

**👤 You:**
> "Calculate the net pay for an employee earning 3000.00 with 2 dependents and an INSS deduction of 260.00."

**🤖 AI Agent:**
> The net salary for the employee is $2,715.45, after subtracting the INSS and IRRF deductions from the gross salary of $3,000.00.

---

**👤 You:**
> "What is the total employer cost for a 4000.00 salary with an 8% contribution rate?"

**🤖 AI Agent:**
> The total monthly expenditure for the employer is $4,320.00, which includes a burden amount of $320.00.


## ❓ FAQ

**Q: How does the INSS calculation work?**
The `get_social_security_deduction` tool uses a progressive bracket method. It partitions the gross salary into specific ranges, applying the corresponding tax rate to each slice of income.

**Q: Can I calculate the impact of dependents on Income Tax?**
Yes. When using `get_income_tax_deduction`, you can provide the number of qualifying dependents to reduce the taxable base, which lowers the final IRRF amount.

**Q: Does this tool estimate employer costs?**
Yes, the `calculate_employer_total_cost` tool estimates the total monthly expenditure by adding statutory charges like FGTS to the gross salary based on a provided contribution rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brazil-clt-payroll-calculator](https://vinkius.com/mcp/brazil-clt-payroll-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brazil CLT Payroll Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `brazil-clt-payroll-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brazil CLT Payroll Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brazil-clt-payroll-calculator": {
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
