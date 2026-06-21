# OpenAQ MCP Server

Access global air quality data — monitor PM2.5, O3, NO2 levels and track pollution via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/openaq)

## Overview
**Category:** data-analytics
**Tools Count:** 9

## Description
Connect **OpenAQ**, the world's largest open air quality database, to any AI agent and monitor real-time pollution levels, track air quality trends, and access data from thousands of monitoring stations globally through natural language.

### What you can do

- **Live Monitoring** — Get the latest PM2.5, O3, NO2, SO2, and CO readings from any location worldwide
- **Historical Analysis** — Query time-series measurement data with date range filters for trend analysis
- **Location Discovery** — Browse monitoring stations by country, city, or geographic area
- **Sensor Tracking** — View active sensor devices and their measurement parameters
- **Parameter Reference** — Look up all measurable air quality parameters with units and classifications
- **Global Coverage** — Access data from 100+ countries with thousands of active monitoring locations

### How it works

1. Subscribe to this server
2. Enter your free OpenAQ API Key
3. Start monitoring air quality from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_countries**: Includes location counts and city counts per country.

List countries with monitoring stations
- **get_latest_measurements**: Useful for getting current air quality status without querying full history.

Get latest measurements per location
- **get_location_by_id**: Get details for a specific location
- **get_locations**: Filter by country, city, parameter, or geographic bounding box. Returns location details including coordinates, sensor counts, and whether the station is an official monitor.

List air quality monitoring locations
- **get_measurements**: Filter by location, parameter, date range, and value range. Returns readings with timestamps.

Get historical air quality measurements
- **get_parameter_by_id**: Get details for a specific parameter
- **get_parameters**: 5, PM10, O3 (ozone), NO2, SO2, CO, etc. Includes units and whether each is a core parameter.

List measurable air quality parameters
- **get_sensor_by_id**: Get details for a specific sensor
- **get_sensors**: Filter by location, parameter type, or active status.

List air quality sensors


## Installation & Usage

To install and use the **OpenAQ** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openaq](https://vinkius.com/mcp/openaq)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
