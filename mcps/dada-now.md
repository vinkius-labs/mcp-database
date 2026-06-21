# Dada Now / 达达 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dada-now)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dada-now-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dada-now-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's leading local on-demand delivery platform — manage shops, create orders, and track couriers via AI.

## Description
Empower your AI agent to orchestrate your local logistics and on-demand delivery with **Dada Now** (达达), the premier open delivery platform in China. By connecting Dada to your agent, you transform complex store management, delivery fee estimation, and courier tracking into a natural conversation. Your agent can instantly register new shop stations, calculate real-time delivery costs, place delivery orders, and monitor courier progress without you ever needing to navigate the comprehensive Dada Developer Portal. Whether you are managing e-commerce fulfillment or coordinating local retail shipments, your agent acts as a real-time logistics coordinator, providing accurate and fast results from a single, authorized source.

### What you can do

- **Shop Orchestration** — Register, update, and retrieve detailed metadata for your shop stations across various cities.
- **Order Management** — Create on-demand delivery orders and manage cancellations with specific reason tracking.
- **Fee Auditing** — Query real-time delivery fee estimates based on route distance and cargo value.
- **Courier Tracking** — Monitor the real-time status and contact information of the assigned transporter for any order.
- **Geographic Discovery** — Access the full list of supported cities and their unique city codes for precise routing.

### How it works

1. Subscribe to this server
2. Enter your Dada App Key, App Secret, and Source ID (Merchant ID)
3. Start managing your local logistics through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Merchants** — automate local fulfillment and monitor delivery health through natural language queries.
- **Retail Operations** — manage multiple shop locations and coordinate courier pickups directly from your AI-powered workspace.
- **Developers** — integrate professional on-demand delivery APIs into your AI-driven daily routines.
- **Dada Power Users** — integrate your existing delivery workflows into your AI-driven daily routines.


## Available Tools
- **add_shop**: Register a new shop
- **cancel_order**: Cancel an order
- **create_order**: Create a delivery order
- **get_order_detail**: Get order status
- **get_shop_detail**: Get shop details
- **list_supported_cities**: List supported cities
- **query_delivery_fee**: Query delivery fee
- **update_shop_info**: Update shop metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dada Now / 达达** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the delivery fee for a order from shop 'S001' to '123 Park Ave, Shanghai'."

**🤖 AI Agent:**
> I've calculated the delivery fee. For a 2km trip with a 50 CNY cargo value, the estimated fee is 8.50 CNY. Would you like to proceed and place this order now?

---

**👤 You:**
> "Check the status of Dada order 'ORD88210934'."

**🤖 AI Agent:**
> The status for order `ORD88210934` is 'Transporter Accepted'. The courier, 'Wang Ming', is currently at the shop picking up the items. I'll alert you once he starts the delivery.

---

**👤 You:**
> "Show me the details for shop station 'SH_STORE_01'."

**🤖 AI Agent:**
> I've retrieved the details for shop `SH_STORE_01`. It is currently 'Online' and operating in the Jing'an District of Shanghai. The contact person is 'Zhang Wei'. Would you like me to update any contact information for this station?


## Installation & Usage

To install and use the **Dada Now / 达达** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dada-now](https://vinkius.com/mcp/dada-now)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
