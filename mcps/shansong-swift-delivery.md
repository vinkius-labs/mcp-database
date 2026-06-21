# Shansong Swift Delivery MCP Server

Bring Shansong's fast P2P Delivery Network into your LLM. Estimate logistics routing, dispatch riders, and track locations.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/shansong-swift-delivery)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Equip your AI Agents with the **Shansong (闪送)** infrastructure logic, bringing one of the fastest Point-to-Point delivery APIs locally into your environment. Through 10 dedicated management extensions, your LLMs can govern entire delivery routes, request estimates, and interact dynamically with local couriers.

### What you can do

- **Live GPS Polling** — Instruct your agent to find where the driver is currently located using `query_rider_position`
- **Dispatch Generation** — Check prices via `calculate_fee` and officially submit `create_order` payloads dynamically
- **Rider Feedback** — Cancel routing autonomously or distribute `add_tip` commands on-demand without touching administrative dashboards

### How it works

1. Sign up on the [Shansong Open Platform](https://open.ishansong.com/)
2. Register an application and note down your **Client ID**, **App Secret**, and your default **Shop ID**
3. Push these variables into Vurb. The Node extension strictly generates the `Sign` string by converting your JSON into an MD5 Hash required by their network implicitly.

### Who is this for?

- **Retail AI Support Centers** — Handle customer 'Where is my order?' queries automatically by fetching live GPS data directly in chat contexts
- **Office Coordinators** — Empower internal company slackbots to dispatch official documents point-to-point instantly


## Available Tools
- **add_tip**: Add a tip to encourage driver pickup
- **calculate_fee**: Calculate delivery fee dynamically
- **cancel_order**: Cancel a delivery dispatch
- **confirm_goods**: Confirm the goods were successfully picked up
- **create_order**: Create a new Shansong delivery order
- **query_city_list**: Get available active operating Cities on Shansong
- **query_order_info**: Get live order status details
- **query_rider_position**: Get live GPS coordinates of the Shansong Rider
- **query_store_list**: Get available Stores within a specific City
- **submit_complaint**: Submit complaint against assigned rider


## Installation & Usage

To install and use the **Shansong Swift Delivery** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shansong-swift-delivery](https://vinkius.com/mcp/shansong-swift-delivery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
