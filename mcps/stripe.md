# Stripe MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stripe)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage payments, customers, subscriptions, invoices, and account balance via Stripe — all from any AI agent.

## Description
Take full control of your payment operations with **Stripe**, the global payments platform trusted by millions of businesses. Your AI agent becomes your financial operations assistant — listing customers, checking payment statuses, reviewing subscriptions, pulling invoices, and monitoring your account balance.

### What you can do

- **Customer Management** — List, search, and create customers with names, emails, and metadata.
- **Payment Tracking** — Monitor payment intents with status, amounts, and currency across all transactions.
- **Subscription Overview** — Check active, past-due, and canceled subscriptions with billing intervals and plan details.
- **Invoice Monitoring** — Review open, paid, and overdue invoices with hosted payment links.
- **Account Balance** — Instantly check available and pending balances across all currencies.

### How it works

1. Subscribe to this server
2. Enter your Stripe Secret Key (from Dashboard → Developers → API keys)
3. Start querying your Stripe data from Claude, Cursor, or any MCP client

### Who is this for?

- **Finance Teams** — audit payments, reconcile subscriptions, and chase overdue invoices from a single conversation.
- **SaaS Founders** — monitor MRR, track customer churn, and review billing status without opening the Stripe dashboard.
- **Support Teams** — quickly look up customer payment status and share invoice links during support tickets.


## Available Tools
- **customers_list**: Optionally filter by email. Returns customer details including name, email, balance, and delinquency status.

List Stripe customers
- **refunds_list**: List Stripe refunds
- **customers_create**: Name and email are required. Returns the created customer with their Stripe ID.

Create a new Stripe customer
- **payments_list**: Optionally filter by customer ID. Amounts are in the smallest currency unit (e.g., 1000 = $10.00).

List Stripe payment intents
- **subscriptions_list**: Optionally filter by customer or status.

List Stripe subscriptions
- **invoices_list**: Optionally filter by customer or status (draft, open, paid, uncollectible, void).

List Stripe invoices
- **balance_get**: Shows available and pending amounts by currency. Amounts are in smallest currency unit (divide by 100 for dollars).

Get Stripe account balance
- **products_list**: Use to browse your product offerings.

List Stripe products
- **product_create**: Use before creating prices.

Create a new Stripe product
- **prices_list**: Filter by product to see all price tiers.

List Stripe prices
- **refund_create**: Specify amount in cents for partial refunds.

Create a refund for a payment
- **charges_list**: Filter by customer ID.

List Stripe charges
- **payouts_list**: List Stripe payouts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stripe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show my Stripe account balance."

**🤖 AI Agent:**
> Your Stripe balance: **$12,450.80 available** and **$3,200.00 pending** in USD.

---

**👤 You:**
> "List all past-due subscriptions."

**🤖 AI Agent:**
> Found 3 past-due subscriptions. The largest is for Acme Corp ($299/month, overdue since March 15). Would you like me to pull the associated invoices?

---

**👤 You:**
> "Create a new customer: Jane Smith, jane@example.com"

**🤖 AI Agent:**
> Customer created: **Jane Smith** (cus_QR7x...). Email: jane@example.com. Ready for invoicing and subscriptions.


## ❓ FAQ

**Q: How do I get started with Stripe MCP?**
Subscribe, then go to the **Stripe Dashboard → Developers → API keys** and copy your Secret key (starts with sk_live_ or sk_test_ for testing). Paste it here and you're ready. No SDK, no server setup, no webhooks — just connect and start querying your payment data.

**Q: Can my AI agent track subscription churn and billing status?**
Yes. Ask your agent to list all subscriptions filtered by status — 'show me all past-due subscriptions' or 'how many canceled subscriptions do we have this month?'. It returns billing intervals, plan amounts, and whether the subscription will cancel at period end. Perfect for SaaS MRR monitoring.

**Q: How do I check if a customer's payment went through?**
Just ask — 'check recent payments for customer cus_abc123' or 'did John's payment go through?'. Your agent pulls the latest payment intents showing the amount, currency, and status (succeeded, requires_action, or failed). No need to log into the Stripe dashboard or refresh browser tabs.

**Q: Can I manage customers and invoices for my entire team?**
Absolutely. Create new customers with name, email, and notes in a single command. List all invoices filtered by customer or status — open, paid, or overdue. Share hosted invoice URLs directly from the conversation. Perfect for finance teams, SaaS billing departments, and e-commerce operations managing hundreds of customer accounts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stripe](https://vinkius.com/mcp/stripe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stripe** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `stripe` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stripe** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stripe": {
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
