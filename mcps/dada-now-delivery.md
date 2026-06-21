# Dada Now Delivery MCP Server

Bring Dada Now's Instant Local Delivery API to your LLM. Schedule swift deliveries, manage your stores, and calculate routing fees.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dada-now-delivery)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Integrate **Dada Now (达达快送)**, one of the leading on-demand delivery platforms, tightly into your AI. With 10 full-scale fleet administration and logistics tools embedded, your AI model can function as an autonomous fleet coordinator for P2P deliveries.

### What you can do

- **Create Deliveries on the Fly** — Simply tell the AI where to send the goods and it will evaluate the `query_order_fee` alongside `add_order` instantly
- **Interactive Routing** — Add rider 'tips' during peak rush-hour dynamically, or complain against delays on the dashboard automatically
- **Store Management** — Create new delivery pickup hubs (Shop registration) directly via conversational prompts

### How it works

1. Sign up on the Dada Now Developer Program to receive an **App Key**, **App Secret**, and Merchant **Source ID**
2. Add them safely into Vurb
3. The backend encapsulates the required `MD5 Signature` rules alongside timestamps so your LLM doesn't have to navigate cryptography.

### Who is this for?

- **E-commerce Chatbots** — Directly dispatch local couriers from customer conversations without hitting backend servers
- **Operations Teams** — Give non-technical logistics staff the ability to control Dada dashboards via natural language


## Available Tools
- **add_complaint**: Submit a complaint about a driver
- **add_order**: Create a new Dada delivery order
- **add_shop**: Register a new Store/Shop to pick up from
- **add_tip**: Add a monetary tip to a specific delivery order
- **cancel_order**: Cancel a delivery dispatch
- **get_city_code**: Retrieve Dada City Codes
- **query_order_fee**: Estimate the delivery fee before ordering
- **query_order_status**: Get live tracking status of an order
- **readd_order**: Re-add an expired or failed delivery order
- **update_shop**: Update existing Station details


## Installation & Usage

To install and use the **Dada Now Delivery** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dada-now-delivery](https://vinkius.com/mcp/dada-now-delivery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
