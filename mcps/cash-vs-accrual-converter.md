# Cash vs Accrual Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/cash-vs-accrual-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Converts farm financial statements from cash basis to accrual basis.

## Description
This MCP server provides specialized tools for agricultural accounting, allowing AI agents to transform cash-basis bookkeeping into accrual-basis reporting. By adjusting cash receipts and expenses with accounts receivable, accounts payable, inventory changes, and prepaid expenses, it reflects the true economic performance of a farm. Use `get_accrual_revenue` to calculate earned revenue, `get_accrual_expenses` for incurred costs, `calculate_net_farm_income` for the final profit/loss, and `generate_reconciliation_schedule` for a detailed adjustment breakdown.


## Available Tools (4)
- **calculate_net_farm_income**: Determines the final adjusted profit or loss for the farm
- **generate_reconciliation_schedule**: Provides a detailed breakdown showing how to get from cash basis to accrual basis
- **get_accrual_expenses**: Calculates the total cost of operations incurred during the period using the accrual method
- **get_accrual_revenue**: Calculates the total revenue earned during the period using the accrual method


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cash vs Accrual Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my accrual revenue. I had $50,000 in cash receipts, $5,000 in accounts receivable, and my grain inventory increased by $2,000."

**🤖 AI Agent:**
> Your total accrual revenue is $57,000.

---

**👤 You:**
> "What are my total accrual expenses? I paid $30,000 in cash, I owe $4,000 to suppliers, and I have $1,000 in prepaid expenses."

**🤖 AI Agent:**
> Your total accrual expenses are $33,000.

---

**👤 You:**
> "Generate a reconciliation schedule for: $40,000 cash receipts, $30,000 cash expenses, $2,000 accounts receivable, $1,500 accounts payable, $3,000 inventory increase, and $500 prepaid expenses."

**🤖 AI Agent:**
> The reconciliation shows an accrual net income of $14,000 based on your provided adjustments.


## ❓ FAQ

**Q: What is the difference between cash and accrual basis in farming?**
Cash basis tracks physical money moving in and out, while accrual basis matches income and expenses to when they actually occurred. This tool uses `generate_reconciliation_schedule` to show exactly how to bridge that gap.

**Q: How does inventory affect my accrual income?**
An increase in inventory (like stored grain) is treated as earned revenue, while a decrease is treated as an expense. You can use `get_accrual_revenue` to include these changes in your totals.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, this MCP server can be connected to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/cash-vs-accrual-converter](https://vinkius.com/ai-agent-connect/cash-vs-accrual-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cash vs Accrual Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cash-vs-accrual-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cash vs Accrual Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cash-vs-accrual-converter": {
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
