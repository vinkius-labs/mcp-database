# N26 Banking MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/n26-banking)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/n26-banking-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/n26-banking-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Universal N26 intelligence — check balances, accounts, and spaces via AI.

## Description
Equip your AI agent with real-time personal finance intelligence through the **N26** MCP server. This integration provides secure access to your N26 bank accounts, allowing your agent to retrieve current balances, list multiple accounts, and fetch recent transaction history. Your agent can also explore N26 'Spaces' (sub-accounts) to monitor specific savings goals. Whether you are auditing your personal spending, tracking budget goals across Europe, or managing daily finances, your agent acts as a dedicated financial assistant through natural conversation.

### What you can do

- **Balance Inquiry** — Get the real-time balance and IBAN for any of your N26 accounts.
- **Transaction History** — Fetch recent transactions to audit your spending patterns and vendors across the Eurozone.
- **Space Monitoring** — Retrieve details and balances for all your N26 Spaces.
- **Financial Auditing** — Ask your agent to summarize your recent financial activity and sub-account status.

### How it works

1. Subscribe to this server
2. Enter your N26 Access Token (get it at N26 Developer portal)
3. Start managing your finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Personal Finance Enthusiasts** — track their spending and balances through simple AI queries.
- **European Expats & Digital Nomads** — monitor their N26 accounts while living or traveling across Europe.
- **Sustainable Devs** — build automated personal finance workflows and budgeting tools.
- **Busy Professionals** — get quick summaries of their financial status without opening an app.


## Available Tools
- **get_n26_accounts**: List all N26 accounts
- **get_n26_spaces**: Get N26 spaces and sub-account balances
- **get_n26_transactions**: Get recent N26 transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **N26 Banking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my N26 account balance."

**🤖 AI Agent:**
> Retrieving your account details... Your current balance is €2,150.40. I've also identified your IBAN if you need it for a transfer. Would you like to see your recent transactions?

---

**👤 You:**
> "What are my last 3 transactions on N26?"

**🤖 AI Agent:**
> Fetching your history... Your last 3 transactions were: 'Lidl' (€15.20), 'Amazon.de' (€45.00), and 'Shell' (€60.00). Would you like to see more details for any of these?

---

**👤 You:**
> "List all my N26 Spaces and their balances."

**🤖 AI Agent:**
> Retrieving your Spaces... You have 3 active spaces: 'Vacation' (€1,200), 'New Car' (€5,000), and 'Emergency Fund' (€2,500). Your total savings across all spaces is €8,700.


## Installation & Usage

To install and use the **N26 Banking** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/n26-banking](https://vinkius.com/mcp/n26-banking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
