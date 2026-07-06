# Lemon Squeezy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lemon-squeezy-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Sell software, subscriptions, and digital products globally with built-in tax compliance, billing, and licensing as your merchant of record.

## Description
Connect your **Lemon Squeezy** store to any AI agent and manage digital sales through natural conversation.

### What you can do

- **Product Management** — List products with variants, pricing, and sales data
- **Order Tracking** — Browse orders with status, amounts, and customer data
- **Subscription Monitoring** — Track active subscriptions, renewals, and churn
- **Customer Database** — List customers with purchase history and LTV
- **Revenue Analytics** — Monitor MRR, refund rates, and growth trends
- **Store Management** — Access store settings, checkout links, and discount codes

### How it works

1. Subscribe to this server
2. Enter your Lemon Squeezy API Key
3. Start managing sales from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Indie Developers** — sell software and track revenue
- **SaaS Founders** — manage subscriptions and monitor MRR
- **Creators** — sell digital products and track customers


## Available Tools (12)
- **get_subscription**: Get subscription details
- **list_customers**: List all customers
- **list_discounts**: List promo codes
- **list_orders**: List all orders
- **list_products**: List all products
- **list_stores**: List all stores
- **list_subscriptions**: List all subscriptions
- **list_variants**: List all product variants
- **list_webhooks**: List configured webhooks
- **get_account_info**: Get account profile
- **get_order**: Get order details
- **get_product**: Get product details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lemon Squeezy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all products with sales data and this month's revenue."

**🤖 AI Agent:**
> Products: 4. 'Pro License' ($49/one-time, 890 sales, $43.6K). 'Team Plan' ($29/mo, 234 active subs). 'Enterprise' ($99/mo, 45 active). 'Starter Kit' ($19, 1.2K sales, $22.8K). This month: $12,400 revenue. MRR: $8,850. One-time: $3,550. Orders: 68. Refunds: 2 ($98).

---

**👤 You:**
> "Show active subscriptions and churn analysis."

**🤖 AI Agent:**
> Active subscriptions: 279. Team Plan: 234 ($6,786/mo). Enterprise: 45 ($4,455/mo). MRR: $11,241. This month: +18 new, -6 cancelled. Churn: 2.1% (excellent). Net revenue retention: 108%. Upcoming renewals (7 days): 32. At-risk (payment failed): 3.

---

**👤 You:**
> "List customers sorted by LTV and show discount codes."

**🤖 AI Agent:**
> Top customers by LTV: 1) Acme Corp — $2,376 (Enterprise, 24 months). 2) TechCo — $1,740 (Team, 5 seats, 12 months). 3) StartupXYZ — $1,188 (Enterprise, 12 months). Total customers: 1,890. Discount codes: 3 active. 'LAUNCH20' (20% off, 45 uses). 'ANNUAL30' (30% annual, 12 uses). 'PARTNER50' (50%, partner only, 3 uses).


## ❓ FAQ

**Q: Can I track subscriptions and MRR?**
Yes. Monitor active subscriptions, renewals, cancellations, churn rate, and MRR with growth trends.

**Q: Can I manage products and discount codes?**
Yes. List products with variants and pricing. Access discount codes, checkout links, and store settings.

**Q: What API does Lemon Squeezy use?**
Bearer authentication against `api.lemonsqueezy.com/v1`. JSON:API format.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lemon-squeezy-alternative](https://vinkius.com/mcp/lemon-squeezy-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lemon Squeezy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lemon-squeezy-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lemon Squeezy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lemon-squeezy-alternative": {
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
