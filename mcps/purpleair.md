# PurpleAir MCP Server

Real-time air quality monitoring — access PM2.5, temperature, and pollution data from 50K+ sensors worldwide via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/purpleair)

## Overview
**Category:** iot-hardware
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **PurpleAir** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/purpleair](https://vinkius.com/mcp/purpleair)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
