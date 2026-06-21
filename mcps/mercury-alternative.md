# Mercury MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mercury-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Bank smarter for your startup with FDIC-insured accounts, treasury management, and business banking built for tech companies.

## Description
Connect your **Mercury** banking account to any AI agent and manage startup finances through natural conversation.

### What you can do

- **Account Management** — Access balances across all checking and savings accounts
- **Transactions** — Browse and filter recent transactions and transfers
- **Statements** — Retrieve monthly account statements
- **Cash Flow** — Track incoming revenue and outgoing expenses
- **Recipient Management** — Access saved wire and ACH recipients

### How it works

1. Subscribe to this server
2. Enter your Mercury API Token
3. Start managing your finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Founders** — check runway and cash flow quickly
- **Finance Teams** — automate transaction categorization and reconciliation
- **Developers** — build internal financial dashboards


## Available Tools
- **get_account**: Get details for a specific Mercury account
- **get_balance**: Get account balance
- **list_accounts**: List Mercury bank accounts
- **list_cards**: List Mercury debit cards
- **list_customers**: List invoicing customers
- **list_invoices**: List account receivable invoices
- **list_recipients**: List payment recipients
- **list_transactions**: List transactions for an account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mercury** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show my current balances for all accounts."

**🤖 AI Agent:**
> Balances retrieved: Total available: $142,500.00. Checking Account (...1234): $45,200.00. Savings Account (...5678): $90,000.00. Treasury Account: $7,300.00.

---

**👤 You:**
> "List all outgoing transactions over $1,000 from last week."

**🤖 AI Agent:**
> Found 3 outgoing transactions over $1,000 (Apr 15 - Apr 22): 1) AWS (Amazon Web Services): -$2,450.00 (Apr 20). 2) Stripe Payout Reversal: -$1,200.00 (Apr 18). 3) Office Rent (WeWork): -$4,500.00 (Apr 15).

---

**👤 You:**
> "Get total revenue received this month."

**🤖 AI Agent:**
> Total incoming transactions (April): 42. Total Volume: $45,890.00. Top sources: Stripe Payouts ($38,400.00), Wire from Acme Corp ($5,000.00), ACH from John Doe ($2,490.00).


## ❓ FAQ

**Q: Can I view balances and recent transactions?**
Yes. You can query balances for all accounts and list recent incoming/outgoing transactions.

**Q: How does Mercury authentication work?**
Mercury uses a Bearer token (API Token) against `api.mercury.com/api/v1`. Tokens must be generated with read-only scopes.

**Q: Can I initiate money transfers via the API?**
The standard API token allows read-only access to balances and transactions for security reasons.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mercury-alternative](https://vinkius.com/mcp/mercury-alternative)
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
3. Set Type to "SSE", enter `mercury-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mercury** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mercury-alternative": {
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
