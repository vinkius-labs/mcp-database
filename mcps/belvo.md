# Belvo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/belvo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/belvo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/belvo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Access financial data across Latin America via Belvo — list links, accounts, and transactions directly from any AI agent.

## Description
Connect your **Belvo** account to any AI agent and orchestrate your financial data workflows across Latin America through natural conversation.

### What you can do

- **Connection Management** — List and inspect all financial institution links (connections) managed by Belvo.
- **Account Oversight** — Query and retrieve details for banking and gig-economy accounts.
- **Transaction Analysis** — List and filter financial transactions to understand spending patterns and history.
- **Income & Expense Insights** — Access processed insights like recurring expenses and income summaries.
- **Investment Portfolios** — Retrieve detailed information on investment holdings and performance.
- **Institution Discovery** — List all supported banks and institutions in the Belvo ecosystem.

### How it works

1. Subscribe to this server
2. Enter your Belvo Secret ID and Secret Password
3. Start querying financial data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fintech Developers** — quickly audit links and account data without navigating the Belvo dashboard.
- **Financial Analysts** — retrieve transaction and income data for modeling and reporting.
- **Product Managers** — verify institution coverage and data availability directly from their workspace.


## Available Tools
- **get_account**: Get specific account details
- **get_investments**: List investment portfolios
- **get_link**: Get specific connection details
- **get_transaction**: Get specific transaction details
- **list_accounts**: List all financial accounts across all links
- **list_balances**: List balances for all accounts
- **list_incomes**: List income insights for the links
- **list_institutions**: List all supported financial institutions
- **list_links**: List all connections (links) to financial institutions
- **list_owners**: List owners of the financial accounts
- **list_recurring_expenses**: List recurring expense insights
- **list_transactions**: List all transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Belvo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active financial links in my Belvo account."

**🤖 AI Agent:**
> I've retrieved 3 active links: 'Itau' (ID: link_123), 'Nubank' (ID: link_456), and 'Uber' (ID: link_789). Which one would you like to explore?

---

**👤 You:**
> "Show my account balances across all links."

**🤖 AI Agent:**
> Fetching balances... I found 2 accounts: 'Savings (Itau)' with R$ 5,000.00 and 'Checking (Nubank)' with R$ 1,200.00.

---

**👤 You:**
> "List recurring expenses found in my accounts."

**🤖 AI Agent:**
> Retrieving insights... I've identified 4 recurring expenses, including 'Netflix', 'Electricity Bill', and 'Gym Membership'. Would you like the breakdown for any of these?


## Installation & Usage

To install and use the **Belvo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/belvo](https://vinkius.com/mcp/belvo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
