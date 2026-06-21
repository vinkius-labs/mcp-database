# Farmonaut MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/farmonaut)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access satellite agriculture data via Farmonaut — monitor crop health with NDVI, weather, soil moisture, crop advisory, and deforestation alerts from any AI agent.

## Description
Connect your **Farmonaut Satellite API** to any AI agent and take full control of satellite-based crop monitoring, vegetation index analysis, weather tracking, AI crop advisory, and deforestation detection through natural conversation.

### What you can do

- **Field Management** — List and register agricultural fields with boundaries, crop types, and planting dates
- **NDVI Analysis** — Calculate NDVI from Sentinel-2, Landsat, and PlanetScope for crop health monitoring
- **NDWI Water Index** — Monitor crop water content and irrigation needs with water index analysis
- **EVI Enhanced Index** — Track enhanced vegetation index for high-biomass and dense canopy crops
- **Weather Data** — Access historical and current weather data for agricultural decision making
- **Weather Forecast** — Get forecasts from 7 days to 3 months for agricultural planning
- **Soil Moisture** — Monitor soil moisture at different depths for irrigation scheduling
- **Satellite Imagery** — Retrieve true-color, false-color, and NDVI overlay images from multiple satellites
- **AI Crop Advisory** — Get AI-powered recommendations for irrigation, fertilizer, pest control, and harvest
- **Deforestation Alerts** — Detect land use changes and tree cover loss for conservation compliance
- **SAR Analysis** — All-weather monitoring using Synthetic Aperture Radar that penetrates clouds
- **Multi-Satellite Support** — Access Sentinel-2, Landsat, PlanetScope, and SAR satellite data

### How it works

1. Subscribe to this server
2. Enter your Farmonaut API key (from the dashboard API section)
3. Start monitoring crops from Claude, Cursor, or any MCP-compatible client

No more manual satellite data analysis or complex GIS workflows. Your AI acts as a dedicated precision agriculture analyst and farm management assistant.

### Who is this for?

- **Farm Managers** — monitor crop health across all fields, plan irrigation, and optimize inputs
- **Agronomists** — analyze vegetation indices, track growth stages, and detect crop stress early
- **Agricultural Consultants** — provide AI-powered advisories and assess field productivity
- **Conservation Teams** — monitor deforestation, land use changes, and environmental compliance


## Available Tools (12)
- **get_soil_moisture**: Returns soil moisture levels at different depths (surface, root zone, deep soil), moisture anomalies, and irrigation recommendations. Essential for irrigation scheduling, drought monitoring, water stress detection, and water resource optimization. AI agents should use this when users ask "what is the soil moisture level in my field", "do I need to irrigate", or need soil moisture data for irrigation planning.

Get soil moisture data for irrigation scheduling and drought monitoring
- **get_weather_forecast**: Includes temperature, precipitation, humidity, wind, and solar radiation forecasts. Essential for planting schedule optimization, harvest timing, irrigation planning, frost protection, and seasonal crop management. AI agents should reference this when users ask "what is the weather forecast for my field next week", "get seasonal precipitation forecast", or need forward-looking weather data for agricultural planning.

Get weather forecasts for agricultural planning and irrigation scheduling
- **get_weather**: Includes temperature (air, soil), precipitation, humidity, wind speed/direction, solar radiation, evapotranspiration, and growing degree days. Essential for irrigation planning, frost risk assessment, disease/pest pressure modeling, and yield prediction. AI agents should use this when users ask "what was the weather like on my field last month", "get temperature and rainfall data", or need historical weather analysis for crop management decisions.

Get historical and current weather data for agricultural fields
- **add_field**: Accepts field boundary as GeoJSON polygon or coordinates, field name, crop type, and planting date. Returns the created field with ID, calculated area, and monitoring activation status. Essential for onboarding new fields into the monitoring system, expanding farm coverage, and setting up new crop seasons. AI agents should use this when users ask "add a new field for monitoring", "register this field boundary", or need to set up satellite monitoring for a new agricultural area.

Register a new agricultural field for satellite monitoring
- **get_crop_advisory**: Returns recommendations for irrigation, fertilization, pest control, harvest timing, and field operations. Essential for data-driven farm management, precision agriculture, and optimizing crop inputs. AI agents should use this when users ask "what should I do in my field this week", "get irrigation and fertilizer recommendations", or need AI-powered crop management advice.

Get AI-powered crop management advisories and recommendations
- **get_deforestation_alerts**: Uses satellite imagery to detect tree cover loss, land clearing, and vegetation changes over time. Essential for conservation compliance, environmental monitoring, carbon credit verification, and land use change detection. AI agents should reference this when users ask "show deforestation alerts in my area", "detect land use changes", or need environmental compliance monitoring.

Get deforestation and land change detection alerts
- **get_evi**: EVI is more sensitive in high-biomass regions and less affected by atmospheric conditions and soil background than NDVI. Essential for monitoring dense canopies, tropical crops, and areas with high atmospheric interference. Returns EVI values, statistics, satellite source, and acquisition dates. AI agents should use this when users ask "show me EVI trends for this field", "how is the canopy developing in high-biomass areas", or need enhanced vegetation index analysis for dense vegetation.

Calculate EVI enhanced vegetation index for high-biomass crop monitoring
- **get_fields**: Returns field names, boundaries (GeoJSON polygons), area in hectares/acres, crop type, planting dates, and current monitoring status. Essential for farm management overview, field inventory, and selecting target fields for satellite analysis. AI agents should use this when users ask "show me all my fields", "list monitored fields", or need to identify available fields for vegetation index or weather queries.

List all agricultural fields monitored in your Farmonaut account
- **get_ndvi**: NDVI measures vegetation health and vigor on a scale of -1 to 1, with higher values indicating healthier vegetation. Returns NDVI values, statistics (mean, min, max, std), satellite source, acquisition date, and cloud cover percentage. Essential for crop health assessment, growth stage monitoring, stress detection, and yield prediction. AI agents should use this when users ask "what is the NDVI for my rice field this month", "calculate vegetation health for field X", or need NDVI-based crop health analysis.

Calculate NDVI vegetation index for crop health monitoring
- **get_ndwi**: NDWI is sensitive to vegetation water content and soil moisture, making it essential for irrigation scheduling, drought monitoring, and water stress detection. Returns NDWI values, statistics, satellite source, and acquisition dates. AI agents should reference this when users ask "what is the water content in my crops", "do I need to irrigate", or need water stress analysis for irrigation planning.

Calculate NDWI water index for crop water stress and irrigation monitoring
- **get_sar_analysis**: SAR penetrates clouds and works day/night, making it essential for monitoring in cloudy or rainy conditions. Returns backscatter values, soil moisture estimates, crop structure information, and change detection analysis. Essential for all-weather monitoring, flood detection, soil moisture mapping, and crop structure analysis. AI agents should use this when users ask "get SAR analysis for my field during cloudy season", "monitor crops through cloud cover", or need all-weather satellite analysis.

Get Synthetic Aperture Radar (SAR) analysis for all-weather crop monitoring
- **get_satellite_images**: Returns true-color and false-color composites, NDVI overlays, and raw spectral bands. Essential for visual crop assessment, change detection, damage assessment, and downloading imagery for further processing. AI agents should reference this when users ask "show me satellite images of my field from last week", "get latest Sentinel-2 imagery", or need satellite imagery for visual assessment.

Retrieve satellite imagery for agricultural fields from multiple sources


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Farmonaut** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the NDVI trend for my rice field over the last 3 months."

**🤖 AI Agent:**
> Fetching NDVI data for rice field (field ID: R-2045)... Found 18 satellite observations from Sentinel-2 over the past 3 months. NDVI progression: Month 1 (0.32) — early vegetative stage, Month 2 (0.58) — active tillering, Month 3 (0.74) — peak vegetative vigor. Current average NDVI is 0.74 indicating healthy crop development. The highest NDVI of 0.79 was recorded on the latest clear-sky pass. Would you like crop advisory recommendations based on this trend?

---

**👤 You:**
> "What is the 7-day weather forecast and current soil moisture for my wheat field?"

**🤖 AI Agent:**
> Fetching 7-day forecast and soil moisture for wheat field (field ID: W-1823)... Weather forecast: Next 2 days sunny 26-30°C no rain. Days 3-5: 70% chance of 20mm rainfall. Days 6-7: partly cloudy 24-28°C. Current soil moisture (root zone): 38% — adequate for current growth stage. With 20mm rain expected in 3-5 days irrigation can be delayed. AI advisory: Hold irrigation for now, reassess after rainfall event.

---

**👤 You:**
> "Get AI crop advisory recommendations for my cotton field this week."

**🤖 AI Agent:**
> Generating AI advisory for cotton field (field ID: C-3156)... Current growth stage: Boll development. Recommendations: 1) IRRIGATION: Apply 25mm this week — soil moisture at 42% with no significant rain forecast. 2) FERTILIZER: Top-dress with potassium (K2O 40kg/ha) to support boll filling. 3) PEST CONTROL: Monitor for bollworm — NDVI shows uniform canopy but scout field edges. 4) HARVEST: Expected harvest window in 4-6 weeks based on current development rate. Priority: Irrigation within 3 days.


## ❓ FAQ

**Q: Can my AI calculate NDVI for my rice field and show me the crop health trend?**
Yes! Use the `get_ndvi` tool with your field ID and date range (e.g., date_from=2025-04-01, date_to=2025-10-31). This returns NDVI values for each satellite overpass from Sentinel-2, Landsat, or PlanetScope, showing vegetation health progression. You can also use `get_crop_advisory` for AI-powered recommendations based on the NDVI trends and current growth stage.

**Q: How do I get soil moisture and weather forecast data to plan irrigation?**
Use `get_soil_moisture` with your field ID and date range to check current soil moisture levels at root zone depth. Combine with `get_weather_forecast` (forecast_range=7_days or 15_days) to see upcoming precipitation. Together these tools help determine if and when irrigation is needed. For AI-powered irrigation recommendations, use `get_crop_advisory` with advisory_type=irrigation.

**Q: Can I monitor my crops during cloudy season when optical satellites cannot see?**
Yes! Use the `get_sar_analysis` tool which uses Synthetic Aperture Radar (SAR) data that penetrates clouds and works day/night. SAR provides backscatter values, soil moisture estimates, and crop structure information regardless of weather conditions. This is essential for monitoring in tropical regions, monsoon seasons, or any cloudy conditions where optical satellites like Sentinel-2 cannot provide clear imagery.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/farmonaut](https://vinkius.com/mcp/farmonaut)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Farmonaut** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `farmonaut` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Farmonaut** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "farmonaut": {
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
