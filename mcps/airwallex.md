# Airwallex MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/airwallex)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/airwallex-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/airwallex-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Process global payments, manage multi-currency accounts, and track international transfers with enterprise-grade treasury tools.

## Description
Connect your **Airwallex** account to any AI agent and take full control of your global treasury, cross-border payments, and FX management through natural conversation.

### What you can do

- **Global Account Orchestration** — List all your business accounts worldwide programmatically, retrieving detailed real-time balances and high-fidelity currency metadata
- **Payment & Intent Tracking** — Monitor recent payment intents and their high-fidelity status transitions to maintain a perfectly coordinated overview of your receivables
- **Beneficiary Lifecycle Management** — Access and manage your directory of global beneficiaries programmatically to streamline international transfers and compliance
- **FX Intelligence & Quotes** — Programmatically retrieve real-time foreign exchange quotes and market rates to optimize your currency conversions and cross-border movements
- **Infrastructure Monitoring** — Track internal transfers and account-level metadata directly through your agent for instant operational financial reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Client ID** and **API Key** from your Airwallex developer portal (Settings > Developer)
3. Start orchestrating your international finances from Claude, Cursor, or any MCP client

No more manual logging into banking portals to check multicurrency balances or FX rates. Your AI acts as your dedicated global treasurer and finance coordinator.

### Who is this for?

- **Finance Managers** — instantly retrieve global liquidity summaries and monitor payment statuses using natural language commands
- **E-commerce Businesses** — track international receivables and optimize FX movements without leaving your creative workspace
- **Developers** — integrate high-speed financial data and cross-border payment intelligence into custom workflows through simple AI queries


## Available Tools
- **get_balance**: Get account balance
- **get_fx_rates**: Get current FX quotes
- **list_accounts**: List all accounts
- **list_beneficiaries**: List beneficiaries
- **list_payments**: List recent payments
- **list_transfers**: List all transfers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Airwallex** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Airwallex global accounts and their base currencies."

**🤖 AI Agent:**
> I've retrieved your global accounts. You currently have 3 accounts: 'Main Treasury' (USD), 'EU Operations' (EUR), and 'HK Growth'. Which one should we check for real-time balances?

---

**👤 You:**
> "Show the current FX rate for converting 10,000 USD to EUR."

**🤖 AI Agent:**
> Accessing FX intelligence... The current rate for USD to EUR is 0.924. Converting 10,000 USD would yield approximately 9,240 EUR. Shall I retrieve the high-fidelity quote for an actual transfer?

---

**👤 You:**
> "Show my recent payment intents and their statuses."

**🤖 AI Agent:**
> Fetching payment data... Your last 5 intents include 3 'Succeeded' payments totaling $4,500 and 2 'Requires Action' items. The most recent is from @user1. Would you like the high-fidelity metadata for the pending ones?


## Installation & Usage

To install and use the **Airwallex** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airwallex](https://vinkius.com/mcp/airwallex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
