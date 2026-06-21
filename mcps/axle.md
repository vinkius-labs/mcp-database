# Axle MCP Server

Fleet management and logistics automation — track vehicles, manage drivers, and monitor loads via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/axle)

## Overview
**Category:** shipping-logistics
**Tools Count:** 12

## Description
Empower your AI agent to orchestrate your entire logistics operation with **Axle**, the comprehensive fleet management platform. By connecting Axle to your agent, you transform complex supply chain monitoring into a natural conversation. Your agent can instantly track real-time vehicle locations, audit driver duty statuses, monitor shipment progress, and retrieve essential shipping documents without you ever touching a heavy transportation dashboard. Whether you're managing a local delivery crew or a national trucking network, your agent acts as a real-time dispatch coordinator, ensuring your fleet is always moving and compliant.

### What you can do

- **Vehicle Tracking** — List all vehicles in your fleet and retrieve real-time GPS locations and technical health details.
- **Driver Management** — Audit driver profiles, monitor current duty statuses (On Duty, Driving, etc.), and check available Hours of Service (HOS).
- **Load Orchestration** — Monitor shipment progress, list active loads, and update shipment details dynamically via natural language.
- **Document Retrieval** — Access scanned shipping documents and paperwork associated with specific loads for instant auditing.
- **System Health** — Quickly verify connection status and logistics network integrity directly from your chat interface.

### How it works

1. Subscribe to this server
2. Enter your Axle API Key and Base URL
3. Start managing your fleet operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fleet Managers** — monitor vehicle locations and driver availability in real-time through natural language.
- **Logistics Coordinators** — audit load statuses and verify delivery documentation without manual dashboard logins.
- **Compliance Officers** — perform rapid checks on driver Hours of Service (HOS) to ensure regulatory safety.
- **Operations Leads** — identify shipment bottlenecks and optimize dispatch workflows directly from chat.


## Available Tools
- **get_account_check**: Verify Axle connection and system health
- **get_driver_availability**: Check a driver remaining hours of service (HOS)
- **get_driver**: Get specific profile details for a driver
- **get_load**: Get details for a specific load
- **get_vehicle_location**: Get the last known GPS location of a vehicle
- **get_vehicle**: Get specific details for a single vehicle
- **list_documents**: Retrieve scanned shipping documents associated with shipments
- **list_drivers**: List all drivers in the system
- **list_loads**: List all shipments/loads
- **list_vehicles**: List all vehicles in the fleet
- **update_driver_status**: Update a driver current duty status
- **update_load**: Update a load/shipment details


## Installation & Usage

To install and use the **Axle** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/axle](https://vinkius.com/mcp/axle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
