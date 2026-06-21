# Gelato MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gelato)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gelato-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gelato-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage print-on-demand orders, track fulfillment, and get shipping quotes via AI agents with Gelato.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gelato** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active print orders and their current status."

**🤖 AI Agent:**
> Retrieving orders... I found 5 active print orders, including 'ORD-99' (Status: In Production) and 'ORD-101' (Status: Shipped). Would you like the tracking details for the shipped one?

---

**👤 You:**
> "Get the shipping details for order 'gelato_12345'."

**🤖 AI Agent:**
> Fetching shipments... Order gelato_12345 has been shipped via DHL. The tracking number is '1Z999...' and the estimated delivery is October 15th.

---

**👤 You:**
> "List all products in the 'Apparel' catalog (ID: cat_987)."

**🤖 AI Agent:**
> Retrieving products... In the Apparel catalog, I found 12 items including 'Classic T-Shirt' (UID: shirt_001) and 'Premium Hoodie' (UID: hood_05).


## Installation & Usage

To install and use the **Gelato** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gelato](https://vinkius.com/mcp/gelato)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
