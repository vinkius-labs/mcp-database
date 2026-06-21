# Blink Payment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blink-payment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage payments, customers, and paylinks seamlessly using Blink Payment with AI Agents.

## Description
Empower your AI Agent with the full capability of Blink Payment. Blink Payment for AI Agents allows you to fully automate your financial operations directly from your isolated workspace.

### What you can do

* **Automate Payments**: Instantly list your recent payments, view detailed information, and even initiate refunds.
* **Generate Payment Intents**: Create precise and quick payment intents and link them directly to customers without leaving your conversational flow.
* **Customer Management**: Effortlessly create new customer profiles, fetch their details, and keep track of your customer base directly through your agent.
* **Paylinks on the Fly**: Generate reusable paylinks to share with clients, accelerating the checkout and invoice resolution processes.

### How it works

1. Secure your **Blink Payment** API credentials from your developer dashboard.
2. Add the API Key and Secret Key into the secure vault of your agent's platform.
3. Instruct your AI to generate a paylink, list recent successful transactions, or refund a specific payment ID.

### Who is it for?

* **Finance & Billing Teams**: Rapidly retrieve transaction data and reconcile accounts using natural language.
* **Sales & Support**: Generate customized paylinks during a support call or sales pitch instantly.
* **Developers**: Eliminate manual dashboard checks and automate your billing operations via AI-driven commands.


## Available Tools
- **create_customer**: Create a customer
- **create_paylink**: Create a paylink
- **create_payment_intent**: Create a payment intent
- **get_customer**: Get customer details by ID
- **get_paylink**: Get paylink details by ID
- **get_payment**: Get payment details by ID
- **list_customers**: List customers
- **list_paylinks**: List paylinks
- **list_payments**: List recent payments
- **refund_payment**: Refund a payment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blink Payment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my 5 most recent payments."

**🤖 AI Agent:**
> Here are your 5 most recent payments retrieved from Blink Payment.

---

**👤 You:**
> "Generate a paylink for 150 GBP for 'Consulting Services'."

**🤖 AI Agent:**
> I have created the paylink for 150 GBP. Here is the URL you can share with your client.

---

**👤 You:**
> "Refund the full amount for payment ID 'pay_12345'."

**🤖 AI Agent:**
> The payment 'pay_12345' has been successfully refunded.


## ❓ FAQ

**Q: Can the AI Agent process a direct credit card charge?**
No, for security reasons and PCI compliance, the agent uses Payment Intents and Paylinks. The end user still securely completes the payment.

**Q: Does this MCP integration support partial refunds?**
Yes, you can instruct the AI to refund a specific amount. If no amount is provided, the transaction is fully refunded.

**Q: Can I use the agent to mass-delete my customer base?**
No, destructive mass operations are not exposed to the AI agent to prevent accidental data loss in your Blink Payment account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blink-payment](https://vinkius.com/mcp/blink-payment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blink Payment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `blink-payment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blink Payment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blink-payment": {
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
