# Mollie MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mollie-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mollie-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mollie-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Accept online payments across Europe with a payment gateway that supports iDEAL, credit cards, PayPal, and local methods seamlessly.

## Description
Connect your **Mollie** account to any AI agent and manage European payments through natural conversation.

### What you can do

- **Payment Management** — Create, list, and inspect payments with full status details
- **Refund Tracking** — Browse all processed refunds
- **Customer Management** — List registered customers for recurring billing
- **Subscriptions** — View active and cancelled subscriptions per customer
- **Payment Methods** — List all enabled payment methods (iDEAL, Bancontact, cards, etc.)

### How it works

1. Subscribe to this server
2. Enter your Mollie API Key
3. Start managing payments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce** — automate payment creation and status tracking
- **Finance Teams** — monitor refunds and reconciliation
- **Developers** — integrate European payment methods


## Available Tools
- **create_payment**: Create a new payment
- **get_payment_details**: Get details for a specific payment
- **list_customers**: List Mollie customers
- **list_payment_methods**: List available payment methods
- **list_payments**: List Mollie payments
- **list_refunds**: List all refunds
- **list_customer_subscriptions**: List subscriptions for a customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mollie** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List recent payments and their statuses."

**🤖 AI Agent:**
> Recent payments: 5. 1) €45.00 — 'Pro Plan Monthly' (Status: Paid ✅, iDEAL). 2) €120.00 — 'Annual License' (Status: Paid ✅, Credit Card). 3) €25.00 — 'Addon Purchase' (Status: Open ⏳). 4) €10.00 — 'Donation' (Status: Expired ❌). 5) €89.00 — 'Enterprise Upgrade' (Status: Paid ✅, Bancontact).

---

**👤 You:**
> "Create a payment of €50 for a premium upgrade."

**🤖 AI Agent:**
> Payment created! ✅ ID: tr_7UhSN1zuXS. Amount: €50.00. Description: 'Premium Upgrade'. Checkout URL: https://www.mollie.com/checkout/... Redirect URL: https://myapp.com/success. Status: Open. Waiting for customer to pay.

---

**👤 You:**
> "Show enabled payment methods and list refunds."

**🤖 AI Agent:**
> Enabled methods: 6. iDEAL ✅, Credit Card ✅, Bancontact ✅, PayPal ✅, SEPA Direct Debit ✅, Klarna ✅. Refunds (last 30 days): 3. 1) €12.00 (tr_abc, Refunded ✅). 2) €45.00 (tr_def, Processing). 3) €8.50 (tr_ghi, Refunded ✅).


## Installation & Usage

To install and use the **Mollie** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mollie-alternative](https://vinkius.com/mcp/mollie-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
