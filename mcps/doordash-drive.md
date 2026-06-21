# DoorDash Drive MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/doordash-drive)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/doordash-drive-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/doordash-drive-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI agent to manage deliveries, track dashers, and monitor order status via the DoorDash Drive API.

## Description
Integrate **DoorDash Drive**, the white-label delivery fulfillment platform, directly into your AI workflow. Manage your inbound and outbound deliveries, track dasher assignments and real-time ETAs, request delivery quotes, and oversee your fulfillment operations using natural language.

### What you can do

- **Delivery Oversight** — List and retrieve detailed information and real-time status for all your DoorDash fulfillment requests.
- **Logistics Intelligence** — Monitor dasher assignments, live location telemetry, and accurate ETA boundaries for every delivery.
- **Quoting & Planning** — Request instant price and time-of-arrival quotes for potential deliveries based on geographic coordinates.
- **Fulfillment Auditing** — Retrieve high-level summaries of delivery activity, success rates, and active in-progress shipments.

### How it works

1. Connect the DoorDash integration to your AI assistant.
2. Authorize using your DoorDash Developer ID, Key ID, and Signing Secret.
3. Orchestrate your last-mile logistics and delivery fulfillment through intuitive conversation.

### Who is this for?

- **Logistics Managers** — Quickly check delivery statuses and dasher locations on the go.
- **Operations Teams** — Monitor fulfillment volumes and active shipment progress via chat.
- **Customer Support** — Research specific delivery details and ETAs to assist customers instantly.


## Available Tools
- **cancel_active_delivery**: Cancel a delivery that has not yet been picked up
- **create_new_delivery**: Request a new DoorDash delivery (Drive v2)
- **get_doordash_developer_metadata**: Retrieve metadata for the current authenticated developer account
- **get_delivery_details**: Get detailed information and real-time status for a specific delivery
- **quick_delivery_volume_audit**: Retrieve a high-level summary of delivery activity and success rates
- **get_delivery_quote**: Get a price and ETA quote for a potential delivery
- **list_in_progress_deliveries**: Identify deliveries that are currently in progress or out for delivery
- **list_doordash_deliveries**: List all active and recent deliveries in your DoorDash Drive account
- **list_latest_deliveries**: Identify the most recently created or updated deliveries
- **search_deliveries_by_external_id**: Search for a delivery using your own external reference ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DoorDash Drive** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all deliveries currently in progress."

**🤖 AI Agent:**
> I've found 3 deliveries in progress, including 'Order-123' (picked up) and 'Order-456' (dasher confirmed). Would you like to see the ETA for 'Order-123'?

---

**👤 You:**
> "Get a delivery quote from '123 Main St' to '456 Oak Ave'."

**🤖 AI Agent:**
> The delivery quote for this route is $8.50 with an estimated pickup in 15 minutes and delivery in 35 minutes. Would you like the full JSON parameters to create this delivery?

---

**👤 You:**
> "Check the status of delivery 'D-998877'."

**🤖 AI Agent:**
> Delivery 'D-998877' is currently 'Picked Up'. The Dasher (John D.) is 2 miles from the dropoff location with an ETA of 12:45 PM. Should I pull the dasher's contact information?


## Installation & Usage

To install and use the **DoorDash Drive** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/doordash-drive](https://vinkius.com/mcp/doordash-drive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
