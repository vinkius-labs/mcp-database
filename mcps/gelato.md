# Gelato MCP Server

Manage print-on-demand orders, track fulfillment, and get shipping quotes via AI agents with Gelato.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gelato)

## Overview
**Category:** ecommerce
**Tools Count:** 12

## Description
Connect your **Gelato** account to any AI agent to automate your print-on-demand (POD) lifecycle through the Model Context Protocol (MCP). Gelato enables creators and businesses to produce and ship custom products globally without inventory. This MCP server allows you to manage orders, retrieve product catalogs, and track real-time shipping statuses directly through natural conversation.

### Key Features

- **Order Management** — List all print orders, fetch detailed status metadata, and create new global orders programmatically.
- **Product Discovery** — Access available product catalogs and retrieve detailed specifications for individual items (product UIDs).
- **Fulfillment Tracking** — Retrieve tracking numbers and real-time shipment details for every order in your account.
- **Pricing & Quoting** — Request real-time shipping and production quotes for potential orders across different regions.
- **Webhook Visibility** — List configured webhooks to ensure your internal systems are receiving real-time production updates.
- **Account Oversight** — Verify your account metadata and API connectivity to maintain a seamless production workflow.
- **Global Fulfillment** — Leverage Gelato's massive network of local production partners directly from your chat interface.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Gelato API Key (found in Developers > API keys)
3. Start managing your POD production from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Operations** — quickly check order statuses or verify fulfillment tracking without manual dashboard navigation.
- **Creative Directors** — get a real-time overview of product catalogs and specifications via simple AI commands.
- **Support Teams** — automate the retrieval of tracking information and order metadata for faster customer resolution.


## Available Tools
- **verify_api_connection**: Check connection
- **create_print_order**: Place new order
- **cancel_print_order**: Cancel an order
- **get_account_info**: Get account identity
- **get_order_status**: Get order details
- **get_product_details**: Get product metadata
- **get_shipping_quote**: Request a quote
- **list_product_catalogs**: List product catalogs
- **list_print_orders**: List all orders
- **list_catalog_products**: List products in catalog
- **get_order_shipments**: Track shipments
- **list_print_webhooks**: List webhook configs


## Installation & Usage

To install and use the **Gelato** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gelato](https://vinkius.com/mcp/gelato)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
