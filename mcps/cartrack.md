# Cartrack MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cartrack)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cartrack-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cartrack-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Manage fleet operations via Cartrack — track vehicle locations, monitor fuel, and analyze trip history directly from any AI agent.

## Description
Connect your **Cartrack** fleet account to any AI agent and take full control of your telematics data and vehicle tracking through natural conversation. Optimize your fleet management and driver safety.

### What you can do

- **Live Tracking** — Retrieve the real-time GPS position and basic status of any vehicle in your fleet natively
- **Fleet Overview** — List all registered vehicles and drivers to get a complete organizational snapshot
- **Trip Intelligence** — Analyze historical trip data, including routes and driving behavior flawlessly
- **Fuel Monitoring** — Monitor fuel levels and consumption metrics to identify inefficiencies securely
- **Alert Oversight** — List and review fleet alerts such as speeding, idling, or geofence breaches in real-time
- **Geofence Mapping** — Access details on all configured geofences to manage operational boundaries

### How it works

1. Subscribe to this server
2. Enter your Cartrack Username, Password, and regional API Base URL
3. Start managing your fleet telematics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fleet Managers** — track vehicle locations and monitor driver alerts using natural language
- **Operations Coordinators** — audit trip histories and fuel usage without opening the complex dashboard
- **Safety Officers** — identify speeding incidents and driving behavior alerts straight from their chat interface
- **Logistics Teams** — quickly verify vehicle availability and geofence statuses for route planning


## Available Tools
- **get_fuel_status**: Get current fuel levels and consumption for a vehicle
- **get_vehicle_position**: Get the real-time GPS position of a specific vehicle
- **get_vehicle_details**: Get detailed information for a specific vehicle
- **list_fleet_alerts**: List recent fleet alerts and events (speeding, etc)
- **list_fleet_drivers**: List all registered drivers in the fleet
- **list_geofences**: List all configured geofences for the fleet
- **list_vehicle_trips**: List historical trips for a specific vehicle
- **list_vehicles**: List all vehicles in the fleet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cartrack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where is vehicle with registration 'ABC-123' currently?"

**🤖 AI Agent:**
> Checking location for 'ABC-123'... The vehicle is currently located at 123 Main Street, Johannesburg, and its status is 'Idling'.

---

**👤 You:**
> "Show me the trip history for vehicle ID 999 for yesterday."

**🤖 AI Agent:**
> Retrieving trips for vehicle 999... I found 4 trips yesterday. The longest was 45km, starting at 08:30 AM and ending at 09:45 AM. Would you like to see the route details?

---

**👤 You:**
> "Check the fuel levels for my entire fleet."

**🤖 AI Agent:**
> Scanning fleet fuel status... Most vehicles are above 70%. However, vehicle 'XYZ-789' is low at 12%. Should I notify the driver?


## Installation & Usage

To install and use the **Cartrack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cartrack](https://vinkius.com/mcp/cartrack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
