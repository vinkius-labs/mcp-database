# AgroLog MCP Server

Access grain monitoring data via AgroLog — monitor temperature, moisture, CO2, crop levels, weather, and control aeration systems from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/agrolog)

## Overview
**Category:** iot-hardware
**Tools Count:** 11

## Description
Connect your **AgroLog Grain Monitoring API** to any AI agent and take full control of real-time temperature monitoring, moisture tracking, CO2 spoilage detection, crop level inventory, and automated aeration control through natural conversation.

### What you can do

- **Temperature Monitoring** — Get real-time grain temperature readings from sensors in silos and bins
- **Moisture Tracking** — Monitor grain moisture content for safe storage and drying decisions
- **CO2 Detection** — Detect elevated CO2 levels as early warning signs of spoilage and mold growth
- **Crop Level Inventory** — Track grain volume and silo fill levels for inventory management
- **Weather Station Data** — Access outdoor temperature, humidity, wind speed, and rainfall data
- **Device Management** — List all monitoring devices and view their configuration attributes
- **Relay Control** — Remotely control fans, aeration systems, and dryers connected to AgroLog devices
- **Alarm Monitoring** — Track active alarms and alerts for proactive grain management
- **Historical Telemetry** — Retrieve time-series sensor data for trend analysis and reporting
- **Multi-Customer Management** — Manage devices across multiple farms or customer organizations

### How it works

1. Subscribe to this server
2. Enter your AgroLog credentials (username, password, and base URL)
3. Start monitoring grain conditions from Claude, Cursor, or any MCP-compatible client

No more manual silo inspections or complex monitoring software. Your AI acts as a dedicated grain storage analyst and facility management assistant.

### Who is this for?

- **Grain Farmers** — monitor stored grain conditions, manage aeration, and prevent spoilage remotely
- **Grain Elevator Operators** — track temperature, moisture, and inventory across multiple bins and silos
- **Facility Managers** — oversee grain storage facilities with real-time sensor data and automated controls
- **Agricultural Consultants** — provide data-driven storage management recommendations to clients


## Available Tools
- **set_relay_state**: Accepts device ID, relay name, and desired state (true=on, false=off). Essential for remote grain management, automated ventilation scheduling, and responding to temperature/moisture alerts. AI agents should use this when users ask "turn on the fan for silo 3", "activate aeration for bin 2", or need to remotely control ventilation equipment based on sensor readings. WARNING: Always verify current conditions before changing relay states.

Control relay outputs (fans, aeration, dryers) connected to an AgroLog device
- **get_alarms**: Alarms are triggered by threshold breaches (high temperature, high moisture, elevated CO2, equipment failure) and indicate conditions requiring immediate attention. Returns alarm severity (critical, warning, info), alarm type, affected device, timestamp, and acknowledgment status. Essential for proactive grain management, quality issue detection, and operational response. AI agents should use this when users ask "show me all active alarms", "what alerts have been triggered", or need alarm data for operational monitoring. Optional device_id filters alarms for a specific device.

Get active and historical alarms/alerts from the AgroLog monitoring system
- **get_co2**: Elevated CO2 levels indicate biological activity (mold growth, insect respiration, or grain respiration) and are early warning signs of spoilage before temperature changes become apparent. Returns timestamped CO2 value in ppm. Essential for early spoilage detection, grain quality monitoring, and proactive storage management. AI agents should use this when users ask "what is the CO2 level in silo 2", "check headspace gas readings for device X", or need early warning indicators of grain spoilage.

Get CO2/headspace gas readings from a specific monitoring device
- **get_crop_level**: Crop level sensors measure the grain volume or height in silos and bins, enabling inventory management and capacity planning. Returns timestamped crop level value (percentage or distance). Essential for grain inventory tracking, bin capacity management, and logistics planning. AI agents should reference this when users ask "how full is silo 4", "check crop level for device X", or need inventory data for storage management and logistics planning.

Get grain crop level (volume/quantity) readings from a specific monitoring device
- **get_customer_devices**: Returns device IDs, names, types, and status for the specified customer. Essential for multi-farm management, service provider operations, and organizational device administration. AI agents should use this when users ask "show me all devices for customer X", "list sensors for this farm organization", or need customer-scoped device inventory in multi-tenant deployments.

List all monitoring devices for a specific customer/organization in multi-tenant setups
- **get_device_attributes**: Essential for understanding device setup, sensor positioning within silos, and device management. AI agents should reference this when users ask "show me the configuration for this sensor", "what is the calibration data for device X", or need device metadata for system administration.

Get configuration attributes and metadata for a specific monitoring device
- **get_devices**: Returns device IDs, names, types (temperature sensor, moisture sensor, weather station, crop level monitor, headspace/CO2 sensor), labels, and current status. Essential for device inventory, system overview, and selecting specific sensors for telemetry queries. AI agents should use this when users ask "show me all sensors in my grain silo", "list monitoring devices", or need to identify available devices before querying temperature, moisture, or other telemetry data.

List all AgroLog monitoring devices (temperature, moisture, weather sensors) in your system
- **get_moisture**: Moisture content is the most critical factor for safe grain storage — high moisture leads to mold, spoilage, and heating. Returns timestamped moisture value as percentage. Essential for grain quality assessment, drying decisions, and storage safety monitoring. AI agents should reference this when users ask "what is the moisture level in bin 5", "check grain moisture for device X", or need moisture data for storage management and drying planning.

Get current grain moisture readings from a specific monitoring device
- **get_device_telemetry**: Supports custom key selection (temperature, moisture, co2, humidity, etc.) and configurable data point limits for historical analysis. Essential for trend analysis, condition monitoring over time, and creating data visualizations. AI agents should reference this when users ask "show me temperature history for device X over the last 48 hours", "get moisture trend for this sensor", or need historical telemetry data for grain management analysis.

Get time-series telemetry data from a specific monitoring device with customizable keys and limits
- **get_temperature**: Temperature is critical for detecting spoilage, mold growth, and insect activity in stored grain. Returns timestamped temperature value in Celsius. Essential for grain quality monitoring, spoilage prevention, and ventilation scheduling. AI agents should use this when users ask "what is the temperature in silo 3", "check grain temperature for device X", or need current temperature data for storage management decisions. Device IDs can be found using get_devices.

Get current grain temperature readings from a specific monitoring device
- **get_weather**: Essential for drying decisions (outdoor air conditions for natural air drying), harvest planning (rain forecasts, wind conditions), and understanding environmental impact on stored grain. Returns the latest 10 readings with timestamps. AI agents should use this when users ask "what are the current weather conditions at my facility", "show me wind speed and rainfall data", or need weather context for grain management decisions.

Get weather station data (temperature, humidity, wind, rainfall) from a specific device


## Installation & Usage

To install and use the **AgroLog** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agrolog](https://vinkius.com/mcp/agrolog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
