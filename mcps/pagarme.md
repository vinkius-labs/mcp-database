# Pagar.me MCP Server

Create orders, manage subscriptions, and process Pix/Boleto payments via Pagar.me API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pagarme)

## Overview
**Category:** money-moves
**Tools Count:** 11

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


## Installation & Usage

To install and use the **Pagar.me** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pagarme](https://vinkius.com/mcp/pagarme)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
