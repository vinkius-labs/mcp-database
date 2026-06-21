# AirVisual MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/airvisual)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/airvisual-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/airvisual-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Monitor global air quality and weather data via AirVisual — access real-time AQI, pollution levels, and meteorological data from any AI agent.

## Description
Connect your **AirVisual** (IQAir) account to any AI agent to monitor environmental health and weather conditions worldwide through natural conversation.

### What you can do

- **Real-time AQI & Weather** — Get current air quality index (AQI) and meteorological data for specific cities or monitoring stations.
- **Location Discovery** — Browse supported countries, states, and cities to find precise monitoring locations.
- **Proximity Search** — Automatically find the nearest air quality data based on your IP address or specific GPS coordinates.
- **Station-Level Detail** — Access granular data from individual monitoring stations for hyper-local environmental insights.

### How it works

1. Subscribe to this server
2. Enter your AirVisual API Key
3. Start monitoring air quality from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Health-Conscious Users** — track pollution levels and allergens in your area to plan outdoor activities.
- **Environmental Researchers** — gather real-time data from thousands of global stations for analysis.
- **Smart Home Enthusiasts** — integrate air quality triggers into your automated workflows.


## Available Tools
- **list_cities**: List all supported cities in a specific state
- **get_city_data**: Get real-time AQI and weather for a specific city
- **list_countries**: List all supported countries
- **get_nearest_city_by_coords**: Get data for the nearest city based on GPS coordinates
- **get_nearest_city_by_ip**: Get data for the nearest city based on IP address
- **list_states**: List all supported states in a specific country
- **get_station_data**: Get data from a specific monitoring station


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AirVisual** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current air quality and weather in Tokyo, Japan?"

**🤖 AI Agent:**
> I've retrieved the data for Tokyo. The current AQI is 42 (Good), with the main pollutant being PM2.5. The weather is clear with a temperature of 18°C and 55% humidity.

---

**👤 You:**
> "Check the air quality at the nearest city based on my IP."

**🤖 AI Agent:**
> Based on your IP, the nearest city is San Francisco. The current AQI is 15 (Excellent). It's currently 14°C with moderate winds.

---

**👤 You:**
> "List all supported states in Canada."

**🤖 AI Agent:**
> I've found 13 supported states/provinces in Canada, including Ontario, British Columbia, Quebec, and Alberta. Which one would you like to explore for city data?


## Installation & Usage

To install and use the **AirVisual** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airvisual](https://vinkius.com/mcp/airvisual)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
