# Zuora MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zuora)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage subscriptions, billing accounts, and unified orders on Zuora — the leading monetization platform for the subscription economy.

## Description
Connect your **Zuora** account to any AI agent and manage your enterprise monetization infrastructure through natural conversation.

### What you can do

- **Subscription Lifecycle** — List all active and historical subscriptions for any account and retrieve deep details including rate plan charges
- **Billing Account Management** — Create new billing accounts, retrieve full account metadata, and update customer profiles directly from your agent
- **Unified Orders** — Create and manage complex Zuora Orders for subscriptions, renewals, or amendments using structured JSON payloads
- **Product Catalog Discovery** — Browse your entire billable product catalog and available rate plans to understand your monetization inventory
- **Invoice Auditing** — List and monitor all generated invoices for a specific account to track billing history and payment requirements
- **Billing Engine Simulation** — Preview subscription charges and generate quotes to verify billing logic before committing any changes
- **Deep Discovery** — Quickly find unique account, subscription, and order IDs required for automated revenue operations workflows

### How it works

1. Subscribe to this server
2. Enter your Zuora API Access Key ID, Secret Access Key, and REST Host
3. Start managing your subscription monetization through Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex billing dashboards to verify a charge. Your AI agent becomes your monetization operations coordinator.

### Who is this for?

- **Revenue Operations (RevOps)** — monitor subscription lifecycles and audit order details through simple chat commands
- **Billing Analysts** — reconcile invoices and preview subscription charges without manual data entry
- **Finance Teams** — verify customer billing account metadata and monitor account standings through conversation
- **Developers** — test Zuora Order payloads and verify product catalog configurations rapidly


## Available Tools
- **create_account**: Create a new billing account
- **create_order**: Create a Zuora unified Order
- **get_account**: Get account details
- **get_invoices**: Get invoices for an account
- **get_order**: Get order details
- **get_subscription**: Get subscription details
- **list_products**: List product catalog
- **list_subscriptions**: List account subscriptions
- **preview_subscription**: Preview subscription charges
- **update_account**: Update account details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zuora** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active subscriptions for account ID 'acc-123'."

**🤖 AI Agent:**
> I found 2 active subscriptions for acc-123: 1. 'SaaS Premium' (No: S-00001, Status: Active), 2. 'API Add-on' (No: S-00002, Status: Active). Would you like to see the rate plan details for either of these?

---

**👤 You:**
> "Show me the last 3 invoices for 'Acme Corp'."

**🤖 AI Agent:**
> Retrieving invoices for Acme Corp (acc-456)... The last 3 invoices are: 1. INV-001 ($1,250.00, Status: Paid), 2. INV-002 ($1,250.00, Status: Posted), and 3. INV-003 ($1,250.00, Status: Posted). Would you like me to pull the PDF download link for any of these?

---

**👤 You:**
> "Preview the charges for subscription 'S-00001'."

**🤖 AI Agent:**
> Billing simulation for S-00001 complete. The projected charge for the next period (2026-04-01 to 2026-05-01) is $1,250.00 plus tax. No amendments were detected. Would you like me to generate a formal quote?


## ❓ FAQ

**Q: Can I preview how much a customer will be charged before updating their subscription?**
Yes. The `preview_subscription` tool simulates a run of the billing engine for a specific subscription ID. Your AI agent will return the projected charges and billing dates without committing any actual changes to the account.

**Q: How do I see the invoice history for a specific billing account?**
You can use the `get_invoices` tool. Provide the unique Zuora account ID or number, and your agent will retrieve a list of all invoices generated for that customer, helping you audit their billing history.

**Q: Is it possible to update a customer's billing contact info via chat?**
Absolutely. Using the `update_account` tool, you can provide a JSON payload with updated fields (e.g., billing email or address) for a specific account ID, and your agent will apply the changes in Zuora instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zuora](https://vinkius.com/mcp/zuora)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zuora** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zuora` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zuora** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zuora": {
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
