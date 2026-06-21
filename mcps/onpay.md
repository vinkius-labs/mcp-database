# OnPay MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/onpay)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Payroll and HR management — manage employees, transactions, and schedules via OnPay.

## Description
Connect your **OnPay** account to empower your AI agents with payroll and HR capabilities. This server provides programmatic access to the **OnPay API**, allowing for seamless management of employee profiles, payment transactions, and recurring pay schedules.

### What you can do

- **Employee Directory** — List and inspect complete employee profiles and records
- **Transaction Monitoring** — Access historical payment transactions and statuses in real-time
- **Payroll Orchestration** — Monitor upcoming pay schedules and cycles for your company
- **Subscription Tracking** — View active and past subscriptions managed through the platform
- **Accounting Integration** — Retrieve item codes and company settings for financial reconciliation

### How it works

1. Subscribe to this server
2. Enter your **OnPay API Token** from your management panel
3. Start managing your payroll operations from Claude, Cursor, or any MCP client


## Available Tools (8)
- **get_company_info**: Get general company information
- **get_employee**: Get employee details
- **get_transaction**: Get transaction details
- **list_employees**: List all employees
- **list_item_codes**: List accounting item codes
- **list_pay_schedules**: List payroll schedules
- **list_subscriptions**: List subscriptions
- **list_transactions**: List payment transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OnPay** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active employees."

**🤖 AI Agent:**
> Fetching employees... I've found 15 active employees. Here are the first few...


## ❓ FAQ

**Q: How do I get an OnPay API Token?**
Log in to your OnPay management panel, and navigate to Settings > API to generate a static API token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/onpay](https://vinkius.com/mcp/onpay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OnPay** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `onpay` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OnPay** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "onpay": {
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
