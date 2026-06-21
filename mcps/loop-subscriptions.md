# Loop Subscriptions MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/loop-subscriptions)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Subscription management for Shopify — manage recurring orders and customers via Loop.

## Description
Empower your AI agents to handle **Loop Subscriptions** directly. This server allows you to monitor and manage recurring revenue, customer profiles, and subscription lifecycles on Shopify.

### What you can do

- **Subscription Control** — List, inspect, pause, resume, or cancel subscriptions instantly
- **Order Orchestration** — Monitor upcoming orders and skip next deliveries when requested by customers
- **Customer Management** — Access detailed profiles and subscription history for your users
- **Operational Visibility** — Track the status and health of your recurring business through simple natural language commands

### How it works

1. Subscribe to this server
2. Enter your **Loop Admin API Token**
3. Start managing your Shopify subscriptions from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **cancel_subscription**: Optional reason can be provided.

Cancel a subscription
- **get_customer**: Get customer details
- **get_subscription**: Get detailed info for a single subscription
- **list_customers**: List all customers with active or past subscriptions
- **list_orders**: List subscription orders
- **list_subscriptions**: List all Loop Subscriptions
- **pause_subscription**: You can optionally provide a resume date.

Pause an active subscription
- **resume_subscription**: Resume a paused subscription
- **skip_next_order**: Skip the next scheduled order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Loop Subscriptions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my active subscriptions."

**🤖 AI Agent:**
> Fetching subscriptions... I've found 15 active subscriptions. Here are the most recent ones...

---

**👤 You:**
> "Pause subscription #12345 until 2026-12-01."

**🤖 AI Agent:**
> Pausing subscription #12345... Success! It is now scheduled to resume on December 1st, 2026.

---

**👤 You:**
> "Skip the next delivery for customer 'John Doe'."

**🤖 AI Agent:**
> Finding John Doe's subscription... Found! Skipping the next scheduled order as requested.


## ❓ FAQ

**Q: Where can I find my Loop API Token?**
Go to your Loop Admin Portal, navigate to Settings > Manage API tokens, and generate a new token with Admin scopes.

**Q: Does this work with headless Shopify stores?**
Yes, this server uses the Admin API, which manages the subscription data regardless of the storefront implementation.

**Q: Can I resume a subscription that was cancelled?**
Generally, only 'Paused' subscriptions can be resumed. Cancelled subscriptions might need to be recreated depending on your Loop configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/loop-subscriptions](https://vinkius.com/mcp/loop-subscriptions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Loop Subscriptions** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `loop-subscriptions` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Loop Subscriptions** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "loop-subscriptions": {
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
