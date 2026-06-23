# Recurly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/recurly-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Automate subscription billing and management via Recurly — manage subscriptions, accounts, and invoices directly from any AI agent.

## Description
Connect your **Recurly** account to any AI agent and simplify your subscription billing, revenue management, and customer orchestration through natural conversation.

### What you can do

- **Subscription Management** — List all active and expired product subscriptions, and retrieve detailed metadata and plan info
- **Account Coordination** — Query your database of billing accounts and retrieve detailed metadata, balance, and status
- **Billing Tracking** — Access a history of generated invoices and monitor their payment status directly from your agent
- **Plan catalog** — Query available subscription plans and their pricing to choose the right context for each interaction
- **Direct Enrollment** — Register new customer accounts programmatically directly from your agent

### How it works

1. Subscribe to this server
2. Enter your Recurly API v3 Key from your account settings
3. Start managing your subscription commerce from Claude, Cursor, or any MCP-compatible client


## Available Tools (11)
- **get_invoice**: Get details for a specific invoice
- **get_revenue_summary**: Get revenue export dates
- **list_coupons**: List all active coupons
- **list_transactions**: List recent transactions
- **create_billing_account**: Register a new account
- **get_account_details**: Get details for a specific account
- **get_subscription_details**: Get details for a specific subscription
- **list_billing_accounts**: List billing accounts
- **list_billing_invoices**: List invoices
- **list_subscription_plans**: List available plans
- **list_subscriptions**: List Recurly subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recurly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active subscriptions in Recurly."

**🤖 AI Agent:**
> I've retrieved your subscriptions. You have 10 active subscriptions, including 'Premium Plan' and 'Standard Tier'.

---

**👤 You:**
> "Show me the subscription revenue breakdown by plan for the current billing period."

**🤖 AI Agent:**
> Revenue by plan this billing period. "Enterprise Annual" leads with $234,000 (42% of total, 78 subscribers). "Professional Monthly" at $156,000 (28%, 520 subscribers). "Starter Monthly" at $89,000 (16%, 1,780 subscribers). "Team Annual" at $67,000 (12%, 134 subscribers). "Free Trial" has 234 active trials, 34% conversion rate. Total MRR: $546,000. Growth vs last period: +8.2%. 12 enterprise accounts renewed this month with an average 15% uplift.

---

**👤 You:**
> "List all failed invoice payments from the last 14 days that need follow-up."

**🤖 AI Agent:**
> 34 failed payments in the last 14 days totaling $18,200. By reason: Card declined (18), Insufficient funds (9), Expired card (5), Network error (2). Retry status: 12 recovered after automatic retry (35% recovery). 22 still outstanding. High-value failures: Acme Corp $2,400 (card expired), TechVentures $1,800 (declined). 8 accounts are past the 3rd retry attempt and need manual outreach. Dunning emails sent: 67 total, 23% updated their payment method.


## ❓ FAQ

**Q: Can I list all my active subscriptions using my AI agent?**
Yes! Use the `list_subscriptions` tool to retrieve a comprehensive list of all subscriptions registered in your Recurly account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/recurly-alternative](https://vinkius.com/mcp/recurly-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recurly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recurly-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recurly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recurly-alternative": {
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
