# Finmo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/finmo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/finmo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/finmo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage global pay-ins, payouts, and multi-currency wallets through AI agents with Finmo.

## Description
Connect your **Finmo** account to any AI agent and automate your global treasury and payment operations through the Model Context Protocol (MCP). Finmo provides a unified platform for managing multi-currency liquidity, local collection methods, and cross-border disbursements, now accessible directly through natural conversation.

### What you can do

- **Global Pay-ins** — List available local collection methods across different countries and initiate pay-ins effortlessly.
- **Simplified Payouts** — Manage your disbursements globally by listing and initiating payouts to verified beneficiaries.
- **Wallet Management** — Get a real-time overview of your organization's wallets and balances across various currencies.
- **Customer & Beneficiary Control** — Maintain your database of customers and payout beneficiaries to ensure secure and accurate transactions.
- **Real-time FX Rates** — Fetch live foreign exchange quotes to make informed decisions on currency conversions and international transfers.
- **Virtual Accounts** — List and manage virtual accounts for streamlined reconciliation and local payment acceptance.
- **Transaction Monitoring** — Track the status of refunds and historical payments to keep your financial records in sync.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Finmo Access Key and Secret Key (found in your Developer Settings)
3. Start managing your global treasury operations from Claude, Cursor, or any MCP client

### Who is this for?

- **Finance Teams** — automate the monitoring of global liquidity and transaction statuses without switching between multiple banking portals.
- **Operations Managers** — quickly verify beneficiary details and initiate local or cross-border payouts through simple AI commands.
- **Platforms & Marketplaces** — manage virtual accounts and customer profiles to streamline user fund flows.


## Available Tools
- **create_customer**: Create a new customer
- **create_payin**: Create a new pay-in
- **create_payout**: Create a new payout
- **get_fx_rate**: Get real-time FX rate
- **list_beneficiaries**: List payout beneficiaries
- **list_customers**: List customers
- **list_payin_methods**: List pay-in methods
- **list_payins**: List pay-ins
- **list_payouts**: List payouts
- **list_refunds**: List refunds
- **list_virtual_accounts**: List virtual accounts
- **list_wallets**: List organization wallets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Finmo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the available pay-in methods for Singapore (SG) in SGD?"

**🤖 AI Agent:**
> Checking methods... For Singapore (SG), Finmo supports several pay-in methods including FAST, PayNow, and local bank transfers in SGD. Would you like the specific details for any of these?

---

**👤 You:**
> "Show me the current balance of all my organization wallets."

**🤖 AI Agent:**
> Retrieving balances... You have 3 active wallets: USD ($12,450.00), EUR (€8,200.00), and SGD (S$15,000.00). Your total liquidity is being tracked across these accounts.

---

**👤 You:**
> "Get a live exchange rate to sell 1000 USD for EUR."

**🤖 AI Agent:**
> Fetching live quote... The current exchange rate for 1000 USD is approximately 920.50 EUR. This quote is valid for the next 60 seconds if you wish to proceed with the conversion.


## Installation & Usage

To install and use the **Finmo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/finmo](https://vinkius.com/mcp/finmo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
