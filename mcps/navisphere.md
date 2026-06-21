# Navisphere MCP Server

Automate freight logistics via Navisphere — search available loads, submit bids, track shipments, and manage documentation directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/navisphere)

## Overview
**Category:** shipping-logistics
**Tools Count:** 11

## Description
Connect your **Navisphere** (C.H. Robinson) account to any AI agent to streamline your supply chain and freight operations through natural conversation.

### What you can do

- **Load Discovery** — Search for available freight loads by origin, destination, equipment type (V, R, F, VV), and pickup dates.
- **Bidding & Offers** — Submit pricing bids for specific loads and accept freight offers extended to your carrier account.
- **Shipment Management** — Create new shipments and update statuses (Arrived, Loaded, Departed) with precise location data.
- **Real-time Tracking** — Fetch the latest milestones, ETAs, and tracking events for any active shipment.
- **Digital Documentation** — Upload BOL, POD, and receipts directly to shipments to accelerate billing and compliance.
- **Rate Estimation** — Get instant spot market or contract rate estimates based on lane and equipment data.

### How it works

1. Subscribe to this server
2. Enter your Navisphere Client ID and Client Secret
3. Start managing your logistics pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Carriers & Dispatchers** — Find and bid on loads instantly without switching between multiple web portals.
- **Logistics Coordinators** — Update shipment statuses and upload proof of delivery (POD) via simple voice or text commands.
- **Supply Chain Managers** — Track high-priority shipments and get rate estimates for new lanes in seconds.


## Available Tools
- **accept_offer**: Accept a freight offer
- **create_shipment**: Create a new shipment (Customer API)
- **get_load_details**: Get details for a specific available load
- **get_rate_estimate**: Uses POST under the hood but acts as a query.

Get a rate estimate for a shipment
- **get_tracking_events**: Get high-frequency tracking events for a shipment
- **search_available_loads**: Search for available freight loads
- **submit_bid**: Submit a bid for an available load
- **subscribe_webhooks**: Subscribe to real-time visibility events
- **track_shipment**: Track a customer shipment
- **update_shipment_status**: g., Arrived, Loaded, Departed).

Update the status of an assigned shipment
- **upload_shipment_documents**: Upload documents for a shipment


## Installation & Usage

To install and use the **Navisphere** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/navisphere](https://vinkius.com/mcp/navisphere)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
