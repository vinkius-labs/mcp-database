# Banco do Brasil MCP Server

Check balance, statements, pay Pix/Boleto, and manage your BB account via API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/banco-do-brasil)

## Overview
**Category:** industry-titans
**Tools Count:** 9

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


## Installation & Usage

To install and use the **Banco do Brasil** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/banco-do-brasil](https://vinkius.com/mcp/banco-do-brasil)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
