# Lalamove Malaysia MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lalamove-malaysia)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lalamove-malaysia-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lalamove-malaysia-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [transportation](../categories/transportation.md)

Orchestrate Lalamove Malaysia deliveries — get quotations, manage orders, and track drivers directly from any AI agent.

## Description
Connect your AI agents to **Lalamove Malaysia**, the leading on-demand delivery platform. This MCP provides 10 tools to automate delivery quotations, orchestrate shipment orders, and track driver status in real-time directly through natural conversation.

### What you can do

- **Delivery Quotation** — Get real-time price estimates for various vehicle types based on pickup and drop-off locations
- **Order Management** — Create, cancel, and retrieve shipment orders programmatically using the official API
- **Driver Tracking** — Monitor driver assignments, contact details, and real-time GPS locations for active deliveries
- **City Intelligence** — Verify service availability and list supported cities within the Lalamove Malaysia network
- **Market Transparency** — Access granular fee breakdowns, including base fares and surcharges, for any delivery task

### How it works

1. Subscribe to this server
2. Register for a [**Lalamove Partner Account**](https://partner.lalamove.com/)
3. Navigate to **API Settings** to obtain your **API Key** and **API Secret**
4. Identify your **Base URL** (Production or Sandbox)
5. Insert your credentials into the fields below to start managing your Malaysian deliveries.

### Who is this for?

- **E-commerce Developers** — automate the integration of on-demand local delivery into Malaysian storefronts
- **Operations Managers** — monitor large volumes of active deliveries and driver statuses via natural language
- **Logistics Coordinators** — quickly provide shipping estimates and track mission-critical parcels


## Available Tools
- **add_priority_fee**: Add a priority fee (tip) to an order
- **cancel_order**: Cancel an active delivery order
- **get_driver_details**: Get information about the assigned driver
- **get_driver_location**: Get real-time GPS location of the assigned driver
- **get_order_details**: Get details for a specific order
- **get_price_breakdown**: Retrieve detailed price breakdown for a quotation
- **get_quotation**: Returns a quotationId and price breakdown.

Get a delivery quotation
- **list_city_info**: List supported cities and service types
- **list_vehicle_info**: List available vehicle types
- **place_order**: Place a new delivery order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lalamove Malaysia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get a Lalamove quote for a motorcycle from 'KLCC' to 'Petaling Jaya'."

**🤖 AI Agent:**
> Retrieving Lalamove quotation... For a motorcycle from KLCC to Petaling Jaya (Approx. 12km), the estimated fare is RM 15.00. This includes basic insurance. Would you like to proceed with the order?

---

**👤 You:**
> "Track my active Lalamove order 'ord_123456789'."

**🤖 AI Agent:**
> Connecting to Lalamove tracking... Your order 'ord_123456789' is currently 'In Progress'. Driver: Ahmad (ID: drv_777) is 5 minutes away from the drop-off point. Would you like me to send you the GPS tracking link?

---

**👤 You:**
> "Cancel my Lalamove order ID 'ord_999888777'."

**🤖 AI Agent:**
> Processing cancellation request... Success! Order 'ord_999888777' has been cancelled. Please note that cancellation fees may apply based on the driver's current location.


## Installation & Usage

To install and use the **Lalamove Malaysia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lalamove-malaysia](https://vinkius.com/mcp/lalamove-malaysia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
