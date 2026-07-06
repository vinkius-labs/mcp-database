# Recharge MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/recharge)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Automate subscription commerce via Recharge — manage subscriptions, customers, and orders directly from any AI agent.

## Description
Connect your **Recharge** account to any AI agent and simplify your subscription management and recurring billing workflows through natural conversation.

### What you can do

- **Subscription Management** — List all active and cancelled subscriptions, retrieve detailed metadata, and update parameters programmatically
- **Customer Database** — Query your database of subscribers and retrieve detailed profile and billing info
- **Order Tracking** — Monitor processed subscription orders and stay on top of your fulfillment pipeline
- **Financial Insights** — Access processed charges and billing history to understand your recurring revenue
- **Direct Control** — Modify subscription quantities and scheduled charge dates without manual dashboard navigation

### How it works

1. Subscribe to this server
2. Enter your Recharge API Access Token from your store settings
3. Start managing your subscription commerce from Claude, Cursor, or any MCP-compatible client


## Available Tools (11)
- **get_customer**: Get details for a specific customer
- **get_order**: Get details for a specific order
- **list_products**: List all subscription products
- **get_subscription_details**: Get details for a specific subscription
- **list_shipping_addresses**: List customer addresses
- **list_billing_charges**: List billing charges
- **list_customers**: List Recharge customers
- **list_subscription_orders**: List processed orders
- **list_subscriptions**: List Recharge subscriptions
- **update_subscription**: Update an existing subscription
- **cancel_subscription**: Cancel a subscription


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recharge** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active subscriptions in Recharge."

**🤖 AI Agent:**
> I've retrieved your subscriptions. You have 50 active subscriptions, including 'Premium Coffee Plan' and 'Monthly Supplement Pack'.

---

**👤 You:**
> "Show me all active subscriptions that are due for renewal in the next 7 days."

**🤖 AI Agent:**
> 142 subscriptions due for renewal within 7 days. Tomorrow: 23 renewals ($4,567 total). Wednesday: 31 renewals ($6,234). Thursday-Sunday: 88 renewals ($18,900). Top products: "Monthly Coffee Box" (45 renewals), "Protein Pack" (34), "Wellness Bundle" (28). 8 subscriptions have failed payment methods that need updating. 3 customers requested skipping their next delivery. Total projected renewal revenue: $29,701.

---

**👤 You:**
> "Show me the churn analysis for the last 30 days with cancellation reasons."

**🤖 AI Agent:**
> 89 cancellations in the last 30 days (4.2% churn rate, down from 5.1% last month). Reasons: "Too expensive" (34%), "No longer needed" (22%), "Switching to competitor" (18%), "Product quality" (12%), "Delivery issues" (8%), "Other" (6%). Average subscription length before cancellation: 4.7 months. Revenue lost: $12,340. 23 cancellations were win-back eligible. 8 customers paused instead of cancelling after retention offers.


## ❓ FAQ

**Q: Can I list all my active subscriptions using my AI agent?**
Yes! Use the `list_subscriptions` tool to retrieve a comprehensive list of all active and cancelled subscriptions in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/recharge](https://vinkius.com/mcp/recharge)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recharge** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recharge` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recharge** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recharge": {
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
