# Gift Up! MCP Server

Manage gift card orders, track balances, and process redemptions via AI agents with Gift Up!.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gift-up)

## Overview
**Category:** ecommerce
**Tools Count:** 12

## Description
Connect your **Gift Up!** account to any AI agent to automate your gift card management and redemption workflows through the Model Context Protocol (MCP). Gift Up! is the simplest way to sell gift cards on your own website. This MCP server enables you to retrieve gift card orders, validate codes, track remaining balances, and process partial or full redemptions directly through natural conversation.

### Key Features

- **Order Management** — List all gift card orders, fetch detailed metadata, and search for orders using public reference numbers.
- **Balance Verification** — Instantly check the remaining value and validity of any gift card code provided by a customer.
- **Flexible Redemptions** — Process full or partial redemptions programmatically to deduct balances during your checkout or support process.
- **Custom Metadata** — Update and retrieve internal key-value pairs attached to orders for seamless mapping with your CRM or ERP.
- **Registry Oversight** — List all active and redeemed gift cards in your system to maintain a complete audit trail.
- **Webhook Visibility** — Monitor active webhooks to ensure your internal systems are receiving real-time redemption notifications.
- **Real-time Synchronization** — Keep your gift card operations accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Gift Up! API Key (found in Settings > API Keys)
3. Start managing your gift cards from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Ops & Support** — quickly verify if a gift card code is valid or process a manual redemption without leaving the chat.
- **Finance & Accounting** — get a real-time overview of recent gift card sales and outstanding balances via simple AI commands.
- **Store Managers** — monitor gift card performance and update order metadata for better fulfillment tracking.


## Available Tools
- **verify_api_connection**: Check connection
- **find_order_by_ref**: Search by reference
- **get_account_details**: Get account identity
- **get_card_details**: Get card metadata
- **validate_gift_card**: Check card balance
- **get_order_details**: Get order metadata
- **list_active_gift_cards**: List all gift cards
- **list_gift_orders**: List all orders
- **list_gift_webhooks**: List webhook configs
- **redeem_gift_card_full**: Redeem full balance
- **redeem_gift_card**: Process partial redemption
- **update_order_metadata**: Set custom fields


## Installation & Usage

To install and use the **Gift Up!** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gift-up](https://vinkius.com/mcp/gift-up)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
