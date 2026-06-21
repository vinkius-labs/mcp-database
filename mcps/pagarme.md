# Pagar.me MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pagarme)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pagarme-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pagarme-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Create orders, manage subscriptions, and process Pix/Boleto payments via Pagar.me API.

## Description
Connect **Pagar.me** to any AI agent and unlock a powerful Brazilian payment infrastructure — create orders with Pix, Boleto, or Credit Card, manage recurring subscriptions, and track transactions through natural conversation.

### What you can do
- **Order Creation** — Create orders for single items with multiple payment methods
- **Pix Payments** — Generate instant Pix QR Codes for immediate payment
- **Boleto Generation** — Create Boleto Bancário with custom due dates
- **Subscriptions** — Set up recurring billing for services
- **Customer Management** — Register customers and view their history
- **Transaction Tracking** — List orders and check their status

### How it works
1. Subscribe to this server
2. Enter your Pagar.me Secret Key
3. Start processing payments and managing subscriptions from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Brazilian Businesses** — Accept Pix and Boleto payments directly from AI chats
- **SaaS Founders** — Manage recurring subscriptions and customer billing
- **Developers** — Integrate Pagar.me orders into complex AI workflows


## Available Tools
- **create_boleto_order**: Create an order paid via Boleto
- **cancel_order**: Cancel an order
- **capture_order**: Capture an authorized order
- **create_customer**: Document can be CPF or CNPJ.

Register a new customer
- **get_customer**: Get customer details
- **get_order**: Get details of a specific order
- **get_subscription**: Get subscription details
- **list_orders**: List recent orders
- **create_order**: Items and Customer are required. You can add custom payments array or use the Pix/Boleto helpers.

Create a new order with credit card or custom payments
- **create_pix_order**: Expires in 1 hour.

Create an order paid via Pix
- **create_subscription**: Create a recurring subscription for a customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pagar.me** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a Pix order for R$50.00 for customer João Silva."

**🤖 AI Agent:**
> Pix order created! QR Code generated. Waiting for payment.

---

**👤 You:**
> "Show me the last 5 orders."

**🤖 AI Agent:**
> Found 5 orders: 1. R$ 50.00 (Pix - Paid). 2. R$ 120.00 (Card - Pending). 3. R$ 15.00 (Boleto - Expired).

---

**👤 You:**
> "Create a monthly subscription of R$99.90 for customer 123 on plan 456."

**🤖 AI Agent:**
> Subscription created successfully! Status: Active. Next billing date: 2026-04-01.


## Installation & Usage

To install and use the **Pagar.me** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pagarme](https://vinkius.com/mcp/pagarme)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
