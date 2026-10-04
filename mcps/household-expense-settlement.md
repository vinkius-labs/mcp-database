# Household Expense Settlement MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-expense-settlement)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate individual financial standings and minimize reimbursement transfers for shared household costs.

## Description
This MCP server provides a complete engine for managing shared household expenses. It allows AI agents to calculate exactly how much each person has paid versus what they owe based on custom ownership weights. Use `calculate_individual_standings` to see the net position of every participant, `generate_settlement_plan` to find the minimum number of transfers needed to balance the books, and `get_expense_summary` for a high-level overview of total spending. It also includes `validate_weights` to ensure your ownership percentages are mathematically sound.


## Available Tools (4)
- **get_expense_summary**: Get a high-level summary of total household expenses
- **calculate_individual_standings**: Calculate individual financial standings based on expenses and ownership weights
- **generate_settlement_plan**: Generate a minimum transfer settlement plan
- **validate_weights**: Validate if ownership weights are mathematically valid


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Expense Settlement** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the standings for Alice (0.6) and Bob (0.4) where Alice paid 60 and Bob paid 40."

**🤖 AI Agent:**
> Alice has paid 60 and owes 48, resulting in a net position of +12. Bob has paid 40 and owes 24, resulting in a net position of +16. Wait, let me recalculate: Alice paid 60, owes 60. Bob paid 40, owes 40. If weights are 0.6/0.4: Alice paid 60, owes 60, net 0. Bob paid 40, owes 40, net 0. Let's use different numbers: Alice paid 100, Bob paid 20. Total 120. Alice owes 72, Bob owes 48. Alice net +28, Bob net -28.

---

**👤 You:**
> "Generate a settlement plan for Alice (+20) and Bob (-20)."

**🤖 AI Agent:**
> Bob should transfer 20 to Alice.

---

**👤 You:**
> "What is the total expense if Alice paid 50 and Bob paid 30?"

**🤖 AI Agent:**
> The total expenses are 80.


## ❓ FAQ

**Q: How does the settlement plan work?**
The `generate_settlement_plan` tool uses a strategy to minimize the number of transactions by matching the largest debtors with the largest creditors.

**Q: What happens if my ownership weights don't add up to 100%?**
You can use the `validate_weights` tool to check your weights. The engine requires that the sum of all ownership weights equals exactly 1.0.

**Q: Can I see a summary of all spending?**
Yes, the `get_expense_summary` tool provides the total expenses, transaction count, and identifies the top contributor.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-expense-settlement](https://vinkius.com/en/ai-agent-connect/household-expense-settlement)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Expense Settlement** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-expense-settlement` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Expense Settlement** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-expense-settlement": {
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
