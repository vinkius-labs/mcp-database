# Deliveroo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deliveroo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/deliveroo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/deliveroo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage Deliveroo restaurant orders — accept deliveries, track preparation stages, and sync POS status directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deliveroo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all live orders for restaurant ID 'REST123'."

**🤖 AI Agent:**
> I've retrieved the live orders for REST123. There are currently 3 active orders: #ABC-1, #ABC-2, and #ABC-3. Would you like details for any of these?

---

**👤 You:**
> "Accept order 'ORD-999' and set its stage to 'in_kitchen'."

**🤖 AI Agent:**
> Order 'ORD-999' has been successfully accepted and the preparation stage is now updated to 'in_kitchen'.

---

**👤 You:**
> "Notify Deliveroo that order 'ORD-456' failed to sync with the POS because items are out of stock."

**🤖 AI Agent:**
> I've sent the sync status update for order 'ORD-456'. It is marked as 'failed' with the reason: 'items_out_of_stock'.


## Installation & Usage

To install and use the **Deliveroo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deliveroo](https://vinkius.com/mcp/deliveroo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
