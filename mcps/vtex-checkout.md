# VTEX Checkout MCP Server

Simulate carts, calculate shipping, apply coupons, and manage client profiles on your VTEX store — all from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/vtex-checkout)

## Overview
**Category:** ecommerce
**Tools Count:** 6

## Description
Connect your **VTEX** e-commerce checkout API to any AI agent and streamline your store's pre-purchase operations through natural conversation.

### What you can do

- **Cart Simulation** — Run complete order simulations with items, quantities, and sellers to instantly preview totals, discounts, and available shipping options for any postal code.
- **Shopping Cart Management** — Retrieve the full state of any active shopping cart (orderform), including items, client profile, payment conditions, and logistics.
- **Coupon Management** — Apply discount coupons to active carts and immediately see the impact on totals.
- **Client Profiles** — Look up registered client profiles by user ID — retrieve name, CPF/CNPJ, email, and contact details.
- **Address Management** — Register new shipping addresses for clients, streamlining the checkout flow.
- **Payment Simulation** — Validate payment tokens and simulate payment conditions before placing an order.

### How it works

1. Subscribe to this server
2. Enter your VTEX Account Name, App Key, and App Token (found in **Account Settings → Application Keys** in your VTEX Admin)
3. Start simulating carts and managing checkout data from Claude, Cursor, or any MCP-compatible agent

### Who is this for?

- **E-Commerce Managers** — Quickly simulate cart scenarios during promotions, flash sales, or seasonal campaigns without navigating the full admin.
- **Support Teams** — Look up client profiles and cart states instantly during live support conversations.
- **Operations Teams** — Validate shipping costs and coupon rules across different regions and postal codes.


## Available Tools
- **create_address**: Add a new address to a client profile
- **get_client_profile**: Get client profile details
- **add_coupon**: Apply a coupon to a shopping cart
- **get_orderform**: Get details of a specific shopping cart
- **simulate_payment**: Simulate a payment validation
- **simulate_order**: Simulate a cart and shipping costs


## Installation & Usage

To install and use the **VTEX Checkout** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vtex-checkout](https://vinkius.com/mcp/vtex-checkout)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
