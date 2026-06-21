# Increase MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/increase)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/increase-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/increase-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Your very own programmatic commercial bank. Construct completely new bank accounts, fetch balance ledgers, map Routing numbers and fire wire limits.

## Description
The **Increase MCP Server** connects AI to a physical, fully compliant commercial US bank built explicitly top-down for programmatic transactions.

### What you can do

- **Endless Provisioning** — Instantly generate new live bank accounts `increase_create_account` acting as sub-ledgers, enabling separate balances.
- **Open Payment Rails** — Need to inject funds into a supplier directly using native American payment streams? Use `increase_create_ach` or sweep high-value overnight `increase_create_wire` securely.
- **Simulation Environment** — Use Sandbox arrays to trigger simulated money hits `increase_simulate_inbound_ach` checking if an external agent script validates receiving deposits before going to production.

### How it works

1. In the Increase dashboard, decide if you're in Development (Sandbox) mode or Live (Production) mode.
2. Obtain an API Key (`sk_test` or `sk_prod`).
3. Plug the key directly into Vinkius to sync the core network natively with agent logic.

### Who is this for?

- **Platform Builders (BaaS)** — Create internal software that orchestrates money mapping transparently.
- **Advanced Corporate Ops** — Fire up temporary transaction routing numbers to accept wires.


## Available Tools
- **increase_create_account**: Spin up a new Bank Account programmatically
- **increase_create_ach**: Push an outbound ACH transfer to any US Bank
- **increase_create_card**: Issue a physical/virtual debit card attached to an account
- **increase_create_routing_number**: Generate new ABA routing & account number data
- **increase_create_wire**: Send a same-day US Wire transfer
- **increase_get_balance**: Fetch realtime ledger balance for a specific account
- **increase_list_accounts**: List all sub-accounts under your charter
- **increase_list_cards**: Sweep the active array of issued Cards
- **increase_list_transactions**: Financial history extraction (Booked)
- **increase_list_transfers**: Audit outbound transfers
- **increase_simulate_inbound_ach**: Simulate receiving an ACH inbound (SANDBOX ONLY)
- **increase_simulate_inbound_wire**: Simulate receiving a Wire inbound (SANDBOX ONLY)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Increase** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Use our main test routing sandbox mechanism to simulate inbound an external payload of $1000 into Account ID 'acc_1234'."

**🤖 AI Agent:**
> Simulation dispatched! Expected parameters were simulated into the core routing infrastructure successfully. The endpoint responded and acknowledged $1,000 artificial liquidity injection into your routing destination target. Validate your app webhooks now.

---

**👤 You:**
> "Audit our entire open accounts layout right now."

**🤖 AI Agent:**
> Found exactly 4 Demand Deposit accounts running 'opened' conditions. They map respectively under entity groups 'Operational', 'Cloud Subscriptions', 'Holding', and 'Local Dev'. Current aggregate counts reflect stability.

---

**👤 You:**
> "Spin up a new fresh physical corporate banking account dedicated uniquely to 'Server Spends'. Send the Routing number to me."

**🤖 AI Agent:**
> Success chain completed in sequence. First, entity 'Server Spends' received a booked ID structure constraint within banking logic. Secondly, the routing generator hooked an incoming ABA/Account array assigned completely to this context. Account numbers are currently available.


## Installation & Usage

To install and use the **Increase** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/increase](https://vinkius.com/mcp/increase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
