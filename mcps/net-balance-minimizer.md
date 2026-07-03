# Net Balance Minimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/net-balance-minimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Efficiently settle group debts with the minimum number of transactions.

## Description
The Net Balance Minimizer is a specialized calculation engine designed to resolve financial imbalances within any group. By analyzing expenses and participant contributions, it identifies exactly who owes what and generates the most efficient settlement plan possible. Using a greedy optimization algorithm, it minimizes the total number of transfers required to bring everyone's balance back to zero, saving time and reducing complexity in shared expense management. You can use tools like `settlement_transactions_tool` to automate your group settlements.


## Available Tools (3)
- **net_balances**: Calculate the net balance for each participant
- **expense_summary**: Summarize total group expenditure
- **settlement_transactions**: Generate transactions to settle all balances


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Net Balance Minimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate net balances for Alice, Bob, and Charlie. Expenses: Alice paid $50 for everyone, Bob paid $20 for Alice and Bob."

**🤖 AI Agent:**
> Alice: +$13.33, Bob: -$6.67, Charlie: -$6.67

---

**👤 You:**
> "Generate a settlement plan for these balances: Alice: +$20, Bob: -$15, Charlie: -$5."

**🤖 AI Agent:**
> 1. Bob transfers $15 to Alice
2. Charlie transfers $5 to Alice

---

**👤 You:**
> "Summarize these expenses: [{'payer_name': 'Dave', 'amount': 100, 'split_between': ['Dave', 'Eve']}]"

**🤖 AI Agent:**
> Total group expenditure: $100.00 across 1 expense entry.


## ❓ FAQ

**Q: How does the minimization algorithm work?**
The engine uses a greedy strategy: it identifies the person with the largest debt and matches them with the person who is owed the most. It settles the maximum possible amount for one of these parties in each step, repeating until all balances are zero.

**Q: What tools are available in this MCP server?**
The server provides three primary tools: `net_balances_tool` to calculate individual surpluses or deficits, `settlement_transactions_tool` to generate the transfer list, and `expense_summary_tool` for a high-level overview of group spending.

**Q: Can I use this with Claude Desktop or Cursor?**
Yes, you can connect this server to any MCP-compatible client like Claude Desktop, Cursor, VS Code, or Windsurf using your personal Connection Token from the Vinkius dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/net-balance-minimizer](https://vinkius.com/mcp/net-balance-minimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Net Balance Minimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `net-balance-minimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Net Balance Minimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "net-balance-minimizer": {
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
