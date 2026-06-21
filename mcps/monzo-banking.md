# Monzo Banking MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/monzo-banking)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/monzo-banking-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/monzo-banking-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Universal Monzo intelligence — check balances, accounts, and transactions via AI.

## Description
Equip your AI agent with real-time personal finance intelligence through the **Monzo** MCP server. This integration provides secure access to your Monzo bank accounts, allowing your agent to retrieve current balances, list multiple accounts, and fetch recent transaction history. Whether you are auditing your personal spending, tracking budget goals, or managing daily finances, your agent acts as a dedicated financial assistant through natural conversation.

### What you can do

- **Balance Inquiry** — Get the real-time balance and daily spending summary for any of your Monzo accounts.
- **Account Listing** — Retrieve a complete list of all bank accounts associated with your profile.
- **Transaction History** — Fetch recent transactions to audit your spending patterns and vendors.
- **Financial Auditing** — Ask your agent to summarize your recent financial activity.

### How it works

1. Subscribe to this server
2. Enter your Monzo Access Token (get it at developers.monzo.com)
3. Start managing your finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Personal Finance Enthusiasts** — track their spending and balances through simple AI queries.
- **Digital Nomads** — monitor their UK-based Monzo accounts while traveling.
- **Developers** — build automated personal finance workflows and budgeting tools.
- **Busy Professionals** — get quick summaries of their financial status without opening an app.


## Available Tools
- **get_monzo_accounts**: List all Monzo accounts
- **get_monzo_balance**: Get balance for a Monzo account
- **get_monzo_transactions**: Get recent transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Monzo Banking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my current Monzo balance."

**🤖 AI Agent:**
> Retrieving your account balance... Your current balance is £1,245.50. You have spent £12.30 so far today. Would you like to see your recent transactions?

---

**👤 You:**
> "List my Monzo accounts."

**🤖 AI Agent:**
> I've found 2 accounts: a 'Personal' account (ending in 4567) and a 'Joint' account (ending in 8901). Which one would you like to check?

---

**👤 You:**
> "What were my last 5 transactions?"

**🤖 AI Agent:**
> Fetching your recent history... Your last 5 transactions include 'Tesco' (£5.40), 'Starbucks' (£3.20), and 'Transport for London' (£2.10). Would you like the full breakdown?


## Installation & Usage

To install and use the **Monzo Banking** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/monzo-banking](https://vinkius.com/mcp/monzo-banking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
