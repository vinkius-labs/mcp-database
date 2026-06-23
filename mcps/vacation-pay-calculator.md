# Vacation Pay Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vacation-pay-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate vacation pay, constitutional bonuses, cash allowances, and tax withholdings.

## Description
An essential tool for calculating employee vacation entitlements. This MCP server provides precise calculations for gross vacation pay including the 1/3 constitutional bonus, cash allowance (abono pecuniário) for converting days to cash, income tax withholding (IRRF), and the legal payment deadline based on your vacation start date. Use `gross_vacation_pay` to find your base amount, `cash_allowance_value` to see the value of converted days, `tax_deductions` to calculate net pay, and `payment_due_date` to know when you must be paid.


## Available Tools (4)
- **cash_allowance_value**: Calculate the value of the cash allowance (abono pecuniário)
- **tax_deductions**: Calculate income tax withholding (IRRF)
- **gross_vacation_pay**: Calculate gross vacation pay and constitutional bonus
- **payment_due_date**: Calculate the vacation payment deadline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vacation Pay Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will my gross vacation pay be if my salary is 3000 and I am taking 30 days?"

**🤖 AI Agent:**
> Your gross vacation pay is 4000.00, which includes a constitutional bonus of 1000.00.

---

**👤 You:**
> "If I convert 10 days to cash with a salary of 3000, how much is the allowance?"

**🤖 AI Agent:**
> The value for your cash allowance (abono pecuniário) is 1000.00.

---

**👤 You:**
> "What is the tax withholding for a total taxable income of 5000?"

**🤖 AI Agent:**
> The IRRF withholding amount is 450.00, leaving you with a net payable amount of 4550.00.


## ❓ FAQ

**Q: How do I calculate my gross vacation pay?**
Use the `gross_vacation_pay` tool by providing your monthly base salary and the number of vacation days you are taking.

**Q: Can I calculate the tax deduction for my vacation?**
Yes, use the `tax_deductions` tool. You just need to provide the total taxable income, which includes your base pay and any bonuses.

**Q: How is the payment deadline determined?**
The `payment_due_date` tool calculates this by looking at your vacation start date and determining the date two days prior.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vacation-pay-calculator](https://vinkius.com/mcp/vacation-pay-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vacation Pay Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vacation-pay-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vacation Pay Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vacation-pay-calculator": {
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
