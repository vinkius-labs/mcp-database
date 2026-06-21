# GoFood MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gofood)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gofood-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gofood-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate GoFood merchant operations — manage outlets, menus, orders, promos, and payments directly from any AI agent.

## Description
Connect your **GoFood/GoBiz** merchant account to any AI agent and take full control of your food delivery and POS integration through natural conversation.

### What you can do

- **Outlet Management** — List, link, and unlink merchant outlets; retrieve detailed outlet configuration and properties
- **Menu & Catalog** — Fetch complete menu catalogs, update items, and manage stock levels for menu items and variants
- **Order Processing** — Accept, cancel, and mark orders as prepared with full order type support
- **Promotions** — Create, list, deactivate, and delete promotional campaigns for specific outlets
- **Webhooks** — Set up notification subscriptions for real-time event monitoring
- **Payments** — Create payment transactions with reference tracking

### How it works

1. Subscribe to this server
2. Enter your GoBiz OAuth 2.0 JWT Bearer token
3. Start managing your GoFood merchant operations from Claude, Cursor, or any MCP-compatible client

No more juggling between multiple dashboards to check order status or update menu availability. Your AI acts as a dedicated GoFood operations manager.

### Who is this for?

- **Restaurant Owners** — instantly manage outlet catalogs, update stock levels, and process incoming orders without opening the GoBiz dashboard
- **POS Integrators** — automate outlet linking, menu synchronization, and webhook configuration for multi-location deployments
- **Operations Teams** — monitor promo campaigns, handle order lifecycle management, and track payment transactions from a single conversational interface


## Available Tools
- **accept_order**: Accept a pending GoFood order
- **cancel_order**: Cancel a GoFood order
- **create_promo**: Create a new promo for a GoFood outlet
- **get_catalog**: Get the full menu catalog for a GoFood outlet
- **get_outlet_info**: Get details for a specific GoFood outlet
- **link_outlet**: Link a GoFood outlet to the integration
- **list_linked_outlets**: List all linked GoFood outlets
- **list_promos**: List all promos for a GoFood outlet
- **mark_order_prepared**: Mark a GoFood order as food prepared
- **unlink_outlet**: Unlink a GoFood outlet from the integration
- **update_catalog**: Update the menu catalog for a GoFood outlet
- **update_menu_stocks**: Update menu item stock levels for a GoFood outlet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GoFood** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my linked GoFood outlets."

**🤖 AI Agent:**
> I've fetched your linked outlets. You currently have 3 outlets connected: 'Nasi Goreng Sudirman' (ID: out_001), 'Bakso Senayan' (ID: out_002), and 'Mie Ayam Thamrin' (ID: out_003). Which outlet would you like to manage?

---

**👤 You:**
> "Show me the full menu catalog for outlet out_001."

**🤖 AI Agent:**
> Retrieving catalog... The outlet 'Nasi Goreng Sudirman' has 24 menu items across 5 categories. Top sellers include 'Nasi Goreng Spesial' (Rp 25,000) and 'Ayam Geprek' (Rp 20,000). Would you like to check stock levels or update any item?

---

**👤 You:**
> "Accept order ORD-12345 for outlet out_001, type food."

**🤖 AI Agent:**
> Order ORD-12345 has been successfully accepted and is now being processed at 'Nasi Goreng Sudirman'. The kitchen has been notified. Would you like me to mark it as prepared once cooking is done?

---

**👤 You:**
> "Create a 20% discount promo for outlet out_001 valid this weekend."

**🤖 AI Agent:**
> Promo created successfully! The 20% discount campaign is now active for 'Nasi Goreng Sudirman' and will run through the weekend. Customers will see the offer when browsing your GoFood listing.


## Installation & Usage

To install and use the **GoFood** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gofood](https://vinkius.com/mcp/gofood)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
