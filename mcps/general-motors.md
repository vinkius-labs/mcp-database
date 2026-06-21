# General Motors MCP Server

AI connected car: control GM vehicles, check diagnostics, and track location via agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/general-motors)

## Overview
**Category:** industry-titans
**Tools Count:** 14

## Description
### What you can do

Connect AI agents to the General Motors Connected Vehicle API for comprehensive car management:

- **List registered vehicles** to manage fleets or personal garages
- **Track GPS location** to find parked cars or monitor fleet movement
- **Monitor diagnostics** including oil life, battery voltage, and check engine status
- **Check EV charge levels** and estimated range for electric vehicles
- **Lock and unlock doors** remotely for security or guest access
- **Start and stop engines** remotely to pre-condition cabin temperature
- **Flash lights and sound horn** to locate vehicles in crowded areas
- **Send navigation destinations** directly to the infotainment system

### How it works

1. **Register at GM Developer Portal** and create an application
2. **Authenticate via OAuth** to obtain an access token for your vehicle
3. **Ask your AI agent** to check status, run diagnostics, or send commands
4. **Natural language commands** replace the myChevrolet/OnStar app navigation

### Who is this for?

Perfect for **GM vehicle owners**, **fleet managers**, **service advisors**, and **roadside assistance teams**. Let AI agents automate morning warm-ups, monitor tire pressure for safety, track mileage for maintenance schedules, and locate vehicles. Ideal for drivers who want to integrate their car into their smart home or AI assistant workflow for seamless mobility management.


## Available Tools
- **flash_horn**: Requires VIN. Use this to locate a vehicle in a crowded parking lot or driveway.

Trigger the horn of a GM vehicle to locate it
- **flash_lights**: Requires VIN. Use this to locate a vehicle in the dark or signal ownership.

Flash the headlights and taillights of a GM vehicle
- **get_charge_status**: Requires VIN. Use this to manage EV range anxiety or schedule charging during off-peak hours.

Get the charging status and battery level of a GM EV (Bolt, Ultium, etc)
- **get_vehicle_diagnostics**: Requires VIN. Use this for maintenance scheduling, pre-trip inspections, or health monitoring.

Get comprehensive diagnostic data for a GM vehicle
- **get_fuel_level**: Requires VIN. Use this to plan refueling stops or monitor fuel economy.

Get the current fuel tank level of a GM vehicle
- **get_vehicle_location**: Requires VIN. Use this to find your parked car, track fleet assets, or verify vehicle movement.

Get the current GPS location of a specific GM vehicle
- **get_odometer**: Requires VIN. Use this to track service intervals, lease mileage limits, or fleet utilization.

Get the current mileage (odometer reading) of a GM vehicle
- **get_tire_pressure**: Requires VIN. Use this to identify leaks, ensure safety, or prepare for long trips.

Get the current tire pressure readings for all four tires
- **get_vehicles**: Use this as the first step to identify which VIN to use for commands or diagnostics.

List all GM vehicles associated with the account
- **lock_doors**: Requires VIN. Returns command status (success/failed/in-progress). Use this to secure the vehicle after parking or if you forgot to lock it.

Lock the doors of a specific GM vehicle remotely
- **send_turn_by_turn**: Requires VIN and a destination object with latitude, longitude, and address. Use this to plan a trip on your phone and have it ready in the car.

Send a destination to the vehicle's built-in navigation system
- **start_vehicle**: Requires VIN. Returns command status. Use this to warm up the car in winter or cool it down in summer before entering.

Remotely start the engine of a GM vehicle
- **stop_vehicle**: Requires VIN. Returns command status. Use this to cancel a remote start if the vehicle is now in use or if there is a safety concern.

Remotely stop the running engine of a GM vehicle
- **unlock_doors**: Requires VIN. Returns command status. Use this to let a passenger in or if keys are locked inside.

Unlock the doors of a specific GM vehicle remotely


## Installation & Usage

To install and use the **General Motors** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/general-motors](https://vinkius.com/mcp/general-motors)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
