# US Payroll Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-payroll-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise US payroll tax liabilities, including FICA, Medicare, FUTA, and SUTA.

## Description
This MCP server provides tools to calculate various United States payroll tax obligations. Use `calculate_employee_withholdings` to determine employee-side deductions like Social Security and Medicare. Use `calculate_employer_liabilities` to find employer costs including FUTA and state-specific SUTA based on the provided state code. Finally, use `get_payroll_summary` for a high-level comparison of net pay versus total company cost.


## Available Tools
- **calculate_employee_withholdings**: Calculate employee-side tax withholdings
- **calculate_employer_liabilities**: Calculate employer-side tax liabilities
- **get_payroll_summary**: Get a high-level payroll summary


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Payroll Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate how much will be withheld from an employee earning $75,000 per year."

**🤖 AI Agent:**
> The `calculate_employee_withholdings` tool will return the Social Security, Medicare, and any additional Medicare withholdings for a $75,000 salary.

---

**👤 You:**
> "What are the employer tax liabilities for an employee in California earning $100,000?"

**🤖 AI Agent:**
> Using `calculate_employer_liabilities` with annualGrossPay: 100000 and stateCode: 'CA' will provide the Social Security, Medicare, FUTA, and SUTA liabilities.

---

**👤 You:**
> "Provide a payroll summary for $150,000 gross pay in Texas."

**🤖 AI Agent:**
> The `get_payroll_summary` tool will calculate the net employee pay, total employer cost, and the aggregate tax burden for $150,000 in TX.


## ❓ FAQ

**Q: How do I calculate employee withholdings?**
Use the `calculate_employee_withholdings` tool by providing the annual gross pay in USD.

**Q: Does this include state-specific taxes?**
Yes. By using `calculate_employer_liabilities` with a valid two-letter US state code, the tool calculates SUTA based on predefined state rates.

**Q: Can I see a summary of total costs?**
Yes, the `get_payroll_summary` tool provides a comparison between net employee pay and the total employer cost.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-payroll-tax-calculator](https://vinkius.com/mcp/us-payroll-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Payroll Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `us-payroll-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Payroll Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-payroll-tax-calculator": {
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
