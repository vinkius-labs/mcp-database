# Volvo Cars Connected MCP Server

Monitor and manage your connected Volvo vehicle — check fuel levels, battery status, door locks, and trip statistics directly via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/volvo-cars-connected)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Connect your AI agent to the **Volvo Cars Connected Vehicle API**. This integration allows you to interact with your Volvo vehicle in real-time, retrieving essential telemetry data and status updates through natural conversation.

### What you can do

- **Vehicle Oversight** — List all vehicles associated with your Volvo ID and get detailed metadata for each (VIN, Model, Year)
- **Real-time Status** — Check battery levels for EVs/Hybrids, fuel levels for ICE vehicles, and estimated distance to empty
- **Security Monitoring** — Verify if doors and windows are locked/closed without opening the app
- **Health Checks** — Monitor tire pressure status and engine states across your fleet
- **Operational Metrics** — Retrieve odometer readings and trip statistics to track usage and efficiency

### How it works

1. Subscribe to this server
2. Enter your **Volvo Access Token** (obtained via Volvo ID OAuth) and **VCC API Key**
3. Start managing your vehicle or fleet directly through chat

### Who is this for?

- **Volvo Owners** — quickly check car status while planning your day
- **Fleet Managers** — monitor the health and usage of multiple Volvo vehicles
- **Tech Enthusiasts** — build automated workflows based on real-time vehicle telemetry


## Available Tools
- **get_battery_status**: Retrieve the current battery level and charging status
- **get_doors_status**: Check if doors are locked or unlocked
- **get_engine_status**: Check the current state of the engine
- **get_fuel_status**: Retrieve the current fuel level and range
- **get_odometer**: Retrieve the current odometer reading
- **get_vehicle_statistics**: Retrieve usage statistics and trip meter data
- **get_tires_status**: Check the pressure status of all tires
- **get_vehicle_details**: Get comprehensive metadata for a specific vehicle
- **get_windows_status**: Check if windows are open or closed
- **list_vehicles**: Retrieve a list of all vehicles associated with the Volvo ID


## Installation & Usage

To install and use the **Volvo Cars Connected** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/volvo-cars-connected](https://vinkius.com/mcp/volvo-cars-connected)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
