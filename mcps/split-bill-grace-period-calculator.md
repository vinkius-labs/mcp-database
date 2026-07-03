# Split-Bill Grace Period Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/split-bill-grace-period-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate adjusted repayment amounts for shared expenses when one party covers the cost upfront and the other delays their contribution.

## Description
The Split-Bill Grace Period Calculator is a financial utility designed to handle the 'float' when splitting expenses. When one person pays for a shared expense upfront and another party delays their contribution, this tool calculates the interest cost of that delay using a fixed daily rate. By using tools like `calculate_repayment_total`, `get_interest_accrual`, and `validate_bill_coverage`, you can determine exactly how much Person B should pay to ensure Person A is made whole, accounting for the opportunity cost of the delayed funds.


## Available Tools (3)
- **calculate_repayment_total**: Calculates the final, adjusted dollar amount that Person B must send to Person A
- **get_interest_accrual**: Isolates and identifies exactly how much extra money is being charged due to the delay
- **validate_bill_coverage**: Verifies if the combined initial payment and final repayment covers the total bill


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Split-Bill Grace Period Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If Person B owes $50.00 and is paying 10 days late, how much should they send to Person A?"

**🤖 AI Agent:**
> $50.10 should be sent to Person A (Principal: $50.00 + Interest: $0.10).

---

**👤 You:**
> "How much interest is being charged on a $200.00 debt that is 30 days overdue?"

**🤖 AI Agent:**
> The interest amount accrued over 30 days is $1.20.

---

**👤 You:**
> "I paid $40 upfront and Person B is paying back $65 for a $100 bill. Is the bill fully covered?"

**🤖 AI Agent:**
> The total amount covered is $105.00, which exceeds the original $100.00 bill. Status: satisfied.


## ❓ FAQ

**Q: How is the interest rate calculated?**
The tool uses a fixed daily rate of 0.02%, which is approximately 7.3% annually, applied to the principal amount for every day of the delay.

**Q: What does `calculate_repayment_total` do?**
It determines the final, adjusted dollar amount that Person B must send to Person A, including the interest accrued during the delay period.

**Q: Can I check if my total payments cover the original bill?**
Yes, you can use the `validate_bill_coverage` tool to verify if the combined initial payment and final repayment are sufficient to cover the total original expense.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/split-bill-grace-period-calculator](https://vinkius.com/mcp/split-bill-grace-period-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Split-Bill Grace Period Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `split-bill-grace-period-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Split-Bill Grace Period Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "split-bill-grace-period-calculator": {
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
