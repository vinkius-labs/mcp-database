# Fleetio MCP Server

Manage vehicles, track maintenance, and monitor fuel entries via AI agents with Fleetio.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fleetio)

## Overview
**Category:** erp-operations
**Tools Count:** 12

## Description
Connect your **Fleetio** account to any AI agent and automate your fleet management workflows through the Model Context Protocol (MCP). Fleetio provides a centralized platform for tracking vehicle data, maintenance schedules, fuel consumption, and compliance. Now, you can monitor your fleet operations directly through natural conversation.

### What you can do

- **Vehicle Management** — List all vehicles in your fleet, fetch detailed metadata including VIN and license plates, and retrieve specific vehicle profiles.
- **Maintenance Tracking** — Monitor reported issues, list active work orders, and fetch upcoming service reminders to keep your fleet in top shape.
- **Meter & Data Entry** — Record new odometer or hour meter readings and report new vehicle issues directly from the agent.
- **Fuel Monitoring** — Retrieve historical fuel entries to track consumption and costs across your operations.
- **Directory Access** — List organization contacts (drivers, managers) and vendors/service providers for better team and supplier context.
- **Real-time Monitoring** — Fetch specific maintenance reminders or issue details to ensure operational safety and compliance.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Fleetio API Key and Account Token (found in Settings > Manage API Keys)
3. Start managing your fleet operations from Claude, Cursor, or any MCP client

### Who is this for?

- **Fleet Managers** — quickly check vehicle statuses or upcoming maintenance while planning operations.
- **Operations Supervisors** — get a real-time overview of reported issues and work orders through simple AI commands.
- **Logistics Coordinators** — automate the retrieval of driver contact information and vendor details for faster coordination.


## Available Tools
- **create_issue**: Report a new issue
- **create_meter_entry**: Add vehicle meter reading
- **get_issue**: Get issue details
- **get_service_reminder**: Get reminder details
- **get_vehicle**: Get vehicle details
- **list_contacts**: List fleet contacts
- **list_fuel_entries**: List fuel entries
- **list_issues**: List vehicle issues
- **list_service_reminders**: List service reminders
- **list_vehicles**: List all vehicles
- **list_vendors**: List fleet vendors
- **list_work_orders**: List work orders


## Installation & Usage

To install and use the **Fleetio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fleetio](https://vinkius.com/mcp/fleetio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
