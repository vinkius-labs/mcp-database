# OpenNode MCP Server

Process Bitcoin and Lightning Network payments, manage charges, and initiate secure withdrawals directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/opennode)

## Overview
**Category:** payment-processing
**Tools Count:** 22

## Description
Connect your **OpenNode** account to any AI agent to seamlessly integrate Bitcoin and Lightning Network payment processing into your workflows.

### What you can do

- **Payment Requests (Charges)** — Create new charges (`create_charge`) with Lightning BOLT11 invoices or on-chain addresses, and retrieve details or list paid charges.
- **Withdrawals & Payouts** — Initiate withdrawals (`initiate_withdrawal`) to Lightning invoices or Bitcoin addresses, and confirm previewed chain or Lightning withdrawals.
- **Transaction History** — Track and list your withdrawal history (`list_withdrawals`) to audit your account activity.

### How it works

1. Subscribe to this server
2. Enter your OpenNode API Key
3. Start managing Bitcoin payments and payouts from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_account_balance**: Get account balance
- **list_activity**: List account activity
- **create_address**: Create a static on-chain address
- **list_addresses**: List static on-chain addresses
- **create_charge**: Create a new OpenNode charge (Bitcoin payment request)
- **get_charge**: Get charge info
- **list_charges**: List paid charges
- **get_currencies**: Get supported originating currencies
- **initiate_exchange**: Initiate an exchange between BTC and Fiat
- **create_lnurl_pay**: Create a static LN address (LNURL-Pay)
- **list_lnurl_pay**: List static LN addresses (LNURL-Pay)
- **initiate_lnurl_withdrawal**: Initiate LNURL withdrawal
- **get_rates**: Get exchange rates
- **create_refund**: Create a refund for an underpaid charge
- **get_refund**: Get refund info
- **list_refunds**: List refunds
- **set_scheduled_withdrawals**: Set scheduled bank withdrawals status
- **confirm_chain_withdrawal**: Confirm a previewed chain withdrawal request
- **confirm_ln_withdrawal**: Confirm a previewed Lightning withdrawal request
- **get_withdrawal**: Get withdrawal info
- **initiate_withdrawal**: Can also be used to preview payouts.

Initiate a withdrawal (Paying via Lightning / Chain)
- **list_withdrawals**: List withdrawals


## Installation & Usage

To install and use the **OpenNode** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opennode](https://vinkius.com/mcp/opennode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
