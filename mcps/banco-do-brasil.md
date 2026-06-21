# Banco do Brasil MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/banco-do-brasil)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/banco-do-brasil-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/banco-do-brasil-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Check balance, statements, pay Pix/Boleto, and manage your BB account via API.

## Description
Connect your **Banco do Brasil** account to any AI agent and perform essential banking tasks — check balances, view transaction history, send Pix payments, and pay bills through natural conversation.

### What you can do
- **Account Details** — View agency, account number, and available limits
- **Balances** — Check available funds and credit limits instantly
- **Statement** — Retrieve transaction history by date range
- **Pix Payments** — Send instant transfers using any Pix key (CPF, Email, Phone)
- **Boleto Payments** — Pay utility bills and barcodes
- **Pix History** — View all sent and received Pix transfers
- **Credit Card** — View credit card invoices and totals

### How it works
1. Subscribe to this server
2. Enter your OAuth2 Access Token from the BB Developers Portal
3. Start managing your finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **BB Customers** — Automate their daily banking tasks via AI
- **Developers** — Integrate BB banking capabilities into financial apps and bots
- **Business Owners** — Monitor account activity and pay suppliers automatically


## Available Tools
- **get_accounts**: Usually returns one active account.

Get list of checking accounts
- **get_balance**: Get current account balance and limits
- **create_pix**: Send a Pix payment to a key
- **get_credit_card_invoices**: Get credit card invoices
- **pay_barcode**: Pay a barcode/boleto bill
- **pay_utility_bill**: Pay a utility bill via barcode
- **get_pix_history**: Type can be RECEIVED or SENT.

Get history of Pix transfers (Sent/Received)
- **get_scheduled_payments**: Get scheduled future payments
- **get_statement**: Dates in YYYY-MM-DD format.

Get account statement (transactions) by date range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Banco do Brasil** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my current balance."

**🤖 AI Agent:**
> Available Balance: R$ 2,500.00 | Credit Limit: R$ 500.00

---

**👤 You:**
> "Send a Pix of R$50 to joao@email.com."

**🤖 AI Agent:**
> Pix sent successfully! End-to-End ID: E1234567890123456789012345678901.

---

**👤 You:**
> "Show me the transactions from last week."

**🤖 AI Agent:**
> Found 5 transactions: 1. R$ -50.00 (Pix Sent). 2. R$ 2,000.00 (Salary Received).


## Installation & Usage

To install and use the **Banco do Brasil** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/banco-do-brasil](https://vinkius.com/mcp/banco-do-brasil)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
