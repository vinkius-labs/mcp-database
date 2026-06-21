# Belvo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/belvo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Access financial data across Latin America via Belvo — list links, accounts, and transactions directly from any AI agent.

## Description
Connect your **Belvo** account to any AI agent and orchestrate your financial data workflows across Latin America through natural conversation.

### What you can do

- **Connection Management** — List and inspect all financial institution links (connections) managed by Belvo.
- **Account Oversight** — Query and retrieve details for banking and gig-economy accounts.
- **Transaction Analysis** — List and filter financial transactions to understand spending patterns and history.
- **Income & Expense Insights** — Access processed insights like recurring expenses and income summaries.
- **Investment Portfolios** — Retrieve detailed information on investment holdings and performance.
- **Institution Discovery** — List all supported banks and institutions in the Belvo ecosystem.

### How it works

1. Subscribe to this server
2. Enter your Belvo Secret ID and Secret Password
3. Start querying financial data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fintech Developers** — quickly audit links and account data without navigating the Belvo dashboard.
- **Financial Analysts** — retrieve transaction and income data for modeling and reporting.
- **Product Managers** — verify institution coverage and data availability directly from their workspace.


## Available Tools
- **get_account**: Get specific account details
- **get_investments**: List investment portfolios
- **get_link**: Get specific connection details
- **get_transaction**: Get specific transaction details
- **list_accounts**: List all financial accounts across all links
- **list_balances**: List balances for all accounts
- **list_incomes**: List income insights for the links
- **list_institutions**: List all supported financial institutions
- **list_links**: List all connections (links) to financial institutions
- **list_owners**: List owners of the financial accounts
- **list_recurring_expenses**: List recurring expense insights
- **list_transactions**: List all transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Belvo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active financial links in my Belvo account."

**🤖 AI Agent:**
> I've retrieved 3 active links: 'Itau' (ID: link_123), 'Nubank' (ID: link_456), and 'Uber' (ID: link_789). Which one would you like to explore?

---

**👤 You:**
> "Show my account balances across all links."

**🤖 AI Agent:**
> Fetching balances... I found 2 accounts: 'Savings (Itau)' with R$ 5,000.00 and 'Checking (Nubank)' with R$ 1,200.00.

---

**👤 You:**
> "List recurring expenses found in my accounts."

**🤖 AI Agent:**
> Retrieving insights... I've identified 4 recurring expenses, including 'Netflix', 'Electricity Bill', and 'Gym Membership'. Would you like the breakdown for any of these?


## ❓ FAQ

**Q: Can I check the balance of a specific account using this integration?**
Yes! Use the `get_account` tool with the Account ID. Your agent will fetch the latest balance and account metadata directly from Belvo.

**Q: How do I list all transactions for a particular connection?**
Simply ask the agent to `list_transactions`. You can then inspect specific transaction details using the `get_transaction` tool with the Transaction ID.

**Q: Does the integration support all institutions in Brazil and Mexico?**
This integration supports all institutions currently active in your Belvo account across supported countries. Use the `list_institutions` tool to see the full list of available banks and platforms.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/belvo](https://vinkius.com/mcp/belvo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Belvo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `belvo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Belvo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "belvo": {
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
