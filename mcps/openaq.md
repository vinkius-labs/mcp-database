# OpenAQ MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openaq)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access global air quality data — monitor PM2.5, O3, NO2 levels and track pollution via AI.

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


## Available Tools (9)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenAQ** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the current PM2.5 level in São Paulo, Brazil?"

**🤖 AI Agent:**
> Latest PM2.5 reading for São Paulo: 18.5 µg/m³ (moderate). This is above the WHO guideline of 5 µg/m³ annual mean. Would you like to see the 24-hour trend?

---

**👤 You:**
> "Which countries have the most air quality monitoring stations?"

**🤖 AI Agent:**
> Top countries by monitoring stations: India (2,100+ locations), United States (1,800+), China (1,500+), Brazil (900+), and Germany (700+). Would you like details for any specific country?

---

**👤 You:**
> "Show me ozone (O3) measurements from the last 24 hours in Paris."

**🤖 AI Agent:**
> Retrieved 48 O3 readings from Paris monitoring stations in the last 24 hours. Average: 65 µg/m³, Peak: 92 µg/m³ at 14:00. All readings within acceptable range. Highest reading was at the Paris 18ème station.


## ❓ FAQ

**Q: How do I get an OpenAQ API Key?**
Visit [**OpenAQ Platform**](https://platform.openaq.org/), create a free account, and generate your API key from the dashboard. Free tier includes 1,000 requests/hour.

**Q: What air quality parameters can I monitor?**
PM2.5, PM10, O3 (ozone), NO2, SO2, CO, BC (black carbon), and more. Use `get_parameters` to see the full list with units and classifications.

**Q: Can I get historical air quality data?**
Yes! Use `get_measurements` with date_from and date_to parameters in ISO 8601 format to retrieve time-series data for any location and parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openaq](https://vinkius.com/mcp/openaq)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenAQ** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `openaq` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenAQ** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openaq": {
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
