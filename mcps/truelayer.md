# TrueLayer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/truelayer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage open banking payments, payouts, and account data via TrueLayer — initiate transfers, check balances, and list transactions directly from any AI agent.

## Description
Connect your **TrueLayer** account to any AI agent to automate financial operations and open banking workflows through natural conversation.

### What you can do

- **Payments & Payouts** — Create instant bank transfers, process payouts, and handle refunds with full control over currency and beneficiaries.
- **Merchant Accounts** — List and inspect your TrueLayer-managed merchant accounts, check balances, and monitor transaction history.
- **Open Banking Data** — Retrieve real-time account balances, transaction lists, and verify account ownership from connected banks.
- **Recurring Payments** — Set up and manage Variable Recurring Payment (VRP) mandates for automated billing and subscriptions.
- **Provider Discovery** — List available banking providers and verify credentials across supported regions.

### How it works

1. Subscribe to this server
2. Enter your TrueLayer Access Token
3. Start managing your fintech operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fintech Developers** — Test and integrate payment flows directly from your code editor without switching to a browser.
- **Finance Teams** — Monitor merchant account balances and reconcile transactions through simple conversational queries.
- **Operations Managers** — Automate payouts and refunds to customers using a dedicated AI financial assistant.


## Available Tools
- **create_mandate**: Create a Variable Recurring Payment (VRP) mandate
- **create_payment**: Requires amount, currency, payment method, beneficiary, and user details.

Create a new single payment
- **create_payout**: Can be closed-loop or open-loop.

Create a new payout
- **create_refund**: Cannot exceed the original payment amount.

Create a refund for a payment
- **get_data_account_balance**: Get balance for a data account
- **get_merchant_account**: Get details for a specific merchant account
- **list_data_account_transactions**: List transactions for a data account
- **list_data_accounts**: Requires user consent token.

List user bank accounts (Data API)
- **list_merchant_account_transactions**: List transactions for a merchant account
- **list_merchant_accounts**: List TrueLayer merchant accounts
- **list_payment_sources**: List payment sources for a merchant account
- **list_providers**: List supported bank providers
- **verify_account**: Verify account ownership


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TrueLayer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my merchant accounts and their current status."

**🤖 AI Agent:**
> I've retrieved your merchant accounts. You have 3 active accounts: 'Main GBP' (ID: acc_01), 'Euro Operations' (ID: acc_02), and 'Savings' (ID: acc_03). Would you like to see the balance for any of these?

---

**👤 You:**
> "Create a payment of £25.50 for user 'John Doe'."

**🤖 AI Agent:**
> I'm initiating a payment of 2550 minor units (GBP). I'll need the beneficiary details and payment method to complete the `create_payment` request. Should I use your default merchant account as the beneficiary?

---

**👤 You:**
> "Show me the last 5 transactions for account acc_01."

**🤖 AI Agent:**
> Fetching transaction history for acc_01... I found 5 recent transactions, including a payment of £100.00 from 'User A' and a payout of £50.00 to 'User B'. Would you like the full details of the most recent one?


## ❓ FAQ

**Q: Can I issue a refund for a specific payment using this server?**
Yes! Use the `create_refund` tool by providing the `payment_id` and the `amount_in_minor` (e.g., 100 for £1.00). The agent will process the repayment against the original transaction.

**Q: How do I check the current balance of my connected bank accounts?**
You can use the `get_data_account_balance` tool with a specific `account_id` to retrieve real-time balance information directly from the bank via TrueLayer's Data API.

**Q: Does this integration support setting up recurring payments?**
Yes. The `create_mandate` tool allows you to set up Variable Recurring Payment (VRP) mandates, enabling automated and flexible recurring transfers from your users.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/truelayer](https://vinkius.com/mcp/truelayer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TrueLayer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `truelayer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TrueLayer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "truelayer": {
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
