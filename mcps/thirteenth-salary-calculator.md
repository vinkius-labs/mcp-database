# Thirteenth Salary Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thirteenth-salary-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate gross and net 13th-month salary installments, including proportional earnings and tax deductions.

## Description
This MCP server provides a precise way to calculate the thirteenth-month salary (13º salário) for employees. It handles the complexities of proportional earnings based on months worked, progressive social security deductions, and income tax withholdings. Using tools like `get_thirteenth_breakdown`, you can obtain a complete financial overview including gross amounts, total deductions, net totals, and specific details for both the first and second installments.


## Available Tools (4)
- **compute_social_security_deduction**: Compute the social security deduction
- **compute_income_tax_deduction**: Compute the income tax deduction
- **calculate_proportional_gross**: Calculate the proportional gross salary
- **get_thirteenth_breakdown**: Get the complete breakdown of the thirteenth salary


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Thirteenth Salary Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my 13th salary if my monthly base salary is 3000 and I worked 8 months this year."

**🤖 AI Agent:**
> Based on a monthly salary of 3,000.00 and 8 months worked, your total proportional gross amount is 2,000.00.

---

**👤 You:**
> "What will my second installment be if I earn 5000 per month and worked 12 months?"

**🤖 AI Agent:**
> For a full year of work at 5,000.00 per month, your second installment after all social security and income tax deductions will be 4,250.50.

---

**👤 You:**
> "Show me the full breakdown for a salary of 2500 and 6 months worked, with payments in November and December."

**🤖 AI Agent:**
> Your total gross amount is 1,250.00. After deductions, your net total is 1,180.00. The first installment in November will be 625.00 and the second in December will be 555.00.


## ❓ FAQ

**Q: How is the proportional gross salary calculated?**
The `calculate_proportional_gross` tool calculates this by dividing your annual base salary by twelve and multiplying it by the number of full months worked in the current year.

**Q: Does the calculator include tax deductions?**
Yes, you can use `compute_social_security_deduction` and `compute_income_tax_deduction` to find the specific amounts deducted from your gross salary.

**Q: Can I see a full breakdown of both installments?**
Yes, the `get_thirteenth_breakdown` tool provides a complete summary including gross amount, total deductions, net amount, and details for both installments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thirteenth-salary-calculator](https://vinkius.com/mcp/thirteenth-salary-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Thirteenth Salary Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `thirteenth-salary-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Thirteenth Salary Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thirteenth-salary-calculator": {
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
