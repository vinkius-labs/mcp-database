# Everyware Payments & Messaging MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/everyware-payments-messaging)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Equip your AI agent to manage payments, track digital invoices, and monitor SMS messages via the Everyware API.

## Description
Integrate **Everyware**, the powerful platform for payments and messaging, directly into your AI workflow. Manage your payment transactions and digital invoices, track SMS and digital messages, monitor real-time delivery statuses and contact records, and oversee your entire customer communication and billing process using natural language.

### What you can do

- **Payment Oversight** — List and retrieve detailed information, amounts, and transaction statuses for all your processed payments.
- **Message Intelligence** — Monitor SMS and digital messages, resolving recipient details and real-time delivery status codes.
- **Invoice Management** — Access and monitor digital invoices and pay-by-text requests, tracking due dates and completion statuses.
- **Operations Auditing** — Retrieve high-level summaries of payment volume, message activity, and organizational account health instantly.

### How it works

1. Connect the Everyware integration to your AI assistant.
2. Authorize using your Everyware REST API Key (found in your account settings).
3. Orchestrate your payment collection and customer messaging strategy through intuitive conversation.

### Who is this for?

- **Accounts Receivable Teams** — Quickly check payment statuses and outstanding invoices on the go.
- **Customer Support Leads** — Research message delivery logs and contact details via chat during troubleshooting.
- **Operations Teams** — Monitor payment volumes and organizational Everyware metadata instantly.


## Available Tools (10)
- **get_everyware_account_metadata**: Retrieve metadata and limits for your Everyware account
- **get_message_delivery_status**: Get detailed delivery status and information for a specific message
- **get_payment_volume_summary**: Retrieve a high-level summary of payment volume and success rates
- **get_payment_detailed_data**: Get detailed settings and information for a specific payment
- **quick_everyware_operations_audit**: Retrieve a high-level summary of payments, messages, and contacts
- **list_customer_contacts**: List all customer contacts registered in your Everyware account
- **list_digital_invoices**: List all digital invoices and pay-by-text requests
- **list_sent_messages**: List all SMS and digital messages sent via the Everyware platform
- **list_successfully_paid_transactions**: Identify payments that have reached a "Paid" or "Captured" status
- **list_processed_payments**: List all payments processed via Everyware


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Everyware Payments & Messaging** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all payments processed today."

**🤖 AI Agent:**
> I've found 12 payments processed today, including $250 from 'John Miller' and $1,200 from 'Alice Connor'. All are currently in 'Paid' status. Would you like to see the payment method breakdown?

---

**👤 You:**
> "Show me the delivery status for message ID 'MSG-12345'."

**🤖 AI Agent:**
> Message ID 'MSG-12345' (Recipient: +15550199) has been successfully 'Delivered'. It was dispatched at 10:30 AM via Verizon. Should I pull the associated contact history?

---

**👤 You:**
> "What is our payment success rate for this month?"

**🤖 AI Agent:**
> Your current payment success rate is 98.5%. Out of 450 total transactions, 443 were successful and 7 failed. The total volume processed is $52,000. Would you like a list of the failed transaction IDs for follow-up?


## ❓ FAQ

**Q: How do I get an Everyware API Key?**
Log in to your Everyware dashboard, navigate to **Settings > API**, and you can generate or retrieve your unique **REST API Key** from there. Ensure your account is enabled for API access.

**Q: Can the agent send new payment links?**
This integration currently focuses on listing and auditing payments, invoices, and messages. Creating or sending new pay-by-text links or digital invoices should be managed via the Everyware dashboard or automated billing triggers.

**Q: Does the integration show real-time delivery status?**
Yes, you can use the get_message_delivery_status tool to retrieve the latest carrier-level status for any message sent through the Everyware platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/everyware-payments-messaging](https://vinkius.com/mcp/everyware-payments-messaging)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Everyware Payments & Messaging** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `everyware-payments-messaging` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Everyware Payments & Messaging** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "everyware-payments-messaging": {
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
