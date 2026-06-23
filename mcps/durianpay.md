# Durianpay MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/durianpay)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Equip your AI agent to manage payments, track checkout orders, and monitor settlements via the Durianpay API.

## Description
Integrate **Durianpay**, the fully integrated payment platform, directly into your AI workflow. Manage your inbound payments and transactions, track checkout orders and payment links, monitor customer profiles and interaction history, and oversee your payment settlements using natural language.

### What you can do

- **Payment Oversight** — List and retrieve detailed information and processing status for all your received transactions.
- **Order Intelligence** — Monitor checkout orders, including line items, expiration settings, and active payment links.
- **Customer Management** — Track registered customer profiles, contact details, and lifetime transaction counts across your organization.
- **Revenue Auditing** — Retrieve high-level summaries of payment activity, success rates, and identified failed transactions instantly.

### How it works

1. Connect the Durianpay integration to your AI assistant.
2. Authorize using your Durianpay Secret API Key (found in your platform settings).
3. Orchestrate your payment gateway operations and revenue analysis through intuitive conversation.

### Who is this for?

- **Finance Managers** — Quickly check daily transaction volumes and success rates on the go.
- **E-commerce Operations** — Monitor checkout order statuses and customer payments via chat.
- **Support Teams** — Research specific payment details and customer history to assist with billing inquiries instantly.


## Available Tools (10)
- **get_durianpay_account_metadata**: Retrieve metadata and usage limits for your Durianpay account
- **get_payment_order_details**: Get detailed information for a specific checkout order
- **get_payment_details**: Get detailed information and lifecycle status for a specific payment
- **quick_revenue_health_audit**: Retrieve a high-level summary of payment activity and success rates
- **list_registered_customers**: List all customers registered in your Durianpay organization
- **list_failed_transactions**: Identify payments that were declined or failed (mock logic)
- **list_payment_orders**: List all checkout orders created in your Durianpay account
- **list_durianpay_payments**: List all payments received in your Durianpay account
- **list_latest_transactions**: Identify the most recently received payments
- **search_payment_orders**: Search for orders using an order ID or customer name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Durianpay** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the latest payments received."

**🤖 AI Agent:**
> I've found 5 recent payments, including IDR 150,000 from 'John Doe' and IDR 500,000 from 'Alice Smith'. All are currently 'Completed'. Would you like to see the payment method for any of these?

---

**👤 You:**
> "Show me the details for order 'ORD-9988'."

**🤖 AI Agent:**
> Order 'ORD-9988' is currently 'Awaiting Payment'. It contains 2 items with a total amount of IDR 750,000. The checkout link expires in 2 hours. Should I pull the customer contact information?

---

**👤 You:**
> "Check for any failed transactions today."

**🤖 AI Agent:**
> I've identified 2 failed payments today: one declined by the bank (IDR 200,000) and one expired checkout. Would you like me to pull the detailed error codes for the declined payment?


## ❓ FAQ

**Q: How do I get a Durianpay API Key?**
Log in to your Durianpay dashboard, navigate to **Settings > API Keys**, and you can find your unique Secret API Key there. Ensure you use the live key for production data.

**Q: Can the agent initiate refunds?**
This integration currently focuses on listing and auditing payments and orders. Processing refunds should be managed via the Durianpay dashboard or specific refund API endpoints.

**Q: Which payment methods are tracked?**
Durianpay tracks various methods including Virtual Accounts, E-wallets, Credit Cards, and Retail outlets. The agent can retrieve the specific method used for each transaction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/durianpay](https://vinkius.com/mcp/durianpay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Durianpay** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `durianpay` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Durianpay** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "durianpay": {
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
