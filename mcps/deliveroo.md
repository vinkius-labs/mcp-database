# Deliveroo MCP Server

Manage Deliveroo restaurant orders — accept deliveries, track preparation stages, and sync POS status directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/deliveroo)

## Overview
**Category:** industry-titans
**Tools Count:** 5

## Description
Connect your **Deliveroo** restaurant account to any AI agent to streamline your kitchen operations and order management through natural language.

### What you can do

- **Order Lifecycle** — List live orders, fetch specific order metadata, and accept or reject incoming requests within the required timeframe.
- **Preparation Tracking** — Update order stages from 'in_kitchen' to 'ready_for_collection' to keep customers and riders informed in real-time.
- **POS Synchronization** — Notify Deliveroo of successful or failed POS injections to ensure your tablet and kitchen systems stay perfectly in sync.
- **Operational Insights** — Query historical orders by brand, restaurant, or date range to analyze performance without leaving your workspace.

### How it works

1. Subscribe to this server
2. Enter your Deliveroo API Client ID and Secret
3. Start managing your restaurant flow from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Restaurant Managers** — monitor live order flows and update kitchen statuses without juggling multiple tablets.
- **Operations Teams** — audit order history and sync failures across multiple brands or locations.
- **Developers** — integrate delivery workflows into internal tools or custom dashboards using natural language queries.


## Available Tools
- **create_prep_stage**: Inform Deliveroo of order preparation progress
- **create_sync_status**: Notify Deliveroo of POS injection status
- **get_order**: Get details for a single Deliveroo order
- **get_orders**: List Deliveroo orders
- **update_order_status**: Must be called within ~10 minutes of receiving a new order.

Accept, reject, or confirm a Deliveroo order


## Installation & Usage

To install and use the **Deliveroo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deliveroo](https://vinkius.com/mcp/deliveroo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
