# Mono MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mono)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mono-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mono-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Automate financial data retrieval and payment orchestration via Mono — access account balances, transaction history, and initiate bank transfers directly from any AI agent.

## Description
Connect your **Mono** account to any AI agent to access real-time financial data and payment capabilities across African financial institutions through natural conversation.

### What you can do

- **Account Insights** — Fetch real-time balances, account numbers, and institution details for any linked account using `get_account`.
- **Transaction Analysis** — Query historical transaction data with filters for dates and types (credit/debit) via `get_transactions`.
- **Statement Retrieval** — Generate and download bank statements in JSON or PDF formats for auditing and reconciliation using `get_statement`.
- **Identity Verification** — Retrieve verified identity information including Full Name, BVN, and contact details with `get_identity`.
- **Payment Initiation** — Orchestrate direct bank transfers with custom references and descriptions using `initiate_payment`.

### How it works

1. Subscribe to this server
2. Enter your Mono Secret Key
3. Start managing financial data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fintech Developers** — Test and integrate Mono features directly from your code editor to maintain development flow.
- **Financial Analysts** — Automate the collection of statements and transaction logs for faster reporting and auditing.
- **Operations Teams** — Verify user identities and initiate payouts through simple natural language commands.


## Available Tools
- **get_account**: Get Mono account details
- **get_identity**: Get identity information for a Mono account
- **initiate_payment**: Initiate a direct bank transfer
- **get_statement**: Get bank statement for a Mono account
- **get_transactions**: Get transactions for a Mono account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mono** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the account details and balance for account ID 642a1b2c3d4e5f6g7h8i9j0k."

**🤖 AI Agent:**
> I've retrieved the details for account 642a1b2c3d4e5f6g7h8i9j0k. The account is held at GTBank with a current balance of 250,000 NGN. The account number is 0123456789.

---

**👤 You:**
> "List all credit transactions for account 642a1b2c... from the last month."

**🤖 AI Agent:**
> I found 3 credit transactions for the requested period. The largest was a transfer of 50,000 NGN on 15-10-2023 labeled 'Salary Deposit'. Would you like to see the full list?

---

**👤 You:**
> "Initiate a payment of 5000 kobo with reference 'REF-998' and description 'Service Fee'."

**🤖 AI Agent:**
> Payment initiation request sent. Reference: REF-998. Amount: 5000 kobo. Description: Service Fee. Please follow the redirect URL provided to complete the authorization.


## Installation & Usage

To install and use the **Mono** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mono](https://vinkius.com/mcp/mono)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
