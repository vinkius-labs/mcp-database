# Mercado Pago MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mercado-pago)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mercado-pago-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mercado-pago-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Process payments, generate Pix QR codes, manage customers and refunds via Mercado Pago API.

## Description
Connect **Mercado Pago** to any AI agent and unlock Brazil's leading payment gateway — create Pix payments, manage credit card transactions, issue refunds, and handle customer data through natural conversation.

### What you can do
- **Pix Payments** — Generate instant Pix QR Codes for frictionless payments
- **Credit Card Processing** — Charge cards (Visa, Mastercard, Elo) securely
- **Checkout Preferences** — Generate payment links for web checkout
- **Customer Management** — Register customers and save cards for one-click payments
- **Refunds** — Issue partial or full refunds instantly
- **Payment Search** — Find and reconcile payments by email, status, or ID
- **Payment Methods** — List all supported methods in Brazil

### How it works
1. Subscribe to this server
2. Enter your Mercado Pago Access Token
3. Start processing payments and managing finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **E-commerce Managers** — Process payments, issue refunds, and manage orders directly from chat
- **Fintech Developers** — Integrate Pix and card payments into AI-driven financial workflows
- **Small Business Owners** — Generate payment links and track transactions without coding


## Available Tools
- **create_card**: Save a card for a customer
- **create_customer**: Register a new customer
- **create_payment**: Requires a valid card token (generated via SDK frontend). Payment methods: visa, master, amex, etc.

Create a new payment using card or other methods
- **create_preference**: Create a checkout preference for redirection
- **get_customer**: Get customer details
- **get_payment**: Get details of a specific payment by ID
- **get_preference**: Get details of a checkout preference
- **get_identification_types**: Get valid identification types (CPF, CNPJ, etc)
- **list_payment_methods**: List all available payment methods for Brazil
- **create_pix_payment**: Returns QR Code data for the user to scan and pay instantly.

Create a Pix payment with QR Code
- **refund_payment**: If amount is omitted, performs a full refund.

Refund a payment partially or fully
- **search_payments**: Useful for reconciliation and reporting.

Search for payments with filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mercado Pago** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a Pix payment for R$150 for a customer."

**🤖 AI Agent:**
> Pix payment created! Status: pending. QR Code generated for customer to scan and pay instantly.

---

**👤 You:**
> "Refund payment 12345678 fully."

**🤖 AI Agent:**
> Full refund processed successfully! Status: refunded.

---

**👤 You:**
> "Show me all approved payments for user@email.com."

**🤖 AI Agent:**
> Found 3 approved payments: 1. R$ 50.00 (Visa). 2. R$ 120.00 (Pix). 3. R$ 85.50 (Mastercard).


## Installation & Usage

To install and use the **Mercado Pago** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mercado-pago](https://vinkius.com/mcp/mercado-pago)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
