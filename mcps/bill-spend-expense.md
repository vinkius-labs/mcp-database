# BILL Spend & Expense MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bill-spend-expense)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage corporate spend via BILL — list budgets, cards, and transactions directly from any AI agent.

## Description
Connect your **BILL Spend & Expense (formerly Divvy)** account to any AI agent and orchestrate your corporate spending through natural conversation.

### What you can do

- **Budget Oversight** — List and inspect active budgets to track spending against limits.
- **Card Management** — View virtual and physical cards assigned to employees.
- **Transaction Auditing** — Retrieve real-time transactions and merchant data.
- **User Management** — List employees and review their roles.
- **Reimbursement Tracking** — Check the status of out-of-pocket expense claims.

### How it works

1. Subscribe to this server
2. Enter your BILL Spend API Token
3. Start managing your expenses from Claude, Cursor, or any MCP-compatible client


## Available Tools (5)
- **list_budgets**: List all budgets
- **list_cards**: List all cards
- **list_reimbursements**: List all reimbursements
- **list_transactions**: List recent transactions
- **list_users**: List all users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BILL Spend & Expense** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active budgets."

**🤖 AI Agent:**
> I've retrieved your budgets. You have 'Marketing Q2' and 'Engineering Software' budgets.

---

**👤 You:**
> "Show recent transactions."

**🤖 AI Agent:**
> Retrieving transactions... I found 5 recent charges, including AWS ($150) and Uber ($25).

---

**👤 You:**
> "List pending reimbursements."

**🤖 AI Agent:**
> You have 2 pending reimbursements for 'Team Lunch' and 'Conference Travel'.


## ❓ FAQ

**Q: Can I view recent transactions across the company?**
Yes! Use the `list_transactions` tool to retrieve recent corporate card usage and merchant details.

**Q: How do I check my available budget?**
Simply ask the agent to `list_budgets` to retrieve budget limits and current spend amounts.

**Q: Does the integration allow me to create virtual cards?**
Currently, the toolset focuses on querying and auditing (listing cards, budgets, transactions). Creating cards must be done on the platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bill-spend-expense](https://vinkius.com/mcp/bill-spend-expense)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BILL Spend & Expense** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bill-spend-expense` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BILL Spend & Expense** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bill-spend-expense": {
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
