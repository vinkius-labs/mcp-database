# Kargo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kargo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kargo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kargo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Automate logistics and loading dock operations via Kargo — track shipments and sync data directly from your AI agent.

## Description
Connect your **Kargo** logistics account to your AI agent and optimize your supply chain and loading dock operations through natural conversation.

### What you can do

- **Shipment Tracking** — List all shipments for your facility and get real-time status updates and carrier info.
- **Order Management** — Access facility-wide customer orders and their current status.
- **Deep Inspection** — Fetch complete metadata for specific shipments or orders using their unique numbers.
- **Data Synchronization** — Push order and shipment payload data directly to Kargo's Unified Endpoint to keep systems in sync.
- **Facility & Device Oversight** — List all business facilities and monitor the status of active IoT devices (cameras, sensors).
- **Audit Logs** — Review the history of data payloads pushed to the platform.

### How it works

1. Subscribe to this server
2. Enter your Kargo API Token, Business Slug, and Facility Slug
3. Start managing your logistics from Claude, Cursor, or any MCP client

### Who is this for?

- **Logistics Coordinators** — instantly check shipment statuses or carrier contact details without manually searching the dashboard.
- **Warehouse Operations** — monitor scheduled departures and IoT device health straight from your communication tool.
- **IT & Supply Chain Managers** — automate data synchronization and audit payload logs through natural language.


## Available Tools
- **get_carrier_info**: Get carrier contact info
- **get_device_status**: Get specific device status
- **get_order**: Get specific order details
- **get_shipment**: Get specific shipment details
- **list_devices**: List facility IoT devices
- **list_facilities**: List all business facilities
- **list_orders**: List facility orders
- **list_payload_logs**: List sync payload logs
- **list_shipments**: List all shipments at the facility
- **update_logistics**: Sync data to Kargo Unified Endpoint


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kargo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active shipments for my facility."

**🤖 AI Agent:**
> I've retrieved the current shipments. You have 4 active shipments: 'SHP-1001' (Carrier: Swift Logistics, Status: At Dock) and 3 others scheduled for later today. Would you like the details for SHP-1001?

---

**👤 You:**
> "Check the status of all IoT devices in the facility."

**🤖 AI Agent:**
> I've checked your IoT fleet. You have 12 devices registered: 10 are 'online' and functioning correctly, while 2 (ID: CAM-04 and ID: SNSR-09) are currently 'offline'. Shall I retrieve the last-seen data for the offline devices?

---

**👤 You:**
> "Get details for shipment number SHP-2024-05."

**🤖 AI Agent:**
> Inspecting SHP-2024-05... This shipment is handled by 'Global Freight' and is scheduled to depart at 4:30 PM. It contains 2 orders: #ORD-99 (Customer: Acme Corp) and #ORD-102 (Customer: RetailPlus).


## Installation & Usage

To install and use the **Kargo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kargo](https://vinkius.com/mcp/kargo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
