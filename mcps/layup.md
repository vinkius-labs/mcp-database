# Layup MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/layup)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage digital lay-by orders, track deposits, and fetch checkout customer data via Layup straight from your AI agent.

## Description
Connect your **Layup** operational account to any AI agent and manage lay-by e-commerce checkout infrastructures effortlessly.

### What you can do

- **Order Metrics** — List all captured lay-by checkouts and inspect target order data instantly
- **Track Payments** — Check the deposit status, timeline, and pending metrics on Layup checkouts
- **Customer Data** — Cross-reference buyer metrics with internal logs
- **Store Automation** — Programmatically create new virtual lay-bys dynamically based on AI discussions

### How it works

1. Subscribe to this server
2. Enter your Layup Merchant API Key
3. Start fetching and creating installments right from Claude or Cursor

### Who is this for?

- **E-Commerce Operators** — check if an installment was completely matched directly via chat
- **Support Teams** — quickly check customer balances and order logs organically
- **Developers** — audit tracking and debugging logs directly from within your IDE


## Available Tools (9)
- **cancel_order**: Void an existing Layup order
- **create_deposit**: Register a new lay-by deposit manually
- **create_order**: Initialize a new lay-by order
- **get_customer**: Retrieve customer explicit parameters
- **get_order**: Get parameters surrounding an explicit order
- **get_payment**: Fetch targeted payment details
- **list_customers**: Read globally saved shopper customers
- **list_orders**: Retrieve active lay-by payment plan orders
- **list_payments**: Retrieve all payments linked to an order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Layup** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find order ID 900 and tell me its completion balance."

**🤖 AI Agent:**
> Understood. Fetching from your Layup module... Order 900 holds a remaining balance of 20.00ZAR with status set as Incomplete.

---

**👤 You:**
> "Fetch all recorded incoming deposits."

**🤖 AI Agent:**
> Connecting to API... You have 15 recent deposit lines mapped over your active lay-bys in the last window.

---

**👤 You:**
> "Search for customer details on the Layup platform."

**🤖 AI Agent:**
> Querying customer list... Retrieved 3 profiles. Should I filter by email?


## ❓ FAQ

**Q: How do I get started?**
Subscribe, enter your API credentials (your secret token from **Layup Dashboard → Developer Settings → API Keys**), and you're ready. No code, no environment files, no endpoints — just connect and start managing your orders through your AI agent.

**Q: Can my AI agent check the remaining balance on an active order?**
Yes! Provide the Order target ID to the agent. It utilizes the `get_order` tool returning exact metrics on money received vs pending values. It aggregates everything in conversational format so you don't jump windows.

**Q: What happens when I need to create a manual dynamic lay-by in chat?**
Just specify the item price, customer token, and configuration. The AI agent executes a `create_order` action connecting via the payload and creates proper links. The shopper gets billed correctly, saving you minutes of UI clicking.

**Q: Can I query an exact list of all historically recorded buyers/customers?**
Absolutely. Ask the agent to list all stored customers. It compiles email arrays, reference ID trackers, phone tags — perfect for store leads and analysts evaluating buyer records without exporting flat files.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/layup](https://vinkius.com/mcp/layup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Layup** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `layup` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Layup** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "layup": {
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
