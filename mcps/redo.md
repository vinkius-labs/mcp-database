# Redo MCP Server

Manage returns, track shipping protection claims, and oversee exchanges via AI agents with Redo.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/redo)

## Overview
**Category:** ecommerce
**Tools Count:** 12

## Description
Connect your **Redo** account to any AI agent to automate your returns management and shipping protection workflows through the Model Context Protocol (MCP). Redo provides a comprehensive suite for handling customer returns, exchanges, and package protection claims for lost or damaged items. This MCP server enables you to track return requests, approve claims, and process final resolutions directly through natural conversation.

### Key Features

- **Returns & Claims Oversight** — List all return requests and shipping protection claims, checking their status and customer metadata instantly.
- **Status Automation** — Update the lifecycle status of a return (e.g., approved, rejected) programmatically from your chat interface.
- **Resolution Processing** — Trigger final actions like refunds, store credits, or exchange order creation for lost or damaged packages.
- **Collaborative Notes** — Add internal comments and communication logs to any return or claim record for better team alignment.
- **Coverage Discovery** — Access high-level information about your shipping protection settings and eligible products.
- **Shipping Rate Calculation** — Retrieve real-time shipping rates for return packages to estimate costs for your customers.
- **Webhook Visibility** — Monitor active webhooks to ensure your internal systems are receiving real-time return notifications.
- **Real-time Synchronization** — Keep your post-purchase operations accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Redo Store ID and API Secret (found in your Redo settings)
3. Start managing your returns and claims from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Ops & Support** — quickly check the status of a customer's claim or approve a return without manual dashboard navigation.
- **Customer Success Teams** — get a real-time overview of recent return reasons and sentiment via simple AI commands.
- **Logistics Managers** — automate the retrieval of shipping rates and monitor protection coverage levels.


## Available Tools
- **add_internal_note**: Post a return comment
- **approve_return_claim**: Approve a request
- **verify_api_connection**: Check connection
- **get_store_details**: Get store metadata
- **get_protection_summary**: Get coverage details
- **get_return_details**: Get return metadata
- **get_return_shipping_rates**: Get shipping costs
- **list_protected_items**: List covered products
- **list_store_returns**: List returns/claims
- **list_return_webhooks**: List webhook configs
- **process_final_resolution**: Finalize return/claim
- **reject_return_claim**: Reject a request


## Installation & Usage

To install and use the **Redo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/redo](https://vinkius.com/mcp/redo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
