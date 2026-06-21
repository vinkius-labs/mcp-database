# Increase MCP Server

Your very own programmatic commercial bank. Construct completely new bank accounts, fetch balance ledgers, map Routing numbers and fire wire limits.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/increase)

## Overview
**Category:** money-moves
**Tools Count:** 12

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


## Installation & Usage

To install and use the **Increase** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/increase](https://vinkius.com/mcp/increase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
