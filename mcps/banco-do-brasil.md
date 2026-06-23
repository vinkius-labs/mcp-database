# Banco do Brasil MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/banco-do-brasil)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Check balance, statements, pay Pix/Boleto, and manage your BB account via API.

## Description
Connect your **Banco do Brasil** account to any AI agent and perform essential banking tasks — check balances, view transaction history, send Pix payments, and pay bills through natural conversation.

### What you can do
- **Account Details** — View agency, account number, and available limits
- **Balances** — Check available funds and credit limits instantly
- **Statement** — Retrieve transaction history by date range
- **Pix Payments** — Send instant transfers using any Pix key (CPF, Email, Phone)
- **Boleto Payments** — Pay utility bills and barcodes
- **Pix History** — View all sent and received Pix transfers
- **Credit Card** — View credit card invoices and totals

### How it works
1. Subscribe to this server
2. Enter your OAuth2 Access Token from the BB Developers Portal
3. Start managing your finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **BB Customers** — Automate their daily banking tasks via AI
- **Developers** — Integrate BB banking capabilities into financial apps and bots
- **Business Owners** — Monitor account activity and pay suppliers automatically


## Available Tools (9)
- **get_accounts**: Usually returns one active account.

Get list of checking accounts
- **get_balance**: Get current account balance and limits
- **create_pix**: Send a Pix payment to a key
- **get_credit_card_invoices**: Get credit card invoices
- **pay_barcode**: Pay a barcode/boleto bill
- **pay_utility_bill**: Pay a utility bill via barcode
- **get_pix_history**: Type can be RECEIVED or SENT.

Get history of Pix transfers (Sent/Received)
- **get_scheduled_payments**: Get scheduled future payments
- **get_statement**: Dates in YYYY-MM-DD format.

Get account statement (transactions) by date range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Banco do Brasil** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my current balance."

**🤖 AI Agent:**
> Available Balance: R$ 2,500.00 | Credit Limit: R$ 500.00

---

**👤 You:**
> "Send a Pix of R$50 to joao@email.com."

**🤖 AI Agent:**
> Pix sent successfully! End-to-End ID: E1234567890123456789012345678901.

---

**👤 You:**
> "Show me the transactions from last week."

**🤖 AI Agent:**
> Found 5 transactions: 1. R$ -50.00 (Pix Sent). 2. R$ 2,000.00 (Salary Received).


## ❓ FAQ

**Q: How do I get an Access Token for Banco do Brasil?**
You must create a Developer account on [**BB Developers Portal**](https://developers.bb.com.br), create an App, and use your Certificate (mTLS) and Client ID/Secret to generate the Access Token via OAuth2.

**Q: Can I pay bills and Pix?**
Yes! Use the `pay_barcode` or `create_pix` actions. You will need a valid token with payment permissions.

**Q: Does it work for companies (CNPJ)?**
Yes, the BB APIs support both Individual (CPF) and Business (CNPJ) accounts, provided your token has the correct scope.

**Q: Are the API connections secure?**
Absolutely. Banco do Brasil requires mTLS certificates and secure environments for their API connections to ensure financial-grade safety.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/banco-do-brasil](https://vinkius.com/mcp/banco-do-brasil)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Banco do Brasil** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `banco-do-brasil` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Banco do Brasil** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "banco-do-brasil": {
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
