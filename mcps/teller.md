# Teller MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/teller)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Connect to your bank accounts, list transactions, check balances, and initiate payments via Teller API.

## Description
Connect your **Teller** enrollment to any AI agent and manage your financial data and payments through natural conversation.

### What you can do

- **Account Management** — List all financial accounts and fetch specific metadata for any connected bank account.
- **Identity Verification** — Retrieve owner information including names, addresses, phone numbers, and emails associated with the accounts.
- **Balances & Details** — Get real-time ledger and available balances, as well as sensitive account and routing numbers.
- **Transaction History** — Query historical ledger transactions with support for pagination and date filtering.
- **Payments** — Create payees and initiate payments (e.g., via Zelle) directly from your specified accounts.
- **Access Control** — Revoke authorization for specific accounts or the entire enrollment when needed.

### How it works

1. Subscribe to this server
2. Enter your Teller Access Token, Certificate, and Private Key
3. Start managing your banking data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — integrate real-time banking data and payment flows into your AI-driven applications without building custom connectors.
- **Finance Teams** — automate transaction monitoring and balance checks across multiple institutions.
- **Personal Finance Users** — interact with your own bank data using natural language to track spending or verify account details.


## Available Tools (11)
- **get_account_balances**: Get real-time ledger and available balances
- **get_account_details**: Get account and routing numbers
- **list_accounts**: List all accounts for the enrollment
- **create_payee**: Create a new payee for an account
- **delete_account**: Delete authorization for a specific account
- **delete_all_accounts**: Delete authorization for all accounts in the enrollment
- **get_account**: Get details for a specific account
- **get_identity**: Get identity information for accounts
- **initiate_payment**: g., via Zelle) from the specified account.

Initiate a payment from an account
- **list_institutions**: List supported financial institutions
- **list_transactions**: Supports pagination and date filtering.

List ledger transactions for an account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Teller** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my connected bank accounts and their IDs."

**🤖 AI Agent:**
> I've retrieved your accounts. You have a 'Checking' account (ID: acc_123) and a 'Savings' account (ID: acc_456) connected via Chase.

---

**👤 You:**
> "What is the current balance of my account acc_123?"

**🤖 AI Agent:**
> The current ledger balance for account acc_123 is $1,250.50, with $1,200.00 available for immediate use.

---

**👤 You:**
> "Show me the identity information associated with my accounts."

**🤖 AI Agent:**
> The identity records show the accounts are owned by 'John Doe', with a registered address at 123 Finance St and email 'john@example.com'.


## ❓ FAQ

**Q: Can I retrieve my full account and routing numbers for a specific account?**
Yes. Use the `get_account_details` tool with the specific Account ID. It will return the sensitive account and routing numbers associated with that account.

**Q: Is it possible to list transactions within a specific date range?**
Absolutely. The `list_transactions` tool allows you to provide `start_date` and `end_date` parameters (in ISO 8601 format) to filter your transaction history.

**Q: Can I initiate a payment like Zelle through this integration?**
Yes. You can use `create_payee` to set up a destination and then `initiate_payment` to send funds using supported schemes like Zelle.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/teller](https://vinkius.com/mcp/teller)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Teller** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `teller` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Teller** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "teller": {
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
