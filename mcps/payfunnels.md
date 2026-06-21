# Payfunnels MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/payfunnels)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Build payment funnels and checkout experiences that maximize conversions with upsells, order bumps, and subscription options.

## Description
Connect your **Payfunnels** account to any AI agent and take full control of your billing orchestration and payment collection through natural conversation. Payfunnels provides a simplified platform for accepting payments online, and this integration allows you to create payment links, monitor active subscriptions, and process refunds directly from your chat interface.

### What you can do

- **Payment Link Orchestration** — Create one-time or recurring payment links programmatically to ensure your sales checkout is always synchronized.
- **Subscription Lifecycle Management** — Access and monitor active recurring subscriptions and retrieve detailed billing metadata directly from the AI interface to track revenue consistency.
- **Transaction & Refund Control** — List all processed payments and trigger refunds for specific transactions via natural language to drive better customer satisfaction.
- **Fee & Charge Intelligence** — Access and manage setup fees and service-related charges to maintain a clear overview of your organizational pricing using simple AI commands.
- **Operational Monitoring** — Track system responses and manage account profile metadata to ensure your payment operations are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Payfunnels External API Key from your dashboard integration settings
3. Start managing your checkouts from Claude, Cursor, or any MCP-compatible client

No more manual logging into dashboards to check payment status. Your AI acts as a dedicated billing coordinator or payments lead.

### Who is this for?

- **Service Providers & Coaches** — quickly retrieve payment summaries and monitor subscriber growth without switching apps.
- **Finance Operations Teams** — automate the management of recurring billing and track refund history via natural conversation.
- **Sales Teams** — streamline the creation of custom payment links and monitor deal closures directly within the chat.


## Available Tools (12)
- **cancel_subscription**: Cancel a recurring subscription
- **create_setup_fee**: Requires a name.

Create a new setup fee
- **create_one_time_payment_link**: Requires title and amount.

Create a one-time payment link
- **create_recurring_payment_link**: Requires title and amount.

Create a subscription payment link
- **get_current_user**: Get authenticated user profile
- **get_payment_details**: Get details for a specific payment
- **get_subscription_details**: Get details for a subscription
- **list_setup_fees**: List setup fees
- **list_payments**: List all payments
- **list_service_fees**: List service fees
- **list_subscriptions**: List all active subscriptions
- **refund_payment**: Refund a specific payment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Payfunnels** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a one-time payment link for $50 labeled 'Setup Fee'."

**🤖 AI Agent:**
> I've generated your payment link for the 'Setup Fee' ($50.00). You can share this URL with your customer: [link]. Would you like me to track when this is paid?

---

**👤 You:**
> "Show me all payment funnels and their conversion rates for the current month."

**🤖 AI Agent:**
> You have 5 active payment funnels this month. "Premium Upgrade" converts at 34% with $47,200 in revenue (412 checkouts started, 140 completed). "Annual Plan Offer" converts at 28% generating $89,100. "Addon Upsell" has the highest rate at 52% but lower volume ($12,400). Total funnel revenue: $178,300 across 892 successful transactions.

---

**👤 You:**
> "Get the detailed transaction history and refund status for funnel Premium Upgrade."

**🤖 AI Agent:**
> "Premium Upgrade" funnel details: 412 checkouts initiated, 140 completed (34% conversion), 272 abandoned. Revenue: $47,200. Refunds: 3 processed totaling $1,011 (2.1% refund rate). Average order value: $337. Payment methods: Credit Card 78%, PayPal 18%, Apple Pay 4%. Peak conversion hour: 2 PM EST.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific payment by its ID?**
Yes! Use the `get_payment` tool with the Payment ID. Your agent will respond with complete metadata, including amount, status, customer info, and transaction date in seconds.

**Q: How do I find my Payfunnels External API Key?**
Log in to your Payfunnels dashboard, navigate to **Billing** > **Integration**, find the 'Payfunnels API Key' section, and click 'Generate' to see your unique secret key.

**Q: Can I process a partial refund via the AI?**
The current `refund_payment` tool processes the full transaction amount. For partial refunds, we recommend using the main Payfunnels dashboard until support is added to the API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/payfunnels](https://vinkius.com/mcp/payfunnels)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Payfunnels** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `payfunnels` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Payfunnels** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "payfunnels": {
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
