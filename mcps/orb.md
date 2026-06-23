# Orb MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/orb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Automate usage-based billing via Orb — ingest events, manage subscriptions, and track invoices directly from any AI agent.

## Description
Connect your **Orb** account to any AI agent to streamline your revenue operations and usage-based billing workflows through natural language.

### What you can do

- **Usage Ingestion** — Send batches of usage events with idempotency keys to track consumption in real-time.
- **Subscription Lifecycle** — Create, update, and cancel subscriptions, tying customers to specific billing plans seamlessly.
- **Customer Management** — Provision new customers and list existing ones with full metadata and external ID mapping.
- **Invoicing & Revenue** — List historical invoices or fetch upcoming draft invoices to predict end-of-month billing.
- **Credit Ledgers** — Manage prepaid credits by creating ledger entries for increments, decrements, or expirations.

### How it works

1. Subscribe to this server
2. Enter your Orb API Key
3. Start managing your billing and usage data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance & RevOps** — Instantly check upcoming revenue and manage customer credits without manual dashboard exports.
- **Engineering Teams** — Debug usage ingestion and verify event delivery directly from the terminal or IDE.
- **Product Managers** — Monitor feature adoption and subscription statuses across the customer base.


## Available Tools (10)
- **cancel_subscription**: Cancel a subscription
- **create_customer**: Requires name and email.

Create a new customer in Orb
- **create_ledger_entry**: Create a ledger entry for credits
- **create_subscription**: Create a subscription for a customer
- **fetch_ledger**: Fetch credit ledger for a customer
- **get_upcoming_invoice**: Fetch upcoming invoice for a subscription
- **ingest_events**: Events require customer_id, event_name, timestamp, idempotency_key, and properties.

Ingest usage events into Orb
- **list_customers**: List customers in Orb
- **list_invoices**: List invoices
- **update_subscription**: Update an existing subscription


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Orb** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 customers created in Orb."

**🤖 AI Agent:**
> I've retrieved the latest customers. The most recent entries include 'Acme Corp' (ID: cust_821), 'Global Tech' (ID: cust_932), and 'Starlight Inc' (ID: cust_104). Would you like to see the subscription details for any of them?

---

**👤 You:**
> "Ingest a usage event for customer cust_123: 50 units of 'api_requests'."

**🤖 AI Agent:**
> Usage event successfully ingested for 'cust_123'. I've used a unique idempotency key for this batch to ensure accurate tracking. The 50 units of 'api_requests' are now reflected in their usage metrics.

---

**👤 You:**
> "What is the upcoming invoice amount for subscription sub_987?"

**🤖 AI Agent:**
> The upcoming draft invoice for subscription `sub_987` is currently at $450.00. This includes the base plan fee plus $120.00 in metered usage accrued during the current period.


## ❓ FAQ

**Q: How do I report usage events for a specific customer?**
Use the `ingest_events` tool. You'll need to provide an array of event objects containing the `customer_id`, `event_name`, `timestamp`, and an `idempotency_key` to ensure usage is only counted once.

**Q: Can I see how much a customer will be charged before the billing cycle ends?**
Yes! The `get_upcoming_invoice` tool allows you to fetch the draft invoice for any active `subscription_id`, giving you real-time visibility into accrued costs.

**Q: How do I manage prepaid credits or balances?**
You can use `create_ledger_entry` to add or remove credits from a customer's balance. You can also use `fetch_ledger` to view the current state of a customer's credit ledger.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/orb](https://vinkius.com/mcp/orb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Orb** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `orb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Orb** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "orb": {
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
