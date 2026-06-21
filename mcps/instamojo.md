# Instamojo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/instamojo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage payments, refunds, and payouts via Instamojo API.

## Description
Empower your AI agents to manage your Indian payment ecosystem with Instamojo. This MCP server allows you to list and retrieve payments, manage payment requests, track refunds, view payouts, and monitor disputes directly through the Instamojo API. Ideal for automating e-commerce operations and financial monitoring in India.


## Available Tools (10)
- **get_payment**: Retrieves details for a specific payment
- **get_payment_request**: Retrieves details for a specific payment request
- **get_refund**: Retrieves details for a specific refund
- **list_disputes**: Lists all active and past disputes
- **list_gateways**: Lists configured payment gateways
- **list_links**: Lists all generated payment links
- **list_payment_requests**: Lists all payment requests created
- **list_payments**: Lists all payments received
- **list_payouts**: Lists all payouts to your bank account
- **list_refunds**: Lists all refunds processed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Instamojo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all recent payments in Instamojo."

**🤖 AI Agent:**
> I'll fetch your recent transaction history from Instamojo.

---

**👤 You:**
> "Show me the status of my recent payment requests."

**🤖 AI Agent:**
> I'll retrieve the list of payment requests and their current statuses.

---

**👤 You:**
> "Check for any active disputes in my account."

**🤖 AI Agent:**
> I'll look up the current disputes in your account.


## ❓ FAQ

**Q: How do I get Instamojo API credentials?**
Log in to your Instamojo dashboard, navigate to API & Plugins, and find your Client ID and Client Secret in the OAuth2 section.

**Q: Does it support Sandbox mode?**
This implementation uses the production API base by default. To use sandbox, the engine URL needs to be updated.

**Q: Can I process refunds?**
This version focus on listing and retrieving refund details. Actions to trigger new refunds may be added in future updates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/instamojo](https://vinkius.com/mcp/instamojo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Instamojo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `instamojo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Instamojo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "instamojo": {
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
