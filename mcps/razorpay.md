# Razorpay MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/razorpay)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate online payments via Razorpay — manage orders, payments, and refunds directly from any AI agent.

## Description
Connect your **Razorpay** account to any AI agent and take full control of your payment orchestration through natural conversation. Razorpay is India's leading payments solution, and this integration allows you to retrieve payment metadata, create customer orders, and manage financial transactions directly from your chat interface.

### What you can do

- **Order & Payment Orchestration** — List all managed orders and retrieve detailed metadata, including creating new payment orders programmatically.
- **Transaction Lifecycle Management** — Access and monitor payment statuses and retrieve technical metadata directly from the AI interface to ensure successful checkouts.
- **Customer CRM Control** — List and search through your customer database to maintain accurate records via natural language.
- **Subscription & Invoice Intelligence** — Access recurring billing plans and monitor invoice statuses to ensure your revenue streams are always optimized.
- **Operational Monitoring** — Track settlements, transfers, and retrieve account profile metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Razorpay Key ID and Key Secret from your dashboard
3. Start managing your payment operations from Claude, Cursor, or any MCP-compatible client

No more manual status checking or spreadsheet transaction logs. Your AI acts as a dedicated payments specialist or finance coordinator.

### Who is this for?

- **E-commerce Merchants** — quickly retrieve payment details and monitor order fulfillment without switching apps.
- **Finance Operations Teams** — automate the management of refunds and track settlements via natural conversation.
- **Developers** — integrate real-time payment data and transaction monitoring directly within the chat.


## Available Tools
- **create_customer**: Create a new customer
- **create_order**: Amount should be in smallest currency subunit (e.g., 50000 for ₹500.00).

Create a new payment order
- **get_order**: Get details of a specific order
- **get_payment**: Get details of a specific payment
- **list_customers**: List all customers
- **list_invoices**: List all invoices
- **list_orders**: List all payment orders
- **list_payments**: List all payments
- **list_refunds**: List all refunds
- **list_settlements**: List all settlements
- **list_subscriptions**: List all subscriptions
- **list_transfers**: List all transfers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Razorpay** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active customers in my Razorpay account."

**🤖 AI Agent:**
> I've retrieved your customers. You have 150 registered contacts. Notable recent profiles include 'John Miller' and 'Sarah Chen'. Which one would you like to see the payment history for?

---

**👤 You:**
> "Show me all payment transactions from today with their statuses and settlement details."

**🤖 AI Agent:**
> 67 transactions today totaling ₹4,23,500. Captured: 62 (₹3,98,200). Authorized but not captured: 3 (₹18,400). Failed: 2 (₹6,900, card declined). By method: UPI 45% (highest), Credit Card 28%, Debit Card 15%, Net Banking 8%, Wallets 4%. Settlement: ₹3,45,000 settled to your bank account at 4 PM. Pending settlement: ₹53,200 (next cycle tomorrow). Average transaction: ₹6,320. Refunds processed: 4 (₹12,800).

---

**👤 You:**
> "Create a new payment link for ₹15,000 for the consulting invoice with 7-day expiry."

**🤖 AI Agent:**
> Payment link created. Amount: ₹15,000. Purpose: Consulting Invoice #INV-2025-089. Short URL: rzp.io/l/cons089. Expiry: May 20, 2025. Accepted methods: UPI, Credit Card, Debit Card, Net Banking, Wallets. Partial payments: disabled. The link has been copied to your clipboard and is ready to share via email or WhatsApp. A payment receipt will be auto-generated upon successful payment.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific payment just by providing its ID?**
Yes! Use the `get_payment` tool with the Payment ID. Your agent will respond with complete metadata, including capture status, refund history, and customer notes in seconds.

**Q: How do I find my Razorpay Key ID and Key Secret?**
Log in to your Razorpay dashboard, navigate to **Settings** > **API Keys**, and generate a new key pair. You will see the Key ID immediately and must download the Key Secret.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/razorpay](https://vinkius.com/mcp/razorpay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Razorpay** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `razorpay` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Razorpay** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "razorpay": {
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
