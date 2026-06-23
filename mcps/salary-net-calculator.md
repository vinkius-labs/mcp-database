# Salary Net Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salary-net-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate net salary, INSS, IRRF, and FGTS deductions based on gross pay.

## Description
An MCP server that calculates net salary by applying progressive tax brackets for INSS and IRRF. It provides a detailed breakdown of deductions including FGTS. Use tools like `calculate_net_payroll` to get precise results.


## Available Tools (3)
- **calculate_net_payroll**: Calculate net salary after INSS and IRRF deductions
- **compare_salary_scenarios**: Compare two gross salary amounts to see the difference in net pay
- **get_tax_configuration**: Retrieve the current INSS, IRRF, and FGTS tax configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salary Net Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate net salary for a gross pay of 5000."

**🤖 AI Agent:**
> For a gross salary of 5000, your net salary is 4250.50 after INSS and IRRF deductions.

---

**👤 You:**
> "Show me the current tax configuration summary."

**🤖 AI Agent:**
> The current configuration uses progressive brackets for INSS and IRRF, with a fixed FGTS rate of 8%.

---

**👤 You:**
> "Compare a gross salary of 3000 to 5000."

**🤖 AI Agent:**
> Comparing 3000 to 5000 results in a net pay difference of 1250.50 and an effective rate change of -1.5%.


## ❓ FAQ

**Q: How do I calculate my net salary?**
Use the `calculate_net_payroll` tool by providing your gross salary amount.

**Q: What taxes are included in the calculation?**
The calculation includes INSS, IRRF, and provides visibility into FGTS amounts.

**Q: Can I compare two different salaries?**
Yes, use the `compare_salary_scenarios` tool to see the difference in net pay between two gross salary inputs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salary-net-calculator](https://vinkius.com/mcp/salary-net-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salary Net Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salary-net-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salary Net Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salary-net-calculator": {
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
