# PurpleAir MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/purpleair)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Real-time air quality monitoring — access PM2.5, temperature, and pollution data from 50K+ sensors worldwide via AI.

## Description
Access the world's largest hyperlocal air quality dataset through **PurpleAir** — a global network of over 50,000 low-cost air quality sensors measuring PM2.5, PM10.0, temperature, humidity, pressure, and more. Connect PurpleAir to your AI agent to monitor real-time air quality, track wildfire smoke, analyze pollution trends, and access historical data for any location — all through natural conversation.

### What you can do

- **Real-Time Air Quality** — Get current PM2.5 readings from sensors near any address or coordinate.
- **Historical Analysis** — Retrieve time-series data for trend analysis, pollution events, and compliance reporting.
- **Geographic Mapping** — Find all sensors within a bounding box for city-wide or regional air quality mapping.
- **Wildfire Smoke Tracking** — Monitor PM2.5 spikes during wildfire events across affected areas.
- **Indoor Air Quality** — Access indoor sensor data for workplace health and HVAC optimization.
- **CSV Export** — Download historical data in CSV format for spreadsheet analysis.
- **Location-Based Queries** — Find the closest sensor to any GPS coordinate.
- **Sensor Filtering** — Filter sensors by type (indoor/outdoor), fields, and update recency.

### How it works

1. Subscribe to this server
2. Enter your PurpleAir API Read Key
3. Start querying air quality data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Environmental Scientists** — track pollution trends and validate air quality models.
- **Public Health Officials** — issue health advisories during poor air quality events.
- **Wildfire Response Teams** — monitor smoke impacts in real-time across affected communities.
- **Real Estate Professionals** — assess air quality for property evaluations.


## Available Tools (10)
- **get_indoor_sensors**: These sensors measure air quality inside buildings, homes, and enclosed spaces. Useful for indoor air quality assessments, HVAC monitoring, and workspace health studies.

Get all indoor PurpleAir sensors
- **get_outdoor_sensors**: These are sensors measuring ambient outdoor air quality. Returns current PM2.5, temperature, humidity and other measurements for each sensor. Useful for regional air quality monitoring, wildfire smoke tracking, and urban pollution studies.

Get all outdoor (outside) PurpleAir sensors
- **get_pm25_sensors**: 5 (fine particulate matter) measurements. PM2.5 is the most important air quality indicator — particles smaller than 2.5 micrometers that can penetrate deep into lungs and bloodstream. Returns current PM2.5 concentrations along with location data. Essential for health advisories, wildfire smoke tracking, and urban pollution monitoring.

Get sensors with PM2.5 measurements
- **get_sensor_data**: Returns PM2.5, PM1.0, PM10.0 particle concentrations, temperature, humidity, pressure, VOC levels, and other measurements depending on the sensor model. Use the fields parameter to specify which measurements to return. Essential for monitoring air quality at a specific location.

Get real-time data from a specific PurpleAir sensor
- **get_sensor_history**: Returns time-series data for the requested fields (PM2.5, temperature, humidity, etc.) at regular intervals. Use start_timestamp and end_timestamp (Unix timestamps) to define the time range. The average parameter controls data aggregation (e.g. 60 for 1-minute averages, 3600 for hourly). Essential for analyzing air quality trends, identifying pollution events, and compliance reporting.

Get historical air quality data from a PurpleAir sensor
- **get_sensor_history_csv**: Same functionality as get_sensor_history but returns data as CSV instead of JSON. Use for offline analysis, charting, or compliance reporting. Requires start_timestamp and end_timestamp parameters.

Get historical sensor data in CSV format for analysis
- **get_sensors_by_bounding_box**: Provide the northwest (nwlat, nwlng) and southeast (selat, selng) corner coordinates. Perfect for mapping air quality across a city, neighborhood, or region. Returns all sensors in the area with current readings. Use with fields parameter to customize returned data.

Get all sensors within a geographic bounding box
- **get_sensors_by_index**: Provide comma-separated sensor indices in the show_only parameter. Useful when you already know the sensor indices from a previous query and want to get fresh readings without fetching all sensors.

Get data for specific sensor(s) by their indices
- **get_sensors_near_me**: Internally uses a bounding box around the point to find nearby sensors. Useful for identifying the closest PurpleAir monitor to any address or coordinate. Returns sensors sorted by proximity with current air quality readings.

Find PurpleAir sensors near a specific location
- **list_sensors**: Use the location_type parameter to filter by sensor type (outside=0, inside=1). Use the fields parameter to specify which data fields to return (e.g. name,latitude,longitude,pm2.5_atm,temperature,humidity). By default returns basic sensor info. Use show_only to filter by specific sensor indices (comma-separated). Use modified_since (Unix timestamp) to get only sensors updated after a specific time. Results include sensor metadata and real-time air quality measurements.

List PurpleAir air quality sensors with optional filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PurpleAir** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the air quality near San Francisco right now?"

**🤖 AI Agent:**
> I found 23 outdoor sensors in the San Francisco area. Current PM2.5 readings range from 3.2 to 18.7 µg/m³, with an average of 8.4 µg/m³ — Moderate air quality. The highest reading is in the Bayview district. Here are the sensor locations and readings.

---

**👤 You:**
> "Show me the PM2.5 trend for sensor 12345 over the last 24 hours."

**🤖 AI Agent:**
> I retrieved hourly PM2.5 data for sensor 12345 over the past 24 hours. PM2.5 started at 5.1 µg/m³, peaked at 42.3 µg/m³ at 2pm (likely wildfire smoke), and has been decreasing to 12.8 µg/m³ currently. Here's the full time series.

---

**👤 You:**
> "Find all outdoor sensors in Los Angeles and show me their PM2.5 readings."

**🤖 AI Agent:**
> I found 47 outdoor sensors in the Los Angeles area. PM2.5 readings range from 4.1 to 35.6 µg/m³. Areas near freeways show higher readings (15-35 µg/m³) while coastal areas are cleaner (4-8 µg/m³). Here's the complete map with readings.


## ❓ FAQ

**Q: How do I find air quality near my address?**
Use the `get_sensors_near_me` tool with your latitude and longitude. Alternatively, search for sensors by bounding box using `get_sensors_by_bounding_box` with corner coordinates. The API will return nearby sensors with current PM2.5, temperature, and humidity readings.

**Q: Can I get historical air quality data?**
Yes. Use `get_sensor_history` with a sensor index and time range (Unix timestamps). You can specify which fields to retrieve (PM2.5, temperature, humidity) and set an averaging interval (e.g. 3600 for hourly averages). For spreadsheet analysis, use `get_sensor_history_csv` to get data in CSV format.

**Q: What does PM2.5 mean and why is it important?**
PM2.5 refers to fine particulate matter smaller than 2.5 micrometers — about 30 times smaller than a human hair. These particles can penetrate deep into lungs and enter the bloodstream, causing respiratory and cardiovascular health effects. The WHO guideline is 5 µg/m³ annual average. PurpleAir sensors measure PM2.5 in real-time, making them essential for health advisories and pollution monitoring.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/purpleair](https://vinkius.com/mcp/purpleair)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PurpleAir** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `purpleair` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PurpleAir** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "purpleair": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
