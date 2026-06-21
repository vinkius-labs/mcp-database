# Stripe Legacy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stripe-legacy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/stripe-legacy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/stripe-legacy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage payments, customers, and account balances on Stripe via the legacy API with AI agents.

## Description
Connect your **Stripe** account to any AI agent to automate your basic payment processing and customer management. This integration provides a streamlined interface for the core Stripe v1 API, allowing you to monitor charges, create payment tokens, and track account balances through natural conversation.

### What you can do

- **Payment Orchestration** — List recent charges and retrieve detailed metadata for specific transactions programmatically.
- **Customer Management** — Access and monitor your customer database to keep your client records synchronized directly from the AI interface.
- **Charge Lifecycle Control** — Create new charges and manage payment tokens using simple AI commands to facilitate transactions.
- **Financial Monitoring** — Retrieve your real-time Stripe account balance to ensure your business liquidity is always visible.
- **Operational Oversight** — Get instant summaries of recent payment activity and customer metadata via natural language.

### How it works

1. Subscribe to this server
2. Enter your Stripe Secret Key (sk_...) from your dashboard
3. Start managing your payment operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Business Owners** — quickly check recent sales and account balances without switching apps.
- **Support Teams** — automate the retrieval of customer charge details to resolve billing inquiries via natural conversation.
- **Developers** — test core Stripe payment flows and monitor balances directly within the chat.


## Available Tools
- **create_charge**: Pass data as a JSON string.

Create a new charge
- **create_customer**: Create a new Stripe customer
- **create_refund**: Create a refund for a charge
- **create_token**: Pass data as a JSON string.

Create a single-use token
- **get_balance**: Check account balance
- **get_charge**: Get charge details
- **get_customer**: Get details for a specific customer
- **list_charges**: List all Stripe charges
- **list_customers**: List all Stripe customers
- **list_invoices**: List all invoices
- **list_subscriptions**: List all active subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stripe Legacy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my current Stripe account balance."

**🤖 AI Agent:**
> I've retrieved your balance. You currently have $5,240.50 available and $1,120.00 pending in your Stripe account.

---

**👤 You:**
> "Show me all charges from the past 24 hours with their status and customer details."

**🤖 AI Agent:**
> 89 charges in 24 hours totaling $23,456. Succeeded (84): $22,100. Failed (3): $890 (2 card declined, 1 insufficient funds). Pending (2): $466. By currency: USD (67, $18,900), EUR (15, €3,200), GBP (7, £1,356). Top customers: Meridian Corp ($4,500, 2 charges), TechVentures ($2,300). Average charge: $263.55. Recurring vs one-time: 56 recurring ($15,200), 33 one-time ($8,256). Disputes: 0. Refunds issued: 2 ($189). Processing fees: $682 (2.9% + $0.30).

---

**👤 You:**
> "Get the current account balance and recent payout schedule."

**🤖 AI Agent:**
> Account balance: Available $34,560. Pending: $12,340 (clears in 2 days). Connect reserved: $0. Total: $46,900. Recent payouts: May 15 - $28,900 (completed, bank ending 4521). May 12 - $24,500 (completed). May 9 - $31,200 (completed). Payout schedule: daily (automatic). Next payout: tomorrow, estimated $18,400. Monthly summary: $156,000 gross volume, $4,524 in fees (2.9%). Net deposits: $151,476. Currency breakdown: 78% USD, 14% EUR, 8% GBP.


## Installation & Usage

To install and use the **Stripe Legacy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stripe-legacy](https://vinkius.com/mcp/stripe-legacy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
