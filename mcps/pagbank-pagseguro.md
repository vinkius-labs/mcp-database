# PagBank PagSeguro MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pagbank-pagseguro)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pagbank-pagseguro-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pagbank-pagseguro-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Create Pix, Boleto, and Card payment links, and manage transactions via PagBank API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PagBank PagSeguro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a Pix payment of R$99.90 for reference 'ORDER-001'."

**🤖 AI Agent:**
> Pix payment created! Status: WAITING. QR Code generated for user to scan.

---

**👤 You:**
> "Show me the balance of my account."

**🤖 AI Agent:**
> Current Available Balance: R$ 1,250.45.

---

**👤 You:**
> "Cancel transaction 12345-ABCDE-67890."

**🤖 AI Agent:**
> Transaction cancelled successfully! Status: CANCELLED.


## Installation & Usage

To install and use the **PagBank PagSeguro** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pagbank-pagseguro](https://vinkius.com/mcp/pagbank-pagseguro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
