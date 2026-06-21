# Alipay Open Platform MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alipay-open-platform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/alipay-open-platform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/alipay-open-platform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate payment workflows via Alipay — create trades, process refunds, execute fund transfers, and reconcile billing ledgers natively from any AI agent.

## Description
Bridge your intelligent agents directly into the sprawling financial infrastructure of **Alipay**, one of the world's largest payment ecosystems processing trillions annually across mobile commerce, lifestyle services, and B2C disbursements.

### What you can do

- **Payment Processing** — Create, query, close, and cancel trade orders dynamically handling full lifecycle management
- **Refund Management** — Execute full or partial refunds with reason tracking, automatically querying settlement status
- **Fund Transfers** — Dispatch B2C payouts to individual accounts verifying transfer completion and handling exceptions
- **Bill Reconciliation** — Download daily transaction summaries pulling structured accounting exports for automated book-keeping
- **User Identity** — Exchange OAuth authorization codes to access verified customer profiles securely

### How it works

1. Register as a developer on the [Alipay Open Platform](https://open.alipay.com/)
2. Create an Application to obtain your unique **App ID**
3. Generate an RSA2 key pair and upload the public key to the Alipay console
4. Paste the **App Private Key** below — the engine handles all RSA-SHA256 signature generation automatically per request

Eliminate manual API signature headaches entirely. Your AI agent now signs, dispatches, and parses every Alipay interaction with cryptographic precision leaving you free to focus on business logic.

### Who is this for?

- **E-commerce Operators** — automate order creation and refund processing across storefronts without switching dashboards constantly
- **Financial Controllers** — pull daily settlement bills reconciling ledgers automatically flagging discrepancies before human review
- **Growth Engineers** — integrate Alipay checkout flows into conversational commerce bots enabling frictionless mobile payments at scale


## Available Tools
- **cancel_trade**: Cancel a trade (rollback)
- **close_trade**: Close an unpaid Alipay trade
- **create_trade**: Create a new Alipay transaction/order
- **get_oauth_token**: Exchange authorization code for an OAuth Token
- **query_bill_download_url**: Query the download URL for accounting bills
- **query_trade**: Query the status of an Alipay trade
- **query_transfer**: Query the status of a fund transfer
- **query_user_info**: Query authorized Alipay user information
- **refund_trade**: Refund an Alipay transaction
- **transfer_fund**: Transfer funds to an Alipay user account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alipay Open Platform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Refund the Alipay order 2024040112345 for 15.50 CNY with reason: defective item."

**🤖 AI Agent:**
> Refund processed successfully! Trade 2024040112345 has been partially refunded 15.50 CNY. Refund ID: RF20240401X9A3. The settlement will reflect in the buyer's account within 3–5 business days. Would you like me to query the refund status for confirmation?

---

**👤 You:**
> "Create a new Alipay trade for 299.00 CNY with subject 'Premium Subscription' and notify URL pointing to my webhook."

**🤖 AI Agent:**
> Trade created successfully! Order ID: AP2024041200987. Amount: 299.00 CNY. Subject: Premium Subscription. The payment link has been generated and the notify URL is configured to ping your webhook upon completion. The trade will auto-close in 30 minutes if unpaid. Shall I monitor the payment status?

---

**👤 You:**
> "Download yesterday's settlement bill and summarize the total revenue and refund amounts."

**🤖 AI Agent:**
> Settlement bill downloaded for 2024-04-11. Summary: 142 successful trades totaling 48,720.50 CNY in gross revenue. 7 refunds processed amounting to 1,230.00 CNY. Net settlement: 47,490.50 CNY. The detailed CSV has been parsed and is ready for export. Would you like me to flag any transactions above 5,000 CNY for review?


## Installation & Usage

To install and use the **Alipay Open Platform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alipay-open-platform](https://vinkius.com/mcp/alipay-open-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
