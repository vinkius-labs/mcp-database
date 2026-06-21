# Brankas MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brankas)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/brankas-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/brankas-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage open finance operations via Brankas API — process direct payments, send disbursements, and access bank statements from any AI agent.

## Description
Connect your **Brankas** Open Finance account to any AI agent and orchestrate your payments, payouts, and financial data workflows across Southeast Asia through natural conversation.

### What you can do

- **Direct Payments (Money-in)** — Initiate checkout sessions to accept instant account-to-account payments and track transaction statuses.
- **Disbursements (Money-out)** — Send payouts automatically through inter-bank or intra-bank transfers and monitor their progress.
- **Data Aggregation** — Retrieve real-time bank account balances, transaction history (statements), and identity data from consented users.

### How it works

1. Subscribe to this server
2. Enter your Brankas API Key and Environment (sandbox or production)
3. Start managing your open finance operations from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **create_checkout**: Create a new Direct payment checkout session
- **get_balance**: Retrieve linked bank account balances
- **get_identities**: Retrieve linked identity data
- **get_statement**: Retrieve linked bank statement data
- **get_transaction**: Get status of a Direct payment transaction
- **get_transfer_status**: Get status of a Disburse transfer
- **inter_bank_transfer**: Initiate an inter-bank disbursement (payout)
- **intra_bank_transfer**: Initiate an intra-bank disbursement (payout)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brankas** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a checkout session for 500 PHP."

**🤖 AI Agent:**
> Checkout session successfully created for 500 PHP. The transaction ID is 'txn_abc123'. You can use this ID to check the status later.

---

**👤 You:**
> "Check the status of transfer trf_99283."

**🤖 AI Agent:**
> The disbursement transfer 'trf_99283' is currently marked as 'SUCCESS'. The funds have been deposited into the beneficiary's account.

---

**👤 You:**
> "Retrieve the latest bank statement data."

**🤖 AI Agent:**
> Retrieving statement data... I found 15 recent transactions for the connected account, including a deposit of 1000 IDR and a withdrawal of 200 IDR.


## Installation & Usage

To install and use the **Brankas** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brankas](https://vinkius.com/mcp/brankas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
