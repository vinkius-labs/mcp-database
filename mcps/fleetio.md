# Fleetio MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fleetio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fleetio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fleetio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage vehicles, track maintenance, and monitor fuel entries via AI agents with Fleetio.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fleetio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active vehicles in my fleet and their current status."

**🤖 AI Agent:**
> Fetching vehicles... I found 10 active vehicles, including 'Truck 01' (Status: Active) and 'Van 05' (Status: In Shop). Would you like to see the details for any of these?

---

**👤 You:**
> "Record a new odometer reading of 50,000 for vehicle ID 'veh_123'."

**🤖 AI Agent:**
> Meter entry recorded! I've added an odometer reading of 50,000 to vehicle 'veh_123'. Your maintenance schedules will be updated based on this new data.

---

**👤 You:**
> "Show me all upcoming service reminders."

**🤖 AI Agent:**
> Retrieving reminders... You have 3 upcoming services: 'Oil Change' for Truck 01 (Due in 500 miles), 'Tire Rotation' for Van 02 (Due in 2 days), and 'Annual Inspection' for Truck 03.


## Installation & Usage

To install and use the **Fleetio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fleetio](https://vinkius.com/mcp/fleetio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
