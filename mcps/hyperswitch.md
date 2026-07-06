# Hyperswitch MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hyperswitch)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage payments, customers, and refunds via Hyperswitch API.

## Description
Empower your AI agents to manage your payment infrastructure with Hyperswitch. This MCP server allows you to list payments, retrieve customer details, manage refunds, track disputes, and view payouts directly through the Hyperswitch API. Ideal for automating fintech operations and payment monitoring.


## Available Tools (10)
- **get_customer**: Retrieves details for a specific customer
- **get_dispute**: Retrieves details for a specific dispute
- **get_payment**: Retrieves details for a specific payment
- **get_payout**: Retrieves details for a specific payout
- **list_customers**: Lists all customers
- **get_refund**: Retrieves details for a specific refund
- **list_disputes**: Lists all disputes
- **list_payments**: Lists all payments
- **list_payouts**: Lists all payouts
- **list_refunds**: Lists all refunds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hyperswitch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 10 payments processed through Hyperswitch."

**🤖 AI Agent:**
> I'll fetch your recent payment history from Hyperswitch.

---

**👤 You:**
> "Check for any active disputes."

**🤖 AI Agent:**
> I'll look up the current disputes in your account.

---

**👤 You:**
> "Show me the details for customer ID 'cust_123'."

**🤖 AI Agent:**
> I'll retrieve that customer's information for you.


## ❓ FAQ

**Q: How do I get Hyperswitch API credentials?**
You can find your API Secret Key in the Hyperswitch dashboard under 'API Keys'.

**Q: Does it support multiple processors?**
Hyperswitch is a payment switch that abstracts multiple processors. This MCP interacts with the Hyperswitch unified API.

**Q: Can I process refunds with this MCP?**
This version focus on listing and retrieving refund details. Actions to trigger new refunds may be added in future updates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hyperswitch](https://vinkius.com/mcp/hyperswitch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hyperswitch** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hyperswitch` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hyperswitch** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hyperswitch": {
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
