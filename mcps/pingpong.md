# PingPong MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pingpong)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pingpong-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pingpong-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Global multi-currency payment platform for E-commerce — manage accounts, balances, and payouts via AI.

## Description
Empower your AI agent to orchestrate your cross-border financial operations with **PingPong**, the leading global payment platform for modern e-commerce. By connecting PingPong to your agent, you transform complex account management and fund orchestration into a natural conversation. Your agent can instantly list your global receiving accounts, retrieve real-time balances, monitor transaction histories, and even initiate payouts without you needing to navigate the complex PingPong dashboard. Whether you are managing multiple Amazon stores or distributing funds to global suppliers, your agent acts as a real-time treasury assistant, keeping your capital accurate and your cross-border payments moving.

### What you can do

- **Account Orchestration** — List all your PingPong global receiving accounts and retrieve detailed metadata for each.
- **Balance Monitoring** — Get real-time balance information across multiple currencies and account types.
- **Transaction Auditing** — Browse transaction histories with full support for filtering by status and currency.
- **Payout Control** — Initiate fund withdrawals and monitor the real-time status of your payouts.
- **Treasury Insights** — Retrieve high-level summaries of your global sales and virtual card (VCC) balances.

### How it works

1. Subscribe to this server
2. Enter your PingPong App ID and App Secret
3. Start managing your global payments through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Sellers** — monitor store payouts and manage receiving accounts across multiple global platforms.
- **Treasury Managers** — audit multi-currency balances and track transaction flows through natural language queries.
- **Operations Teams** — oversee virtual card usage and coordinate fund withdrawals via a unified AI interface.
- **Business Owners** — get real-time insights into organization-wide sales performance and cash liquidity.


## Available Tools
- **create_payout**: Create a new payout
- **get_account_details**: Get account information
- **get_balance**: Get account balance
- **get_exchange_rates**: Get real-time exchange rates
- **get_payout_status**: Check payout status
- **get_sales_summary**: Get global sales summary
- **get_vcc_balance**: Get virtual card balance
- **list_accounts**: List global accounts
- **list_store_accounts**: ).

List e-commerce store accounts
- **list_transactions**: List account transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PingPong** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my PingPong receiving accounts."

**🤖 AI Agent:**
> I've retrieved your global receiving accounts. You have 5 active accounts, including receiving channels for Amazon US, Shopify, and Walmart. Would you like to check the balance for any of them?

---

**👤 You:**
> "What is my current balance in USD across all accounts?"

**🤖 AI Agent:**
> Your total current balance across all USD accounts is approximately $45,200. This includes $32,000 in your main receiving account and $13,200 in your VCC balance. Would you like a detailed breakdown?

---

**👤 You:**
> "Check the status of payout 'PAY-8821'."

**🤖 AI Agent:**
> I've checked the status for payout 'PAY-8821'. It is currently 'Processing' by the receiving bank. Funds are expected to arrive in your destination account within 24 hours.


## Installation & Usage

To install and use the **PingPong** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pingpong](https://vinkius.com/mcp/pingpong)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
