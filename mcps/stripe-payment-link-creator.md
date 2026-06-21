# Stripe Payment Link Creator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stripe-payment-link-creator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

This MCP does exactly one thing: it generates custom Stripe Checkout URLs on the fly for any amount negotiated in chat. That's its only function. Incredible for turning your AI into a real-time closer.

## Description
We refused to build a bloated Stripe integration that gives an AI agent terrifying access to your financial dashboard, payout history, and customer subscriptions. Instead, this MCP server provides a surgical, zero-trust bridge: **just generating a Checkout Session URL.**

Your AI agent gains the immediate ability to close deals inside a conversation. If a customer agrees to pay $150 for a custom consulting session, the agent doesn't send them to a generic pricing page—it instantly creates a unique `$150` checkout link and drops it in the chat.

### The Superpowers

- **Real-Time Closing:** End the friction of sending users to complex pricing pages. The AI negotiates the price and generates the exact payment link right then and there.
- **Zero-Bloat Integration:** No massive SDKs. It uses a direct `POST` to the Stripe `/v1/checkout/sessions` API. You only need your Stripe Secret Key.
- **Absolute Containment:** Because this is strictly a "Push-only" creation tool, the agent cannot read your Stripe dashboard, cannot issue refunds, and cannot see your bank account details. It only generates links. A completely secure, one-way funnel.


## Available Tools (1)
- **create_stripe_payment_link**: Provide the product name, the amount in cents (e.g. 5000 for $50.00), and the currency code (e.g. "usd" or "brl"). Send the resulting checkoutUrl directly to the customer.

Generates a unique Stripe Checkout Session URL for a custom amount


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stripe Payment Link Creator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a payment link for $45.00 USD for 'Priority Support Ticket'."

**🤖 AI Agent:**
> I've generated the payment link. You can complete your purchase here: https://checkout.stripe.com/c/pay/cs_test_...


## ❓ FAQ

**Q: Can the agent issue refunds or read my bank account info?**
No. This MCP only accesses the endpoint to create a Checkout Session. It does not have functions to read balances, list transactions, or issue refunds.

**Q: Do I need to create a Product in Stripe first?**
No! This MCP uses inline `price_data`. The AI generates the product name and price entirely on the fly during the conversation, so you don't need any pre-configured products in your Stripe dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stripe-payment-link-creator](https://vinkius.com/mcp/stripe-payment-link-creator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stripe Payment Link Creator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stripe-payment-link-creator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stripe Payment Link Creator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stripe-payment-link-creator": {
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
