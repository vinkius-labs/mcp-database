# Uscreen MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uscreen)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Launch your own video streaming service with membership management, mobile apps, and monetization tools for content creators.

## Description
Connect your **Uscreen** account to any AI agent and manage your video membership business.

### What you can do

- **Customer Management** — List all customers and view detailed profiles
- **Content Library** — Browse and inspect videos and courses
- **Collection Organization** — List and view content collections
- **Subscription Plans** — View all membership plans and pricing
- **Product Catalog** — Browse available products for purchase
- **Revenue Tracking** — List all payment transactions


## Available Tools (10)
- **check_uscreen_status**: Verify API connectivity
- **get_collection**: Get collection details
- **get_content**: Get content details
- **get_customer**: Get customer details
- **list_collections**: List collections
- **list_content**: List all content
- **list_customers**: List all customers
- **list_products**: List products
- **list_subscriptions**: List subscriptions
- **list_transactions**: List transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Uscreen** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Uscreen customers."

**🤖 AI Agent:**
> You have 1,234 customers. Active: 987, Churned: 247. Top recent signup: 'Jane D.' (Premium plan, joined today).

---

**👤 You:**
> "Show all subscription plans."

**🤖 AI Agent:**
> 3 plans: 'Basic' (.99/mo, 312 subscribers), 'Premium' (.99/mo, 489 subscribers), 'VIP' (.99/mo, 186 subscribers).

---

**👤 You:**
> "List all payment transactions."

**🤖 AI Agent:**
> 247 transactions this month. Total revenue: ,450. Average transaction: .40. Top: Premium renewals (67%).


## ❓ FAQ

**Q: Can my AI list all customers and their subscriptions?**
Yes. `list_customers` returns all customers, and `get_customer` shows detailed profile including subscription status.

**Q: Can I view revenue transactions?**
Yes. `list_transactions` returns all payment transactions with amounts, dates, and customer info.

**Q: How do I browse my content library?**
Use `list_content` to see all videos and courses, then `get_content` for detailed metadata on any item.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uscreen](https://vinkius.com/mcp/uscreen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Uscreen** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uscreen` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Uscreen** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uscreen": {
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
