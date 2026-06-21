# PagBank PagSeguro MCP Server

Create Pix, Boleto, and Card payment links, and manage transactions via PagBank API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pagbank-pagseguro)

## Overview
**Category:** money-moves
**Tools Count:** 9

## Description
Connect **PagBank (PagSeguro)** to any AI agent and unlock Brazil's leading payment solutions — generate Pix QR codes, Boleto payments, and checkout links for credit cards through natural conversation.

### What you can do
- **Instant Pix** — Generate Pix payments with QR Code data for instant confirmation
- **Boleto Generation** — Create Boleto Bancário for customers without credit cards
- **Checkout Links** — Generate payment links that support Credit Card installments
- **Transaction Search** — Find payments by date range or reference code
- **Refunds** — Cancel transactions (full or partial) easily
- **Account Balance** — Check your current available balance
- **Installments** — Calculate credit card installment options

### How it works
1. Subscribe to this server
2. Enter your PagBank Production or Sandbox Access Token
3. Start processing payments and managing your finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Brazilian Sellers** — Accept payments via Pix and Boleto instantly from your AI assistant
- **E-commerce Managers** — Monitor transactions, check balances, and issue refunds via chat
- **Developers** — Integrate PagBank payments into AI workflows without complex SDKs


## Available Tools
- **get_balance**: Get the current account balance
- **create_boleto_payment**: Generate a Boleto payment
- **cancel_transaction**: If amount is provided, performs partial cancellation.

Cancel a transaction (full or partial refund)
- **create_checkout_link**: Returns a code and a URL.

Create a payment link (checkout) for multiple items
- **get_order**: Get details of an order by ID
- **get_transaction**: Get details of a transaction by code
- **get_installment_options**: Get installment options for a card brand
- **create_pix_payment**: Create an instant Pix payment
- **search_transactions**: Search for transactions by date range


## Installation & Usage

To install and use the **PagBank PagSeguro** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pagbank-pagseguro](https://vinkius.com/mcp/pagbank-pagseguro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
