# Afterpay MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/afterpay)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Buy Now, Pay Later orchestration — manage checkouts, payments, and refunds via AI.

## Description
Connect your **Afterpay (Clearpay)** merchant account to your AI agent to unlock enterprise-grade BNPL (Buy Now, Pay Later) orchestration. From creating secure checkout tokens to monitoring payment statuses and processing partial refunds, your agent handles your financial transactions through natural conversation.

### What you can do

- **Checkout Orchestration** — Create new checkout sessions and retrieve secure redirect tokens for your customers
- **Payment Monitoring** — List and audit historical payments, check capture statuses, and retrieve technical metadata
- **Refund Management** — Initiate full or partial refunds for specific orders directly from your chat interface
- **Configuration Audit** — Retrieve merchant-specific configuration including minimum and maximum order limits
- **Transaction Insights** — Quickly identify successful captures or pending authorizations without manual dashboard exports

### How it works

1. Subscribe to this server
2. Enter your Afterpay Merchant ID and Secret Key
3. Start managing your BNPL transactions and monitoring performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Operations** — automate refund processing and audit transaction logs effortlessly
- **E-commerce Managers** — monitor checkout health and verify order limit configurations on the fly
- **Customer Support Teams** — quickly look up payment statuses and order history to resolve billing inquiries
- **Developers** — verify API integration and inspect payment responses using simple commands


## Available Tools (5)
- **get_afterpay_config**: Retrieve the minimum and maximum order transaction limits enforced by your Afterpay merchant account
- **create_checkout**: The amount must fall within the configured limits.

Initiate a secure Afterpay BNPL payment session token for a customer transaction
- **list_payments**: Retrieve historical BNPL transactions and authorizations securely from your Afterpay account
- **get_payment_details**: Retrieve detailed financial status, settlement info, and logs for a specific Afterpay order ID
- **refund_payment**: Always verify the remaining balance before refunding.

Initiate a full or partial refund to immediately credit a consumer against a previously captured Afterpay order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Afterpay** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create an Afterpay checkout session for $100.00."

**🤖 AI Agent:**
> I've initiated the checkout session for $100.00. Here is your checkout token and the redirect URL for the customer: https://portal.afterpay.com/checkout/...

---

**👤 You:**
> "Check the status of order ID '12345678'."

**🤖 AI Agent:**
> I've retrieved the details for order 12345678. The payment status is 'APPROVED' and it was captured on March 30th. Would you like to see the settlement details?

---

**👤 You:**
> "Show me my current Afterpay order limits."

**🤖 AI Agent:**
> I've retrieved your merchant configuration. Your minimum order amount is $1.00 and your maximum limit per transaction is $2,000.00. These apply to both US and Canada regions.


## ❓ FAQ

**Q: How do I find my Afterpay Merchant credentials?**
Log in to your Afterpay Merchant Portal, go to **Settings** > **API**. You can generate and retrieve your **Merchant ID** and **Secret Key** there. Make sure to choose the correct region (US, AU, UK).

**Q: Can I process a partial refund via the agent?**
Yes! Use the `refund_payment` tool and provide the `orderId` and the specific amount. Your agent will submit the partial refund request to Afterpay for processing.

**Q: What is the difference between Capture and Auth?**
'Capture' finalizes the payment immediately. 'Auth' (Authorization) holds the funds on the customer's account, and you must call the capture tool later (usually when shipping) to finalize the transaction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/afterpay](https://vinkius.com/mcp/afterpay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Afterpay** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `afterpay` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Afterpay** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "afterpay": {
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
