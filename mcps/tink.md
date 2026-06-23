# Tink MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tink)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Connect to bank accounts, list transactions, and initiate payments via Tink directly from your AI agent.

## Description
Connect your **Tink** account to any AI agent to manage your open banking data and payments through natural conversation.

### What you can do

- **Account Overview** — List all connected bank accounts and retrieve their underlying details.
- **Transaction History** — Access and filter transaction records by account ID or specific date ranges for deep financial analysis.
- **Payment Initiation** — Create payment requests to specific destination accounts with custom amounts, currencies, and references.

### How it works

1. Subscribe to this server
2. Enter your Tink Access Token
3. Start managing your finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Financial Analysts** — quickly pull transaction data for reporting without manual CSV exports.
- **Developers** — test payment flows and account connectivity directly from the code editor.
- **Business Owners** — monitor cash flow and initiate transfers via simple text commands.


## Available Tools (3)
- **list_accounts**: List user bank accounts
- **create_payment_request**: Create a payment request
- **list_transactions**: List transactions for accounts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tink** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my bank accounts connected via Tink."

**🤖 AI Agent:**
> I've found 2 connected accounts: 'Main Checking' (ID: acc_8821) and 'Savings' (ID: acc_9932). Would you like to see the transactions for either of them?

---

**👤 You:**
> "Show me transactions for account acc_8821 from October 2023."

**🤖 AI Agent:**
> Fetching transactions for October... I found 12 entries. The largest was a transfer of 1,200 EUR for 'Rent'. Would you like a full breakdown?

---

**👤 You:**
> "Create a payment request of 50 EUR to Alice Smith (IBAN: DE123456789) for 'Dinner'."

**🤖 AI Agent:**
> I've initiated the payment request for 50 EUR to Alice Smith. You can track this request using the reference ID: pay_ref_5521.


## ❓ FAQ

**Q: How can I see all my connected bank accounts at once?**
You can use the `list_accounts` tool. It will retrieve a complete list of all bank accounts currently linked to your Tink profile.

**Q: Is it possible to filter my spending by specific dates?**
Yes! The `list_transactions` tool allows you to provide an optional `startDate` and `endDate` (ISO 8601) to narrow down your transaction history.

**Q: Can I initiate a bank transfer using this server?**
Yes, you can use the `create_payment_request` tool. You will need to provide the destination account number, type, amount, and recipient details to start the process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tink](https://vinkius.com/mcp/tink)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tink** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tink` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tink** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tink": {
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
