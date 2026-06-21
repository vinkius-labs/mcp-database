# Monnify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/monnify)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/monnify-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/monnify-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage payments and virtual accounts in Nigeria via Monnify — track transactions and reserve accounts directly from your AI agent.

## Description
Connect your **Monnify** merchant account to your AI agent and manage your Nigerian payment operations and customer virtual accounts through natural conversation.

### What you can do

- **Transaction Monitoring** — List all payments and get real-time status updates and references.
- **Virtual Account Reservation** — Create and manage dedicated virtual bank accounts for your customers.
- **Payment Initialization** — Start new payment processes and generate checkout URLs for card or transfer payments.
- **Disbursements & Transfers** — Track outgoing bank transfers and payouts from your account.
- **Invoice Management** — Access digital invoices generated via the Monnify platform.
- **Settlement Tracking** — Monitor the history of payouts from Monnify to your corporate bank account.
- **Bank Discovery** — List all supported Nigerian banks for disbursements and account verification.

### How it works

1. Subscribe to this server
2. Enter your Monnify API Key and Secret Key
3. Start managing your Nigerian finances from Claude, Cursor, or any MCP client

### Who is this for?

- **Fintech Startups** — quickly create virtual accounts for new users or verify transaction statuses.
- **Merchant Operations** — monitor daily collections and bank transfer performance in the Nigerian market.
- **Support Teams** — verify payment references and customer account details during assistance.


## Available Tools
- **get_account_details**: Get reserved account details
- **list_settlements**: List merchant settlements
- **get_transaction**: Get transaction details
- **init_payment**: Initialize a payment transaction
- **list_reserved_accounts**: List reserved virtual accounts
- **list_banks**: List supported Nigerian banks
- **list_monnify_invoices**: List Monnify digital invoices
- **list_transactions**: List Monnify transactions
- **list_disbursements**: List bank transfers (disbursements)
- **reserve_account**: Create a reserved virtual account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Monnify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my most recent transactions on Monnify."

**🤖 AI Agent:**
> I've fetched your recent transactions. You have 8 transactions today, totaling ₦45,000. Most are 'SUCCESSFUL', but one with reference 'REF-123' is 'PENDING'. Would you like the details for the pending one?

---

**👤 You:**
> "Reserve a virtual account for a new customer named 'Ayo Balogun'."

**🤖 AI Agent:**
> Initializing account reservation... I've successfully reserved a virtual account for Ayo Balogun. The Account Number is 1234567890 (Wema Bank) and the Account Name is 'YOUR_COMPANY Ayo Balogun'. Shall I provide the payment reference?

---

**👤 You:**
> "List all Nigerian banks supported by Monnify."

**🤖 AI Agent:**
> Retrieving supported banks... Monnify supports 25+ banks including Access Bank, GTBank, Zenith Bank, First Bank, and United Bank for Africa (UBA). Would you like to see the full list with their bank codes?


## Installation & Usage

To install and use the **Monnify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/monnify](https://vinkius.com/mcp/monnify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
