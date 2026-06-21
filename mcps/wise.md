# Wise MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wise)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wise-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wise-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Equip your AI agent with direct access to Wise — check multi-currency balances, track international transfers, and manage recipients without opening the banking interface.

## Description
Connect your **Wise** Business account to your AI agent and manage international payments and multi-currency operations conversationally.

### What you can do

- **Multi-Currency Balances** — Check real-time balances across all your currency accounts (USD, EUR, GBP, and 50+ currencies) instantly.
- **Transfer Tracking** — Monitor the status of outgoing transfers, view estimated delivery dates, and check exchange rates applied.
- **Recipient Management** — List, search, and manage your payment recipients across countries and currencies.
- **Exchange Rates** — Get live exchange rates and compare costs before initiating transfers.

### How it works

1. Subscribe to the Wise integration on the marketplace.
2. Generate a Personal API Token from your Wise Business account (Settings → API tokens → Add new token).
3. Ask your AI agent to check balances, track transfers, or manage recipients.

### Who is this for?

- **International Businesses** — Monitor multi-currency cash positions across global operations without logging into the Wise dashboard.
- **Finance Teams** — Track FX rates and transfer statuses for month-end reconciliation and treasury management.
- **Freelancers & Agencies** — Check incoming payments from international clients and manage multi-currency invoicing from your AI assistant.


## Available Tools
- **list_profiles**: List Wise business profiles
- **get_currencies**: List supported currencies
- **list_balances**: List multi-currency balances
- **get_balance**: Get specific balance details
- **list_recipients**: List payment recipients
- **create_quote**: Create a transfer quote
- **list_transfers**: List all transfers
- **get_transfer**: Get transfer details
- **get_exchange_rate**: Get live exchange rate
- **list_statements**: List account statements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wise** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my current balances across all currencies?"

**🤖 AI Agent:**
> Here are your Wise balances: USD $85,200.00, EUR €42,100.00, GBP £18,500.00, and BRL R$15,800.00. Total equivalent: approximately $167,400 USD.

---

**👤 You:**
> "Get me a quote to send €10,000 from my EUR balance to a USD account."

**🤖 AI Agent:**
> Quote ready: €10,000 → $10,842.50 USD at a rate of 1.0850. Wise fee: €28.50. Estimated delivery: 1 business day. The recipient will receive $10,842.50.

---

**👤 You:**
> "Track the status of my recent transfer to our London office."

**🤖 AI Agent:**
> Your transfer of £15,000 to 'London Office Ltd' is currently in 'Processing' stage. Exchange rate locked at 1.2650 (USD→GBP). Estimated delivery: tomorrow by 3:00 PM GMT.


## Installation & Usage

To install and use the **Wise** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wise](https://vinkius.com/mcp/wise)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
