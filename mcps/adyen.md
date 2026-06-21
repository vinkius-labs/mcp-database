# Adyen MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adyen)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Global payment processing — manage payments, refunds, and merchant accounts via AI.

## Description
Connect your **Adyen** account to your AI agent to unlock enterprise-grade payment orchestration and financial management. From monitoring real-time transaction statuses to handling refunds and auditing merchant account configurations, your agent handles your global payment ecosystem through natural conversation.

### What you can do

- **Payment Monitoring** — List and retrieve details for authorized, captured, or refused payments across your accounts
- **Refund & Modification** — Initiate refunds and manage payment modifications (captures, cancels) directly from chat
- **Merchant Oversight** — List and audit your merchant accounts and their technical configurations via the Management API
- **Payment Method Auditing** — Retrieve and verify available payment methods for specific regions and currencies
- **Financial Insights** — Quickly identify transaction trends and reconciliation patterns directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Adyen API Key and Merchant Account ID
3. Start managing your global payments and monitoring performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Operations** — automate refund processing and payment status audits effortlessly
- **E-commerce Managers** — monitor checkout health and verify payment method availability on the fly
- **Customer Support** — check payment details and transaction history to resolve billing inquiries quickly
- **Developers** — verify API integration and inspect payment responses using simple commands


## Available Tools (4)
- **get_payment_details**: Requires the 16-digit PSP reference.

Retrieve the full technical authorization and capture metadata for a specific Adyen payment
- **refund_payment**: Always double-check the amount before processing. Requires original PSP reference.

Initiate a full or partial refund for a previously captured payment in Adyen
- **list_merchants**: g. US, EU regions) and find a required Merchant ID.

Retrieve all active merchant accounts associated with your Adyen company profile
- **get_merchant_details**: Retrieve the technical configuration and status for a specific Adyen merchant account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adyen** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the status of payment with PSP reference '8816123456789012'."

**🤖 AI Agent:**
> I've retrieved the details for PSP reference 8816123456789012. The payment was successfully 'Captured' on March 30th for an amount of $50.00. Would you like to see the settlement details?

---

**👤 You:**
> "Refund $25.00 for PSP reference '8516123456789012'."

**🤖 AI Agent:**
> I've initiated a partial refund of $25.00 for PSP reference 8516123456789012. The request has been received by Adyen and is currently 'Received'. You will be notified via webhook when it is processed.

---

**👤 You:**
> "List all my active merchant accounts."

**🤖 AI Agent:**
> I've retrieved your merchant accounts. You have 3 active accounts: 'EcomStore_US', 'EcomStore_EU', and 'RetailPOS_UK'. Would you like to check the available payment methods for any of them?


## ❓ FAQ

**Q: How do I find my Adyen API Key?**
Log in to your Adyen Customer Area, go to **Developers** > **API credentials**, and select your web service user (ws@Company.YourCompany). You can generate and copy your API key from the 'Authentication' section.

**Q: Can I process a refund via the agent?**
Yes! Use the `refund_payment` tool and provide the original PSP reference and the amount. Your agent will submit the refund request to Adyen for processing.

**Q: Does this support checking payment statuses?**
Yes, the `get_payment_details` tool allows you to retrieve the full technical response for any PSP reference, including authorization codes and refusal reasons.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adyen](https://vinkius.com/mcp/adyen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Adyen** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `adyen` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Adyen** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adyen": {
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
