# ThriveCart MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thrivecart)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your ThriveCart sales and products — audit transactions and subscriptions via AI.

## Description
Empower your AI agent to orchestrate your entire checkout ecosystem with **ThriveCart**, the world's easiest-to-use cart platform. By connecting ThriveCart to your agent, you transform complex sales management into a natural conversation. Your agent can instantly list your products, audit recent transactions, and retrieve subscription details without you ever touching a dashboard. Whether you are selling digital courses, physical products, or subscription services, your agent acts as a real-time sales manager, ensuring your revenue data is always accessible and organized.

### What you can do

- **Sales Auditing** — List all recent and historical transactions, and retrieve detailed metadata for each sale.
- **Product Oversight** — List all products, upsells, and coupons in your account to maintain a structured catalog.
- **Subscription Management** — Query active and cancelled subscriptions, and retrieve specific customer billing details instantly.
- **Customer Administration** — List your customers and monitor their purchase history to understand lifetime value.
- **Account Auditing** — Quickly retrieve account-wide sales data to maintain strict organizational control.

### How it works

1. Subscribe to this server
2. Enter your ThriveCart API Key
3. Start managing your sales and products through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Owners** — monitor daily sales and transaction details straight from your workflow.
- **Marketing Leads** — verify if coupons and upsells are being correctly applied and tracked.
- **Customer Support** — perform rapid transaction audits and verify subscription statuses without manual dashboard logins.
- **Operations Managers** — automate sales querying to orchestrate your e-commerce growth smoothly.


## Available Tools (10)
- **get_product**: Get details for a specific product
- **get_transaction**: Get details for a specific transaction
- **get_customer**: Get details for a specific customer
- **get_subscription**: Get details for a specific subscription
- **list_coupons**: List all coupons
- **list_customers**: List ThriveCart customers
- **list_products**: List all ThriveCart products
- **list_subscriptions**: List all subscriptions
- **list_transactions**: List recent transactions
- **list_upsells**: List all upsells


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ThriveCart** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my top 5 recent transactions in ThriveCart."

**🤖 AI Agent:**
> I've retrieved your recent sales. You have 5 new transactions, including a $97 purchase for 'Masterclass AI' by john@doe.com. Would you like the full details for any of them?

---

**👤 You:**
> "Show me all my active products."

**🤖 AI Agent:**
> I've found 3 active products in your account: 'Course X', 'Ebook Y', and 'Consulting Z'. I can provide pricing and upsell info for each if you like.

---

**👤 You:**
> "Check if there are any new subscriptions today."

**🤖 AI Agent:**
> I've scanned your subscriptions. You have 2 new recurring agreements started today for 'VIP Program'. Both are currently in active status.


## ❓ FAQ

**Q: How do I find my ThriveCart API Key?**
Log in to your ThriveCart account, go to **Settings** > **API & Webhooks** > **API Keys**, and you will find your API Key there. Copy and paste it into the field below.

**Q: Can the agent list my active subscriptions?**
Yes. Use the `list_subscriptions` tool to retrieve all ongoing billing agreements. You can also filter by specific customer or status to audit your recurring revenue.

**Q: Is it possible to see transaction details via the agent?**
Yes. The `get_transaction` tool allows your agent to fetch complete metadata for a specific sale, including amount, currency, and customer info.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thrivecart](https://vinkius.com/mcp/thrivecart)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ThriveCart** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `thrivecart` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ThriveCart** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thrivecart": {
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
