# Business Trip Reimbursement MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/business-trip-reimbursement)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate expense calculations, per diem, mileage, and final settlements.

## Description
This MCP server automates the complex process of business trip reimbursement. It connects AI agents to financial logic for calculating reimbursable expenses from receipts, applying policy limits, managing per diem allowances, and calculating mileage. Use `calculate_expense_totals` to process receipts against policy limits and exchange rates, `calculate_per_diem_allowance` for daily allowances, `calculate_mileage_reimbursement` for vehicle costs, and `calculate_final_settlement` to determine the net amount owed to or by the employee.


## Available Tools (4)
- **calculate_expense_totals**: Calculate total reimbursable and non-reimbursable expenses from receipts
- **calculate_final_settlement**: Calculate final net reimbursement or repayment
- **calculate_mileage_reimbursement**: Calculate mileage reimbursement
- **calculate_per_diem_allowance**: Calculate total per diem allowance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Business Trip Reimbursement** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my total reimbursable expenses for these receipts: [{'amount': 50, 'currency': 'EUR', 'category': 'meals', 'date': '2023-10-01'}]. My policy limit for meals is 40 and the EUR to USD rate is 1.1."

**🤖 AI Agent:**
> The total reimbursable amount is 40.00, and the non-reimbursable amount is 10.00.

---

**👤 You:**
> "I traveled for 5 days with a daily rate of 50. How much is my per diem?"

**🤖 AI Agent:**
> Your total per diem is 250.00.

---

**👤 You:**
> "What is my final settlement if my expenses are 500, per diem is 200, mileage is 50, and I received a 100 advance?"

**🤖 AI Agent:**
> The final net reimbursement is 650.00.


## ❓ FAQ

**Q: How does the tool handle currency conversion?**
You can use `calculate_expense_totals` by providing an exchange rates object. The tool will convert all receipt amounts to your base currency before checking them against policy limits.

**Q: Can I calculate the final amount I owe the company?**
Yes. By using `calculate_final_settlement`, the tool subtracts any advances from the sum of expenses, per diem, and mileage. A negative result indicates the amount the employee must repay.

**Q: What happens if my meal costs exceed the per diem?**
If you set `hasMealReceipts` to true in `calculate_per_diem_allowance`, the per diem for meals is zeroed out, and you should instead use `calculate_expense_totals` to process your actual meal receipts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/business-trip-reimbursement](https://vinkius.com/en/ai-agent-connect/business-trip-reimbursement)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Business Trip Reimbursement** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `business-trip-reimbursement` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Business Trip Reimbursement** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "business-trip-reimbursement": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
