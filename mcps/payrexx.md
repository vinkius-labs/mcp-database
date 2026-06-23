# Payrexx MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/payrexx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Accept payments online with a Swiss payment gateway that supports local and international methods with PCI compliance built in.

## Description
Connect your **Payrexx** account to any AI agent and take full control of your payment orchestration and checkout flows through natural conversation. Payrexx is the leading payment provider in Switzerland and Europe, and this integration allows you to create payment gateways, monitor real-time transaction metadata, and manage recurring subscriptions directly from your chat interface.

### What you can do

- **Gateway & Link Orchestration** — Create custom payment gateways and multi-use payment links programmatically to ensure your sales flow is always synchronized.
- **Transaction Lifecycle Management** — Access and monitor real-time transaction statuses and retrieve detailed financial metadata directly from the AI interface to track revenue health.
- **Subscription & Recurring Control** — Manage recurring billing cycles and list active subscriptions via natural language to drive better customer retention.
- **Payout & Invoice Oversight** — Access organizational payouts and list invoices to maintain a clear overview of your cash flow using simple AI commands.
- **Operational Monitoring** — Track system responses and manage webhook metadata to ensure your automation workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Payrexx Instance Name and API Secret from your merchant settings
3. Start managing your payment operations from Claude, Cursor, or any MCP-compatible client

No more manual status checks in the dashboard. Your AI acts as a dedicated payments coordinator or finance coordinator.

### Who is this for?

- **Swiss & European Merchants** — quickly retrieve payment summaries and monitor transaction status without switching apps.
- **Finance Operations Teams** — automate the retrieval of payout metadata and track organizational billing via natural conversation.
- **Developers** — integrate real-time payment data and gateway management directly within the chat.


## Available Tools (11)
- **check_api_status**: Verify API connectivity and signature
- **create_gateway**: Create a new payment gateway (hosted payment page)
- **get_gateway**: Get details of a specific gateway
- **get_transaction**: Get details of a specific transaction
- **list_gateways**: List all payment gateways
- **list_invoices**: List invoices
- **list_payment_methods**: List available payment methods
- **list_payouts**: List payouts
- **list_subscriptions**: List recurring subscriptions
- **list_transactions**: List recent transactions
- **list_webhooks**: List configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Payrexx** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a payment link for 50.00 CHF titled 'Event Registration'."

**🤖 AI Agent:**
> I've generated your payment gateway for 'Event Registration' (50.00 CHF). You can share this link with your customers: [link]. Should I monitor this for new transactions?

---

**👤 You:**
> "Show me all payment transactions from the last 48 hours with their statuses."

**🤖 AI Agent:**
> 32 transactions processed in the last 48 hours. 28 completed successfully (CHF 12,450 total), 2 are pending 3D Secure verification, 1 was declined (insufficient funds), and 1 was refunded. Payment methods: TWINT (45%), credit card (35%), PostFinance (15%), PayPal (5%). Average transaction value: CHF 389.

---

**👤 You:**
> "Create a new payment link for a CHF 250 consultation fee with an expiration date of June 30th."

**🤖 AI Agent:**
> Payment link created successfully. Amount: CHF 250.00. Purpose: Consultation Fee. Link: pay.payrexx.com/p/abc123. Expiration: June 30, 2025. Accepted methods: TWINT, Visa, Mastercard, PostFinance. The link supports 3D Secure and is ready to be shared with your client via email or messaging.


## ❓ FAQ

**Q: Can my AI automatically find the status for a specific transaction by its ID?**
Yes! Use the `get_transaction` tool with the Transaction ID. Your agent will respond with complete metadata, including payment method, currency, amount, and final status in seconds.

**Q: How do I find my Payrexx API Secret and Instance Name?**
Log in to your Payrexx merchant dashboard, navigate to **Settings** > **API**, and you will find your unique secret key and instance name (e.g., yourname.payrexx.com) there.

**Q: Does this work for recurring payments?**
Absolutely. You can use the `list_subscriptions` tool to monitor active recurring billing cycles and orchestrate multi-use gateways for recurring customer payments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/payrexx](https://vinkius.com/mcp/payrexx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Payrexx** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `payrexx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Payrexx** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "payrexx": {
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
