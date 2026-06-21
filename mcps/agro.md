# Agro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Monitor agricultural land using satellite imagery, weather data, and soil metrics directly from your AI agent.

## Description
Connect the **AgroMonitoring API** to your AI agent to transform how you manage precision agriculture. Access high-resolution satellite data, historical crop health indices, and hyper-local weather conditions through simple commands.

### What you can do

- **Polygon Management** — Create, list, and update areas of interest (polygons) representing your fields or farms.
- **Satellite Insights** — Search for available satellite imagery and retrieve NDVI (Normalized Difference Vegetation Index) and EVI history to track crop health over time.
- **Weather Intelligence** — Get current, forecast, and historical weather data, including accumulated temperature and precipitation metrics.
- **Soil & UV Monitoring** — Access real-time and historical soil moisture and temperature data, along with UV index tracking for optimal field management.

### How it works

1. Subscribe to this server
2. Enter your AgroMonitoring API Key
3. Start querying field data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Agronomists & Farmers** — Monitor crop health and soil conditions across multiple fields without manual data entry.
- **Data Scientists** — Quickly pull historical weather and satellite indices for agricultural modeling.
- **AgTech Developers** — Integrate field-level environmental data into your development workflow via natural language.


## Available Tools
- **delete_polygon**: Delete a polygon
- **get_current_weather**: Get current weather data
- **get_current_uvi**: Get current UV Index
- **create_polygon**: Create a new polygon for an area of interest
- **get_accumulated_precipitation**: Get accumulated precipitation
- **get_accumulated_temperature**: Get accumulated temperature
- **get_forecast_uvi**: Get forecast UV Index
- **get_forecast_weather**: Get forecast weather data
- **get_historical_soil**: Get historical soil data
- **get_historical_uvi**: Get historical UV Index
- **get_current_soil**: Get current soil data
- **get_historical_weather**: Get historical weather data
- **get_ndvi_history**: Get NDVI and EVI historical data
- **get_polygon**: Get info for one polygon
- **list_polygons**: Get list of polygons
- **search_imagery**: Search for satellite imagery
- **update_polygon**: Update polygon info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my registered agricultural polygons."

**🤖 AI Agent:**
> I've retrieved your polygons. You have 3 registered areas: 'North Corn Field' (ID: 64b1...), 'South Vineyard' (ID: 64b2...), and 'Experimental Plot' (ID: 64b3...).

---

**👤 You:**
> "Get the NDVI history for polygon 64b123456789 for the last 30 days."

**🤖 AI Agent:**
> Fetching NDVI data... For the last 30 days, the average NDVI for 'North Corn Field' started at 0.65 and increased to 0.78, indicating healthy growth. There are 4 data points available from Sentinel-2.

---

**👤 You:**
> "What is the current soil moisture and temperature at coordinates 45.5, -73.6?"

**🤖 AI Agent:**
> Checking soil conditions... At those coordinates, the current soil moisture is 0.28 m3/m3 and the surface temperature is 22.4°C (72.3°F).


## ❓ FAQ

**Q: How do I define a new field for monitoring?**
Use the `create_polygon` tool. You need to provide a name and the area's geometry in GeoJSON format (coordinates). This polygon ID will then be used for satellite and soil queries.

**Q: Can I check the historical health of my crops?**
Yes! Use the `get_ndvi_history` tool with your Polygon ID and a time range. It returns NDVI and EVI data, which are key indicators of vegetation vigor and growth.

**Q: What kind of soil data can I retrieve?**
You can use `get_current_soil` or `get_historical_soil` to get moisture levels and surface temperature for a specific polygon, helping you optimize irrigation schedules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agro](https://vinkius.com/mcp/agro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agro** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `agro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agro": {
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
