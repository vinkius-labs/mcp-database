# Shared Building Expense Settlement MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shared-building-expense-settlement)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Settles shared building expenses by calculating unit obligations and optimized transfers.

## Description
This MCP server provides a complete financial settlement engine for shared building expenses. It allows AI agents to calculate how much each unit owes based on allocation shares using `calculate_expense_distribution`, determine net financial positions with `calculate_settlement_balances`, and generate the most efficient payment paths via `optimize_minimum_transfers`. It also provides unit-specific health checks through `get_unit_status_summary`.


## Available Tools (4)
- **calculate_expense_distribution**: Determines how much each beneficiary owes based on the total expense and their assigned shares
- **get_unit_status_summary**: Provides a high-level overview of the financial health of a specific unit regarding a specific expense
- **calculate_settlement_balances**: Calculates the net financial position (owed vs. paid) for every unit involved in the expense
- **optimize_minimum_transfers**: Generates the most efficient list of payments required to settle all outstanding debts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shared Building Expense Settlement** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the distribution for a $1000 expense where Unit A has a share of 600 and Unit B has a share of 400."

**🤖 AI Agent:**
> Unit A owes $600 and Unit B owes $400.

---

**👤 You:**
> "What is the status of Unit 101 if they have a net balance of -50?"

**🤖 AI Agent:**
> Unit 101 is a Debtor with a total debt of $50.

---

**👤 You:**
> "Generate the minimum transfers for Unit A (balance +100) and Unit B (balance -100)."

**🤖 AI Agent:**
> Unit B should pay Unit A $100.


## ❓ FAQ

**Q: How does the tool calculate what each unit owes?**
The `calculate_expense_distribution` tool takes the total expense and a list of unit shares to determine the exact amount owed by each beneficiary.

**Q: Can I minimize the number of bank transfers needed?**
Yes, use `optimize_minimum_transfers` to generate a list of the fewest possible payments required to clear all debts.

**Q: How do I check if a specific unit has already paid?**
You can use `calculate_settlement_balances` to see the `amountPaid` for each unit, or `get_unit_status_summary` for a high-level status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shared-building-expense-settlement](https://vinkius.com/en/ai-agent-connect/shared-building-expense-settlement)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shared Building Expense Settlement** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shared-building-expense-settlement` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shared Building Expense Settlement** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shared-building-expense-settlement": {
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
