# Tango MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tango)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tango-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tango-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Document any process by recording your screen clicks and turning them into step-by-step guides with annotated screenshots.

## Description
Connect your **Tango (formerly Tango Card)** reward platform account to any AI agent and simplify how you distribute digital gift cards, manage customers, and monitor funding accounts through natural conversation.

### What you can do

- **Catalog Discovery** — Browse the full global catalog of brands, including gift cards, prepaid cards, and non-profit donations.
- **Reward Distribution** — Place and automate orders for digital rewards delivered via email instantly.
- **Customer & Account Management** — List, create, and manage customer groups and their associated funding accounts.
- **Financial Oversight** — Check real-time account balances, list funding sources, and retrieve current exchange rates.
- **Order Tracking** — Monitor your reward history and fetch detailed status and credentials for specific order IDs.
- **Scalable Rewards** — Coordinate bulk payouts and loyalty incentives directly from Claude, Cursor, or any MCP client.

### How it works

1. Subscribe to this server
2. Enter your Tango Platform Name and Platform Key
3. Start managing your digital reward ecosystem from your favorite AI assistant

### Who is this for?

- **HR & Culture Managers** — quickly send employee recognition rewards and verify account balances via simple AI commands.
- **Marketing & Loyalty Teams** — automate the distribution of campaign incentives and browse brand availability directly from the workspace.
- **Operations Leads** — monitor order histories and manage customer group funding via the AI assistant.


## Available Tools
- **create_account**: Create a new funding account
- **create_customer**: Create a new customer
- **create_order**: Place a reward order
- **get_account**: Get account balance
- **get_catalog**: List available reward brands
- **get_customer**: Get customer details
- **get_exchange_rates**: Get currency exchange rates
- **get_order**: Get order status
- **list_accounts**: List accounts for a customer
- **list_customers**: List all customers
- **list_funding_sources**: List funding sources
- **list_orders**: List recent orders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tango** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all available gift card brands in the catalog."

**🤖 AI Agent:**
> I've retrieved the global catalog. You have access to hundreds of brands including Amazon, Starbucks, Apple, and Target. Which country or category are you interested in?

---

**👤 You:**
> "What is the current balance of account 'acc_10293'?"

**🤖 AI Agent:**
> Fetching balance... The account 'acc_10293' currently has a balance of $1,250.00 USD. You have sufficient funds for your upcoming reward distributions.

---

**👤 You:**
> "Send a $25 Amazon gift card (UTID: AMZN-US-2500) to 'john.doe@example.com'."

**🤖 AI Agent:**
> Order initiated! I've triggered the delivery of a $25.00 Amazon reward to john.doe@example.com. The order ID is ord_88231. I'll let you know once the status shows it's successfully delivered.


## Installation & Usage

To install and use the **Tango** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tango](https://vinkius.com/mcp/tango)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
