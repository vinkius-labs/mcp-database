# LianLian Pay MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lianlian-pay)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lianlian-pay-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lianlian-pay-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Global cross-border payment and settlement platform — manage balances, payments, and settlements via AI.

## Description
Empower your AI agent to orchestrate your international financial infrastructure with **LianLian Pay**, the premier cross-border payment platform for enterprise global trade. By connecting LianLian Pay to your agent, you transform complex settlement tracking, fund collections, and multi-currency management into a natural conversation. Your agent can instantly list your balances, retrieve transaction details, monitor fund settlements, and even initiate refund requests without you ever needing to navigate the comprehensive LianLian Global portal. Whether you are managing cross-border e-commerce revenue or coordinating international supplier payments, your agent acts as a real-time global treasury assistant, keeping your data accurate and your settlements moving.

### What you can do

- **Balance Orchestration** — Retrieve real-time balance information across your LianLian merchant accounts.
- **Payment Management** — Create and track payment orders with full support for unique identifiers and status queries.
- **Settlement Monitoring** — Browse historical settlements and fund withdrawals to track your capital flow.
- **Transaction Auditing** — Filter and retrieve detailed transaction records for financial reconciliation.
- **Treasury Insights** — Retrieve current FX exchange rates and supported bank lists for efficient fund management.

### How it works

1. Subscribe to this server
2. Enter your LianLian Merchant ID and RSA Private Key
3. Start managing your global settlements through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Directors** — monitor organization-wide liquidity and audit global settlements through natural language.
- **Treasury Operations** — coordinate payments and track fund withdrawals directly from your AI-powered workspace.
- **E-commerce Enterprises** — manage cross-border revenue and reconcile transactions via a unified AI interface.
- **Logistics & Trade Partners** — integrate international payment status tracking into your automated workflows.


## Available Tools
- **create_payment**: Create a new payment
- **get_account_info**: Get merchant account info
- **get_balance**: Get account balance
- **get_bank_list**: Get supported banks
- **get_exchange_rates**: Get current FX rates
- **list_settlements**: List settlements
- **list_transactions**: List transactions
- **list_withdrawals**: List fund withdrawals
- **query_order**: Query order status
- **refund_order**: Refund a payment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LianLian Pay** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current balance on LianLian Pay?"

**🤖 AI Agent:**
> I've retrieved your account balances. You have a total available balance of $120,500 USD and €15,200 EUR. Would you like a breakdown of pending settlements?

---

**👤 You:**
> "Check the status of order 'LL-ORDER-8821'."

**🤖 AI Agent:**
> The order 'LL-ORDER-8821' is currently 'Completed'. The payment was successfully collected at 10:30 AM today. Funds are scheduled for settlement in 2 business days.

---

**👤 You:**
> "List the last 5 settlements for my merchant account."

**🤖 AI Agent:**
> I've listed your 5 most recent settlements. The largest was for $45,000 on April 8th. Total settled amount for this week is $112,000. Should I check for any failed withdrawal attempts?


## Installation & Usage

To install and use the **LianLian Pay** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lianlian-pay](https://vinkius.com/mcp/lianlian-pay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
