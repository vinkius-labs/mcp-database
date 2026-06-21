# OpenNode MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opennode)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/opennode-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/opennode-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [payment-processing](../categories/payment-processing.md)

Process Bitcoin and Lightning Network payments, manage charges, and initiate secure withdrawals directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenNode** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a charge for 10000 satoshis with the description 'Coffee purchase'."

**🤖 AI Agent:**
> I've created the charge using `create_charge`. Here is your Lightning Invoice (BOLT11): `lnbc100u...` and the on-chain address: `tb1q...`. The charge ID is `ch_123456`.

---

**👤 You:**
> "List my paid charges on page 1."

**🤖 AI Agent:**
> Retrieving paid charges... I found 3 paid charges via `list_charges`. Notable payments include 'Order #1002' (ID: `ch_abc123`) and 'Donation' (ID: `ch_xyz789`).

---

**👤 You:**
> "Get the details of charge ID ch_abc123."

**🤖 AI Agent:**
> Inspecting charge `ch_abc123` using `get_charge`... The charge is marked as 'paid' for 5000 satoshis, created on 2023-10-27, with the description 'API Access'.


## Installation & Usage

To install and use the **OpenNode** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opennode](https://vinkius.com/mcp/opennode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
