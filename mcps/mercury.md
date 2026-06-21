# Mercury MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mercury)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Equip your AI agent with direct access to Mercury — check account balances, review transactions, and manage recipients without opening the banking dashboard.

## Description
Connect your **Mercury** business banking account to your AI agent and manage your startup finances conversationally.

### What you can do

- **Account Balances** — Check real-time balances across all your Mercury accounts instantly from your AI agent.
- **Transaction History** — Pull recent transactions filtered by date, amount, or counterparty to track spending patterns.
- **Recipient Management** — List, create, and manage payment recipients for ACH and wire transfers.
- **Account Details** — Retrieve routing numbers, account numbers, and account metadata programmatically.

### How it works

1. Subscribe to the Mercury integration on the marketplace.
2. Generate an API token from your Mercury dashboard (Settings → API Tokens).
3. Ask your AI agent to check balances, pull transactions, or manage recipients.

### Who is this for?

- **Startup Founders** — Get an instant snapshot of your runway and cash position during investor calls without switching to a browser.
- **Finance & Operations Teams** — Automate daily balance checks and transaction reconciliation directly from your development environment.
- **Bookkeepers & CFOs** — Monitor cash flow and payment activity across multiple Mercury accounts from a single conversational interface.


## Available Tools (10)
- **list_accounts**: List all Mercury bank accounts
- **list_team_members**: List all team members
- **get_account**: Get bank account details
- **list_transactions**: List recent transactions
- **get_transaction**: Get transaction details
- **list_recipients**: List payment recipients
- **create_recipient**: Required for sending payments.

Create a new payment recipient
- **list_payments**: List sent payments
- **list_statements**: List bank statements
- **get_treasury_balance**: Get treasury balance overview


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mercury** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the current balance on all my Mercury accounts?"

**🤖 AI Agent:**
> I queried your Mercury accounts. You have two active accounts: 'Operating Account' with $142,350.00 and 'Savings Reserve' with $500,000.00. Total cash position: $642,350.00.

---

**👤 You:**
> "Show me all transactions above $5,000 from this month."

**🤖 AI Agent:**
> I found 4 transactions above $5,000 this month: AWS Infrastructure ($12,400), Payroll Run ($87,500), Office Lease ($8,200), and Legal Retainer ($15,000). Total: $123,100.

---

**👤 You:**
> "List all my payment recipients."

**🤖 AI Agent:**
> You have 12 saved recipients. Here are the top 5 by frequency: AWS (ACH), Gusto Payroll (ACH), WeWork (Wire), Stripe Atlas (ACH), and Latham & Watkins (Wire).


## ❓ FAQ

**Q: How do I get my Mercury API token?**
Log in to your Mercury account at app.mercury.com. Go to **Settings → API Tokens** and click **Create Token**. Choose the token type (Read Only for balance checks, or Read and Write for managing recipients). Copy the token immediately — it will only be shown once. Paste it into the configuration field below, and you're ready. No code, no SDK, no webhooks.

**Q: Can my AI agent check my startup's runway instantly during a board meeting?**
Absolutely. Just ask your AI agent 'What's my current balance across all Mercury accounts?' and it returns real-time balances for every account — checking, savings, and treasury — in seconds. No tab-switching, no logging in, no waiting for the dashboard to load.

**Q: What if I need to review recent transactions for month-end close?**
Ask your AI agent to pull transactions from any date range. It retrieves each transaction with amount, counterparty, status, and date — perfect for reconciliation. You can filter by account, ask for Wire vs ACH breakdowns, or request only transactions above a specific threshold, all without exporting CSVs.

**Q: Is this suitable for companies with multiple Mercury accounts?**
Yes. The integration retrieves data across all accounts linked to your API token — operating accounts, savings accounts, and treasury balances. Perfect for venture-backed startups managing multiple entities, holding companies, or finance teams tracking cash positions across subsidiaries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mercury](https://vinkius.com/mcp/mercury)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mercury** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mercury` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mercury** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mercury": {
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
