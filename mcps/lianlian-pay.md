# LianLian Pay MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lianlian-pay)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Global cross-border payment and settlement platform — manage balances, payments, and settlements via AI.

## Description
Empower your AI agent to orchestrate your international financial infrastructure with **LianLian Pay**, the premier cross-border payment platform for enterprise global trade. By connecting LianLian Pay to your agent, you transform complex settlement tracking, fund collections, and multi-currency management into a natural conversation. Your agent can instantly list your balances, retrieve transaction details, monitor fund settlements, and even initiate refund requests without you ever needing to navigate the comprehensive LianLian Global portal. Whether you are managing cross-border e-commerce revenue or coordinating international supplier payments, your agent acts as a real-time global treasury assistant, keeping your data accurate and your settlements moving.

### What you can do

- **Balance Orchestration** — Retrieve real-time balance information across your LianLian merchant accounts.
- **Payment Management** — Create and track payment orders with full support for unique identifiers and status queries.
- **Settlement Monitoring** — Browse historical settlements and fund withdrawals to track your capital flow.
- **Transaction Auditing** — Filter and retrieve detailed transaction records for financial reconciliation.
- **Treasury Insights** — Retrieve current FX exchange rates and supported bank lists for efficient fund management.

### How it works

1. Subscribe to this server
2. Enter your LianLian Merchant ID and RSA Private Key
3. Start managing your global settlements through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Directors** — monitor organization-wide liquidity and audit global settlements through natural language.
- **Treasury Operations** — coordinate payments and track fund withdrawals directly from your AI-powered workspace.
- **E-commerce Enterprises** — manage cross-border revenue and reconcile transactions via a unified AI interface.
- **Logistics & Trade Partners** — integrate international payment status tracking into your automated workflows.


## Available Tools
- **create_payment**: Create a new payment
- **get_account_info**: Get merchant account info
- **get_balance**: Get account balance
- **get_bank_list**: Get supported banks
- **get_exchange_rates**: Get current FX rates
- **list_settlements**: List settlements
- **list_transactions**: List transactions
- **list_withdrawals**: List fund withdrawals
- **query_order**: Query order status
- **refund_order**: Refund a payment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LianLian Pay** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current balance on LianLian Pay?"

**🤖 AI Agent:**
> I've retrieved your account balances. You have a total available balance of $120,500 USD and €15,200 EUR. Would you like a breakdown of pending settlements?

---

**👤 You:**
> "Check the status of order 'LL-ORDER-8821'."

**🤖 AI Agent:**
> The order 'LL-ORDER-8821' is currently 'Completed'. The payment was successfully collected at 10:30 AM today. Funds are scheduled for settlement in 2 business days.

---

**👤 You:**
> "List the last 5 settlements for my merchant account."

**🤖 AI Agent:**
> I've listed your 5 most recent settlements. The largest was for $45,000 on April 8th. Total settled amount for this week is $112,000. Should I check for any failed withdrawal attempts?


## ❓ FAQ

**Q: How do I find my LianLian Merchant ID?**
Your Merchant ID is an 18-digit number starting with '14', provided by LianLian Pay after your account is successfully registered and verified. You can find it in the LianLian Global portal dashboard.

**Q: How do I set up the RSA keys for API calls?**
Generate a 2048-bit RSA key pair. Upload your Public Key to the LianLian Global portal under [Developer Settings]. Use your Private Key in the credentials section of this server to sign requests.

**Q: Can I initiate a refund through the agent?**
Yes. Use the `refund_order` tool with the original order ID and the refund amount. Your agent will initiate the request with LianLian Pay and monitor the processing status for you.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lianlian-pay](https://vinkius.com/mcp/lianlian-pay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LianLian Pay** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `lianlian-pay` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LianLian Pay** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lianlian-pay": {
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
