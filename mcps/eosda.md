# EOSDA MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eosda)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access satellite agriculture data via EOSDA — monitor crop health, vegetation indices, weather, soil moisture, and generate zoning maps from any AI agent.

## Description
Connect your **EOSDA Agriculture API** to any AI agent and take full control of satellite-based crop monitoring, vegetation index analysis, weather tracking, and precision agriculture through natural conversation.

### What you can do

- **Field Management** — List and register agricultural fields with boundaries, crop types, and planting dates
- **Vegetation Indices** — Calculate 17+ indices (NDVI, EVI, NDRE, MSAVI, NDMI, etc.) from Sentinel-2 and Landsat
- **NDVI Time Series** — Track vegetation health trends across entire growing seasons
- **EVI Time Series** — Monitor enhanced vegetation index for high-biomass and tropical crops
- **NDMI Time Series** — Monitor crop water content and irrigation needs
- **Satellite Imagery** — Retrieve raw satellite imagery bands from multiple satellite sources
- **Weather Data** — Access 20+ years of historical weather data with 1800+ parameters
- **Weather Forecast** — Get forecasts from 15 days to 7 months for agricultural planning
- **Soil Moisture** — Monitor soil moisture levels at different depths for irrigation scheduling
- **Zoning Maps** — Generate productivity and vegetation health zoning maps for precision agriculture
- **Index Map Rendering** — Create visual vegetation index maps with customizable colormaps
- **Custom Field Registration** — Add new fields with GeoJSON boundaries for satellite monitoring

### How it works

1. Subscribe to this server
2. Enter your EOSDA API key (from the My account > API section)
3. Start monitoring crops from Claude, Cursor, or any MCP-compatible client

No more manual satellite data analysis or complex GIS workflows. Your AI acts as a dedicated precision agriculture analyst.

### Who is this for?

- **Farm Managers** — monitor crop health, plan irrigation, and optimize inputs across all fields
- **Agronomists** — analyze vegetation indices, track growth stages, and detect crop stress early
- **Agricultural Consultants** — generate zoning maps, assess field productivity, and advise on precision agriculture
- **AgriTech Companies** — integrate satellite-based crop data into farm management platforms


## Available Tools
- **get_ndmi_timeseries**: NDMI is sensitive to vegetation water content and is used for drought monitoring, irrigation scheduling, and fire risk assessment. Returns NDMI values per satellite overpass date. Essential for water stress detection, irrigation optimization, drought impact assessment, and harvest timing. AI agents should use this when users ask "show me crop water stress trends", "how is the moisture content changing", or need moisture index analysis for irrigation planning.

Get NDMI time series data for crop water stress monitoring
- **create_field**: Accepts field boundary as GeoJSON polygon or coordinates, field name, crop type, and planting date. Returns the created field with ID, calculated area, and monitoring activation status. Essential for onboarding new fields into the monitoring system, expanding farm coverage, and setting up new crop seasons. AI agents should use this when users ask "add a new field for monitoring", "register this field boundary", or need to set up satellite monitoring for a new agricultural area.

Register a new agricultural field for satellite monitoring
- **get_evi_timeseries**: EVI is more sensitive in high-biomass regions and less affected by atmospheric conditions than NDVI. Returns EVI values per satellite overpass date for trend analysis. Essential for monitoring dense canopies, tropical crops, and areas with high atmospheric interference. AI agents should reference this when users ask "show me EVI trends for this field", "how is the canopy developing", or need enhanced vegetation index analysis for high-biomass crops.

Get EVI time series data for enhanced vegetation monitoring over a growing season
- **get_fields**: Returns field names, boundaries (GeoJSON polygons), area in hectares/acres, crop type, planting dates, and current growth stage information. Essential for farm management overview, field inventory, and selecting target fields for satellite analysis. AI agents should use this when users ask "show me all my fields", "list monitored fields", or need to identify available fields for vegetation index or weather queries.

List all agricultural fields monitored in your EOSDA account
- **get_ndvi_timeseries**: Returns NDVI values per satellite overpass date, enabling trend analysis of crop health, growth stages, and stress detection. Essential for season-long crop monitoring, growth curve analysis, yield prediction, and identifying problematic periods. AI agents should use this when users ask "show me the NDVI trend for this season", "how has vegetation health changed over the growing season", or need time-series vegetation analysis.

Get NDVI time series data showing vegetation health trends over a growing season
- **render_index_map**: Returns rendered raster images (JPEG, PNG, or GeoTIFF) with color-coded vegetation index values overlaid on field boundaries. Supports colormaps like NDVI (green-yellow-red), thermal, grayscale, and custom color schemes. Essential for field reports, stakeholder communication, visual crop assessment, and creating shareable vegetation maps. AI agents should reference this when users ask "create a color-coded NDVI map of my field", "generate a vegetation health visualization", or need shareable vegetation index images for reports.

Generate visual vegetation index maps with customizable colormaps for field visualization
- **get_satellite_imagery**: ) for a specific field and date range. Supports Sentinel-2, Landsat 8/9, MODIS, NAIP, and CBERS-4 sources. Returns image metadata, acquisition dates, cloud cover percentages, band availability, and download URLs. Essential for visual crop assessment, custom band analysis, change detection, and downloading raw imagery for further processing. AI agents should reference this when users ask "show me satellite images of my field from last week", "get Sentinel-2 imagery for field X", or need raw satellite imagery download links.

Retrieve raw satellite imagery for a specific field and date range
- **get_soil_moisture**: Returns soil moisture levels at different depths (surface, root zone, deep soil), moisture anomalies, and irrigation recommendations. Essential for irrigation scheduling, drought monitoring, water stress detection, and water resource optimization. AI agents should reference this when users ask "what is the soil moisture level in my field", "do I need to irrigate", or need soil moisture data for irrigation planning.

Get soil moisture data for agricultural fields
- **get_vegetation_index**: Supports 17+ indices including NDVI (vegetation health), EVI (enhanced vegetation index), GNDVI (green NDVI), NDRE (red edge), MSAVI (soil adjusted), RECI (red edge chlorophyll), NDSI, NDWI (water), SAVI, ARVI, GCI (chlorophyll), SIPI, NBR (burn ratio), MSI (moisture), ISTACK, FIDET, and CCCI. Returns index values, statistics (mean, min, max, std), satellite source (Sentinel-2, Landsat), and cloud cover percentage. Essential for crop health assessment, stress detection, and growth monitoring. AI agents should use this when users ask "what is the NDVI for my corn field this month", "calculate vegetation health for field X", or need vegetation index analysis.

Calculate vegetation indices (NDVI, EVI, NDRE, etc.) for a specific field and date range
- **get_weather_data**: Includes 1800+ weather parameters: temperature (air, soil), precipitation, humidity, wind speed/direction, solar radiation, evapotranspiration, dew point, pressure, and growing degree days. Historical data available since 1979. Essential for irrigation planning, frost risk assessment, disease/pest pressure modeling, and yield prediction. AI agents should use this when users ask "what was the weather like on my field last month", "get temperature and rainfall data", or need historical weather analysis for crop management decisions.

Get historical and current weather data for agricultural fields
- **get_weather_forecast**: Includes temperature, precipitation, humidity, wind, and solar radiation forecasts. Essential for planting schedule optimization, harvest timing, irrigation planning, frost protection, and seasonal crop management. AI agents should reference this when users ask "what is the weather forecast for my field next week", "get seasonal precipitation forecast", or need forward-looking weather data for agricultural planning.

Get weather forecasts (15 days to 7 months) for agricultural fields
- **get_zoning_map**: Returns zone boundaries, average index values per zone, area percentages, and management recommendations. Essential for variable rate application (VRA), precision fertilization, targeted irrigation, and yield optimization. AI agents should use this when users ask "create a zoning map for my field", "generate productivity zones", or need management zone maps for precision agriculture.

Generate productivity and vegetation health zoning maps for fields


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EOSDA** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the NDVI trend for my corn field over the 2025 growing season."

**🤖 AI Agent:**
> Fetching NDVI time series for corn field (field ID: 12345)... Found 28 satellite observations from April to October 2025. NDVI progression: April (0.25) — early growth, May (0.42) — vegetative development, June (0.61) — canopy closure, July (0.78) — peak vegetation, August (0.74) — grain fill, September (0.58) — senescence begins, October (0.35) — harvest ready. Peak NDVI of 0.78 was reached on July 15. Would you like a visual NDVI map or comparison with last season?

---

**👤 You:**
> "What is the 15-day weather forecast and current soil moisture for my soybean field?"

**🤖 AI Agent:**
> Fetching 15-day forecast and soil moisture for soybean field (field ID: 67890)... Weather forecast: Next 3 days sunny, 28-32°C, no rain. Days 4-7: 60% chance of 15mm rainfall. Days 8-15: variable clouds, 25-30°C, 5-10mm scattered showers. Current soil moisture (root zone): 42% — adequate for current growth stage. With 15mm rain expected in 4-7 days, irrigation can be delayed. Next recommended irrigation check: 10 days from now.

---

**👤 You:**
> "Generate a productivity zoning map for my wheat field with 4 zones."

**🤖 AI Agent:**
> Generating zoning map for wheat field (field ID: 11223)... Using NDVI from 2025-06-15 with 4 management zones. Zone 1 (Very High): 22% of field, avg NDVI 0.82 — excellent productivity. Zone 2 (High): 31% of field, avg NDVI 0.71 — good productivity. Zone 3 (Medium): 28% of field, avg NDVI 0.58 — moderate productivity. Zone 4 (Low): 19% of field, avg NDVI 0.41 — below average, may need soil amendment. Zoning map rendered and ready for variable rate application planning. Download: https://api.eos.com/zoning/wheat_field_zoning_map.png


## ❓ FAQ

**Q: Can my AI calculate NDVI for my corn field and show me the vegetation health trend over the growing season?**
Yes! Use the `get_ndvi_timeseries` tool with your field ID and the growing season date range (e.g., date_from=2025-04-01, date_to=2025-10-31). This returns NDVI values for each satellite overpass, showing vegetation health progression from planting through harvest. You can also use `get_vegetation_index` with index=NDVI for point-in-time analysis, or `render_index_map` to generate a visual color-coded NDVI map of your field.

**Q: How do I get weather forecasts and soil moisture data to plan irrigation for my fields?**
Use `get_weather_forecast` with your field ID and forecast_range=15_days or 1_month to get upcoming precipitation and temperature forecasts. Combine this with `get_soil_moisture` to check current soil moisture levels at root zone depth. Together these tools help you determine if and when irrigation is needed. For historical context, use `get_weather_data` with past dates to understand rainfall patterns and evapotranspiration trends.

**Q: Can I generate a zoning map to identify low and high productivity areas within my field?**
Yes! Use the `get_zoning_map` tool with your field ID. You can specify the vegetation index (NDVI is most common), number of zones (3-5 recommended), and date for analysis. The API returns zone boundaries, average index values per zone, area percentages, and management recommendations. This is essential for variable rate application (VRA), precision fertilization, and targeted irrigation planning.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eosda](https://vinkius.com/mcp/eosda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EOSDA** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `eosda` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EOSDA** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eosda": {
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
