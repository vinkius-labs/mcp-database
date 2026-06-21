# Stripe Payment Link Creator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stripe-payment-link-creator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/stripe-payment-link-creator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/stripe-payment-link-creator-mcp)
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


## Available Tools
- **create_stripe_payment_link**: Provide the product name, the amount in cents (e.g. 5000 for $50.00), and the currency code (e.g. "usd" or "brl"). Send the resulting checkoutUrl directly to the customer.

Generates a unique Stripe Checkout Session URL for a custom amount


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stripe Payment Link Creator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a payment link for $45.00 USD for 'Priority Support Ticket'."

**🤖 AI Agent:**
> I've generated the payment link. You can complete your purchase here: https://checkout.stripe.com/c/pay/cs_test_...


## Installation & Usage

To install and use the **Stripe Payment Link Creator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stripe-payment-link-creator](https://vinkius.com/mcp/stripe-payment-link-creator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
