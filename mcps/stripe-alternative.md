# Stripe MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stripe-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage payments, customers, products and subscriptions via Stripe — create payment intents, track invoices and audit refunds from any AI agent.

## Description
Connect your **Stripe** account to any AI agent and take full control of your payment infrastructure through natural conversation.

### What you can do

- **Customer Management** — List, retrieve and create customers with email, name and metadata
- **Product & Pricing** — Browse products and their prices (one-time and subscription) with currency and amount details
- **Payment Tracking** — Monitor payment intents with status (succeeded, pending, failed) and associated customers
- **Charge & Refund Audit** — Review all charges and refunds with amounts, statuses and timestamps
- **Subscription Oversight** — Track active subscriptions, their billing cycles and associated prices
- **Invoice Review** — List invoices with amounts due, status (draft, paid, open) and customer details
- **Balance Monitoring** — Check available and pending balances across currencies
- **Coupon Management** — List discount coupons with percent-off, amount-off and duration settings

### How it works

1. Subscribe to this server
2. Enter your Stripe Secret Key
3. Start managing your payments from Claude, Cursor, or any MCP-compatible client

No more switching to the Stripe dashboard to check a payment status or audit refunds. Your AI acts as a dedicated payments engineer.

### Who is this for?

- **Finance Teams** — quickly check balances, review invoices and audit refunds without opening the Stripe dashboard
- **Developers** — create payment intents, list customers and inspect product pricing without leaving your IDE
- **Product Managers** — monitor subscription statuses, track customer growth and review coupon usage via conversation


## Available Tools
- **create_customer**: Optionally set the email, name and description. Returns the created customer with its ID.

Create a new Stripe customer
- **create_payment_intent**: Requires the amount (in smallest currency unit, e.g. cents for USD) and currency (e.g. "usd"). Optionally associate with a customer. Returns the payment intent with its client_secret for use with Stripe.js.

Create a new payment intent in Stripe
- **get_balance**: Returns available and pending balances broken down by currency and type (card, bank_transfer, etc.). Useful for checking your Stripe payout status.

Get current Stripe account balance
- **get_customer**: Provide the customer ID (starts with "cus_").

Get details for a specific Stripe customer
- **list_charges**: Each charge has an ID, amount, currency, status (succeeded, pending, failed), customer, payment method and creation date. Optionally filter by customer and set a limit.

List charges in Stripe
- **list_coupons**: Each coupon has an ID, name, percent_off or amount_off, duration (once, repeating, forever) and active status. Optionally set a limit.

List coupons in Stripe
- **list_customers**: Each customer has an ID, email, name, description and metadata. Optionally filter by email to find a specific customer and set a limit on the number of results returned.

List customers in Stripe
- **list_invoices**: Each invoice has an ID, customer, amount due, status (draft, open, paid, uncollectible), creation date and line items. Optionally filter by customer and set a limit.

List invoices in Stripe
- **list_payment_intents**: Each intent has an ID, amount, currency, status (requires_payment_method, requires_confirmation, requires_action, processing, succeeded, canceled) and associated customer. Optionally filter by customer and set a limit.

List payment intents in Stripe
- **list_prices**: Each price has an ID, unit amount, currency, recurring interval (if subscription) and associated product. Optionally filter by product ID, active status and limit.

List prices in Stripe
- **list_products**: Each product has an ID, name, description, images and active status. Products are used with Prices to define what you sell. Optionally filter by active status and set a limit.

List products in Stripe
- **list_refunds**: Each refund has an ID, amount, charge ID, status (succeeded, pending, failed, canceled) and creation date. Optionally set a limit.

List refunds in Stripe
- **list_subscriptions**: Each subscription has an ID, customer, status (trialing, active, past_due, canceled, unpaid, incomplete), items (prices) and billing cycle details. Optionally filter by customer, status and set a limit.

List subscriptions in Stripe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stripe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active subscriptions and their monthly revenue."

**🤖 AI Agent:**
> I found 47 active subscriptions. Total monthly recurring revenue is $12,450. The largest plan is the Enterprise tier at $499/mo (3 customers), followed by Pro at $99/mo (18 customers) and Starter at $29/mo (26 customers).

---

**👤 You:**
> "Show me all refunds issued in the last 30 days."

**🤖 AI Agent:**
> I found 8 refunds in the last 30 days totaling $347.50. The largest was $149.00 for charge ch_3Oa... (Annual Plan cancellation). All others were under $50 each. Would you like the details for any specific refund?

---

**👤 You:**
> "What's my current Stripe balance?"

**🤖 AI Agent:**
> Your available balance is $8,234.50 USD and €1,120.00 EUR. Pending balance: $2,450.00 USD (3 payment intents still processing). Next payout is scheduled for tomorrow.


## ❓ FAQ

**Q: How do I get my Stripe Secret Key?**
Log in to the [**Stripe Dashboard**](https://dashboard.stripe.com/apikeys), go to **Developers > API keys**, toggle **Test mode** for testing or stay in Live mode for production. Copy the Secret Key (starts with `sk_test_` or `sk_live_`). Keep it secret — never expose it in frontend code.

**Q: What's the difference between a payment intent and a charge?**
A **Payment Intent** represents a pending payment that may require additional steps (3D Secure, confirmation). It tracks the lifecycle of a payment attempt. A **Charge** is the result of a successfully completed payment — it represents money that has been collected. Use list_payment_intents to track in-progress payments and list_charges for completed ones.

**Q: Can I create a payment intent for any amount?**
Yes! Use the `create_payment_intent` tool with the amount in the smallest currency unit (e.g. 1000 = $10.00 USD, 1000 = €10.00 EUR) and the currency code (usd, eur, gbp, etc.). Optionally associate it with a customer ID. The tool returns the payment intent with its client_secret for use with Stripe.js.

**Q: Can I track subscription statuses?**
Yes! Use `list_subscriptions` to see all subscriptions with their status (active, trialing, past_due, canceled, unpaid), customer, billing cycle and items. You can filter by customer ID or status to narrow results. This is useful for monitoring recurring revenue and identifying at-risk accounts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stripe-alternative](https://vinkius.com/mcp/stripe-alternative)
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
3. Set Type to "SSE", enter `stripe-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stripe** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stripe-alternative": {
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
