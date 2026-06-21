# AgroLog MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agrolog)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/agrolog-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/agrolog-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Access grain monitoring data via AgroLog — monitor temperature, moisture, CO2, crop levels, weather, and control aeration systems from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AgroLog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the temperature and moisture in silo 3 and tell me if there is any spoilage risk."

**🤖 AI Agent:**
> Checking silo 3 sensors... Temperature: 18.5°C (normal, safe storage range). Moisture: 13.2% (within safe limits for grain storage). CO2: 850 ppm (normal, no biological activity detected). Crop level: 72% full. Overall assessment: Grain condition is GOOD — no spoilage risk detected. Temperature is stable and well below the 25°C spoilage threshold. Moisture is below the 15% critical level. Continue routine monitoring. Next aeration check recommended in 48 hours. Would you like to see temperature trends from the past week?

---

**👤 You:**
> "Show me all active alarms in my grain storage facility."

**🤖 AI Agent:**
> Fetching active alarms... Found 2 active alarms. Alarm 1 (CRITICAL): Silo 7 — High Temperature Alert. Temperature reached 28.3°C at 14:32 today, exceeding the 25°C threshold. Immediate aeration recommended. Alarm 2 (WARNING): Bin 3 — Elevated CO2 detected. CO2 levels at 1650 ppm, above the 1500 ppm warning threshold. Monitor closely and consider ventilation. All other bins and silos are within normal parameters. Priority action: Activate aeration for Silo 7 immediately. Would you like me to turn on the fan for Silo 7?

---

**👤 You:**
> "What is the current crop level inventory across all my grain bins?"

**🤖 AI Agent:**
> Checking crop levels across all bins... Silo 1: 85% full (approx. 4,250 tonnes). Silo 2: 62% full (approx. 3,100 tonnes). Silo 3: 72% full (approx. 3,600 tonnes). Silo 4: 45% full (approx. 2,250 tonnes). Silo 5: 91% full (approx. 4,550 tonnes) — approaching capacity. Silo 6: 28% full (approx. 1,400 tonnes). Silo 7: 55% full (approx. 2,750 tonnes). Total estimated inventory: 21,900 tonnes. Silo 5 is approaching maximum capacity — consider planning grain removal soon. Would you like a detailed report with moisture and temperature data for each bin?


## Installation & Usage

To install and use the **AgroLog** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agrolog](https://vinkius.com/mcp/agrolog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
