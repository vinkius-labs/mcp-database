# GoCardless MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gocardless)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage direct debit payments, track mandates, and oversee customers via AI agents with GoCardless.

## Description
Connect your **GoCardless** merchant account to any AI agent to automate your direct debit payments and customer mandates through the Model Context Protocol (MCP). GoCardless is the global leader in bank-to-bank payments, simplifying the collection of recurring and one-off payments. This MCP server enables you to retrieve customer records, track mandate authorizations, manage payment collections, and monitor bank payouts directly through natural conversation.

### Key Features

- **Customer & Bank Oversight** — List all customers registered in your system and fetch detailed profile and bank account metadata instantly.
- **Mandate Management** — Access and track customer authorizations (mandates) to ensure you have the legal right to collect payments.
- **Payment Orchestration** — List all direct debit collections, track their status (confirmed, failed), and programmatically initiate new payments against active mandates.
- **Subscription Insights** — Retrieve active and inactive recurring payment plans to understand your predictable revenue health.
- **Payout Tracking** — Access a complete list of funds being sent from GoCardless to your own bank account for easy reconciliation.
- **Refund Visibility** — Monitor processed refunds and reversed payments to maintain an accurate financial audit trail.
- **Real-time Synchronization** — Keep your bank-to-bank payment data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GoCardless Access Token (found in Developers > Access Tokens)
3. Start managing your direct debits from Claude, Cursor, or any MCP client

### Who is this for?

- **Finance & Billing Ops** — quickly check if a mandate is active or verify if a payout has been initiated without manual portal navigation.
- **Account Managers** — get a real-time overview of a customer's payment history and subscription status via simple AI commands.
- **Operations Leads** — automate the retrieval of failed payment logs and mandate status reports seamlessly.


## Available Tools
- **verify_api_connection**: Check connection
- **create_new_payment**: Initiate a collection
- **get_account_details**: Get account identity
- **get_customer_details**: Get customer metadata
- **get_mandate_status**: Check mandate details
- **get_payment_details**: Get payment metadata
- **list_payment_customers**: List all customers
- **list_payment_mandates**: List active mandates
- **list_direct_debit_payments**: List all payments
- **list_merchant_payouts**: List bank payouts
- **list_payment_refunds**: List reversed payments
- **list_recurring_subscriptions**: List recurring plans


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GoCardless** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my payments that are currently 'pending_submission'."

**🤖 AI Agent:**
> Retrieving payments... I found 5 payments pending submission, including a $50.00 collection for customer 'Acme Corp'. Would you like the full list?

---

**👤 You:**
> "Check the status of mandate 'MD12345'."

**🤖 AI Agent:**
> Fetching mandate... Mandate MD12345 is 'Active'. It was authorized by John Doe on October 1st and is valid for both one-off and recurring payments.

---

**👤 You:**
> "Show me the last 3 payouts sent to my bank account."

**🤖 AI Agent:**
> Retrieving payouts... I found 3 recent payouts: $1,250.00 (Oct 5th), $850.00 (Oct 2nd), and $2,100.00 (Sept 28th). All have been 'Paid' successfully.


## ❓ FAQ

**Q: How do I get an Access Token for GoCardless?**
Log in to your GoCardless dashboard, navigate to Developers > Access Tokens, and you can generate a new token for either Sandbox or Live use there.

**Q: What is a 'Mandate' in GoCardless?**
A mandate is an authorization from your customer that allows you to collect payments from their bank account automatically in the future.

**Q: In what units should I provide the payment amount?**
The API uses minor units for currency. For example, to collect $1.00 USD (or £1.00 GBP), you must provide the value 100 (cents/pence).

**Q: Can I test this without using real money?**
Yes! Use the 'sandbox' environment by setting the 'Environment' credential and providing a Sandbox Access Token from your GoCardless account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gocardless](https://vinkius.com/mcp/gocardless)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GoCardless** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gocardless` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GoCardless** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gocardless": {
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
