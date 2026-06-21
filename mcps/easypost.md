# EasyPost MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/easypost)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/easypost-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/easypost-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage shipments, track packages, and monitor carrier accounts via the EasyPost API.

## Description
Integrate **EasyPost**, the leading shipping API for e-commerce, directly into your AI workflow. Manage your outbound shipments and carrier rates, track packages in real-time with detailed event logs, monitor your connected carrier accounts (UPS, FedEx, USPS, etc.), and oversee your shipping addresses using natural language.

### What you can do

- **Shipment Oversight** — List and retrieve detailed information, rates, and carrier options for all your logistics shipments.
- **Real-time Tracking** — Monitor active trackers, resolving real-time transit statuses, checkpoint events, and estimated delivery dates.
- **Carrier Management** — Access and monitor all connected carrier accounts, verifying active service capability boundaries across your fleet.
- **Delivery Auditing** — Retrieve high-level summaries of shipment activity, success rates, and identify packages currently in transit.

### How it works

1. Connect the EasyPost integration to your AI assistant.
2. Authorize using your EasyPost API Key (found in your dashboard).
3. Orchestrate your shipping operations and delivery tracking through intuitive conversation.

### Who is this for?

- **E-commerce Managers** — Quickly check shipment statuses and delivery success rates on the go.
- **Logistics Teams** — Monitor in-transit packages and carrier performance via chat.
- **Customer Support** — Research specific tracking codes and delivery events to assist customers instantly.


## Available Tools
- **get_easypost_account_metadata**: Retrieve metadata and usage limits for your EasyPost account
- **list_carrier_accounts**: List all connected carrier accounts (e.g. UPS, FedEx, USPS)
- **quick_delivery_health_audit**: Retrieve a high-level summary of shipment activity and delivery success rates
- **get_shipment_details**: Get detailed information and rates for a specific shipment
- **get_tracking_details**: Get real-time tracking events and status for a specific tracker
- **list_in_transit_packages**: Identify shipments that are currently in transit with a carrier
- **list_latest_shipments**: Identify the most recently created shipments
- **list_shipping_shipments**: List all shipments created in your EasyPost account
- **list_active_trackers**: List all active tracking objects in your account
- **search_by_tracking_code**: Search for a tracker using a specific tracking code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EasyPost** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active package trackers."

**🤖 AI Agent:**
> I've found several active trackers, including codes for FedEx and UPS. 3 packages are 'In Transit' and 1 is 'Out for Delivery'. Would you like to see the details for the package out for delivery?

---

**👤 You:**
> "Show me the details for shipment 'shp_998877'."

**🤖 AI Agent:**
> Shipment 'shp_998877' is currently 'Label Purchased'. It has 3 available rates from USPS and UPS. The lowest rate is $7.50 via USPS Ground Advantage. Should I pull the full carrier rate list?

---

**👤 You:**
> "Which carrier accounts are connected to my account?"

**🤖 AI Agent:**
> Your account has 4 connected carrier accounts: 'USPS' (Active), 'FedEx' (Active), 'UPS' (Active), and 'DHL Express' (Pending Configuration). Would you like to see the account credentials for any of these?


## Installation & Usage

To install and use the **EasyPost** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/easypost](https://vinkius.com/mcp/easypost)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
