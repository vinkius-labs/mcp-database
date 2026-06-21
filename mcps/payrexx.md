# Payrexx MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/payrexx)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/payrexx-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/payrexx-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Accept payments online with a Swiss payment gateway that supports local and international methods with PCI compliance built in.

## Description
Connect your **Payrexx** account to any AI agent and take full control of your payment orchestration and checkout flows through natural conversation. Payrexx is the leading payment provider in Switzerland and Europe, and this integration allows you to create payment gateways, monitor real-time transaction metadata, and manage recurring subscriptions directly from your chat interface.

### What you can do

- **Gateway & Link Orchestration** — Create custom payment gateways and multi-use payment links programmatically to ensure your sales flow is always synchronized.
- **Transaction Lifecycle Management** — Access and monitor real-time transaction statuses and retrieve detailed financial metadata directly from the AI interface to track revenue health.
- **Subscription & Recurring Control** — Manage recurring billing cycles and list active subscriptions via natural language to drive better customer retention.
- **Payout & Invoice Oversight** — Access organizational payouts and list invoices to maintain a clear overview of your cash flow using simple AI commands.
- **Operational Monitoring** — Track system responses and manage webhook metadata to ensure your automation workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Payrexx Instance Name and API Secret from your merchant settings
3. Start managing your payment operations from Claude, Cursor, or any MCP-compatible client

No more manual status checks in the dashboard. Your AI acts as a dedicated payments coordinator or finance coordinator.

### Who is this for?

- **Swiss & European Merchants** — quickly retrieve payment summaries and monitor transaction status without switching apps.
- **Finance Operations Teams** — automate the retrieval of payout metadata and track organizational billing via natural conversation.
- **Developers** — integrate real-time payment data and gateway management directly within the chat.


## Available Tools
- **check_api_status**: Verify API connectivity and signature
- **create_gateway**: Create a new payment gateway (hosted payment page)
- **get_gateway**: Get details of a specific gateway
- **get_transaction**: Get details of a specific transaction
- **list_gateways**: List all payment gateways
- **list_invoices**: List invoices
- **list_payment_methods**: List available payment methods
- **list_payouts**: List payouts
- **list_subscriptions**: List recurring subscriptions
- **list_transactions**: List recent transactions
- **list_webhooks**: List configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Payrexx** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a payment link for 50.00 CHF titled 'Event Registration'."

**🤖 AI Agent:**
> I've generated your payment gateway for 'Event Registration' (50.00 CHF). You can share this link with your customers: [link]. Should I monitor this for new transactions?

---

**👤 You:**
> "Show me all payment transactions from the last 48 hours with their statuses."

**🤖 AI Agent:**
> 32 transactions processed in the last 48 hours. 28 completed successfully (CHF 12,450 total), 2 are pending 3D Secure verification, 1 was declined (insufficient funds), and 1 was refunded. Payment methods: TWINT (45%), credit card (35%), PostFinance (15%), PayPal (5%). Average transaction value: CHF 389.

---

**👤 You:**
> "Create a new payment link for a CHF 250 consultation fee with an expiration date of June 30th."

**🤖 AI Agent:**
> Payment link created successfully. Amount: CHF 250.00. Purpose: Consultation Fee. Link: pay.payrexx.com/p/abc123. Expiration: June 30, 2025. Accepted methods: TWINT, Visa, Mastercard, PostFinance. The link supports 3D Secure and is ready to be shared with your client via email or messaging.


## Installation & Usage

To install and use the **Payrexx** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/payrexx](https://vinkius.com/mcp/payrexx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
