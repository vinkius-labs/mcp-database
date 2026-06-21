# OpenWeather Agro MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openweather-agro)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/openweather-agro-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/openweather-agro-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access agricultural weather and satellite data via OpenWeather — monitor NDVI, soil temperature, evapotranspiration, frost risk, and GDD from any AI agent.

## Description
Connect your **OpenWeather Agro API** to any AI agent and take full control of satellite-based vegetation monitoring, weather-driven agricultural insights, and precision farming data through natural conversation.

### What you can do

- **NDVI Analysis** — Monitor crop vegetation health with satellite-derived NDVI values
- **EVI Monitoring** — Track enhanced vegetation index for high-biomass and dense canopy areas
- **Soil Temperature** — Check soil thermal conditions for seed germination and root activity
- **Evapotranspiration** — Calculate crop water use for precision irrigation scheduling
- **Current Weather** — Get real-time weather conditions for daily farming decisions
- **Weather Forecast** — Access 5-day forecasts for planting and harvest planning
- **Historical Weather** — Retrieve past weather data for crop performance analysis
- **Growing Degree Days** — Track heat accumulation for crop development staging
- **Satellite Imagery** — Access satellite imagery for visual field assessment
- **Historical NDVI** — Analyze vegetation health trends over growing seasons
- **Crop Health Index** — Get comprehensive crop condition scores
- **Frost Risk** — Assess frost danger for crop protection planning

### How it works

1. Subscribe to this server
2. Enter your OpenWeather API key (appid from your dashboard)
3. Start analyzing agricultural conditions from Claude, Cursor, or any MCP-compatible client

No more manual weather checking or complex satellite data processing. Your AI acts as a dedicated agricultural meteorologist and crop health analyst.

### Who is this for?

- **Farmers** — monitor crop health, plan irrigation, and assess frost risk with satellite and weather data
- **Agronomists** — analyze NDVI trends, track GDD accumulation, and advise on crop management
- **Agricultural Consultants** — provide data-driven recommendations based on satellite imagery and weather patterns
- **Researchers** — access historical vegetation indices and weather data for agricultural studies


## Available Tools
- **get_crop_health_index**: CHI provides a single metric for overall crop health, making it easier to track field conditions over time and compare across fields. Essential for quick field health assessment, prioritizing scouting missions, and communicating crop status to stakeholders. AI agents should use this when users ask "what is the overall crop health score for my field", "get a quick health assessment", or need a simplified crop condition metric. Date format: YYYY-MM-DD.

Get Crop Health Index (CHI) for comprehensive crop condition assessment
- **get_current_weather**: Essential for daily farming decisions, spray application timing, harvest planning, and frost protection. AI agents should use this when users ask "what is the weather like at my farm right now", "should I spray pesticides today", or need current weather data for agricultural operations.

Get current weather conditions for agricultural decision making
- **get_evi**: EVI is more sensitive than NDVI in high-biomass regions and less affected by atmospheric conditions and soil background. Essential for monitoring dense canopies, tropical crops, and areas with high vegetation cover. AI agents should reference this when users ask "what is the EVI for my dense crop area", "monitor high-biomass vegetation", or need enhanced vegetation index for areas where NDVI saturates. Date format: YYYY-MM-DD.

Get EVI (Enhanced Vegetation Index) for high-biomass crop monitoring
- **get_soil_temperature**: Soil temperature is critical for seed germination timing, root activity assessment, and nutrient uptake optimization. Essential for planting decisions, irrigation scheduling, and soil health monitoring. AI agents should use this when users ask "what is the soil temperature for planting", "check if soil is warm enough for germination", or need soil thermal data for agricultural planning. Date format: YYYY-MM-DD.

Get satellite-derived soil temperature for seed germination and root activity assessment
- **get_weather_forecast**: Essential for planting schedules, harvest timing, spray application windows, and irrigation planning. AI agents should reference this when users ask "what is the weather forecast for my farm this week", "will it rain in the next 5 days", or need forward-looking weather data for agricultural planning.

Get multi-day weather forecast for agricultural planning
- **get_evapotranspiration**: ET combines soil evaporation and plant transpiration, providing the most accurate measure of crop water use. Essential for precision irrigation scheduling, water resource management, and drought assessment. AI agents should reference this when users ask "what is the evapotranspiration rate for my field", "calculate irrigation needs", or need crop water use data for irrigation planning. Date format: YYYY-MM-DD.

Get evapotranspiration rates for irrigation scheduling and water management
- **get_frost_risk**: Returns risk levels (low, moderate, high, critical), predicted frost timing, and recommended protection measures. Essential for frost-sensitive crops (fruits, vegetables, vineyards), irrigation-based frost protection, and crop insurance documentation. AI agents should reference this when users ask "is there frost risk for my orchard tonight", "assess frost danger for my crops", or need frost warning data for crop protection planning.

Get frost risk assessment for crop protection planning
- **get_growing_degree_days**: GDD measures heat accumulation used to predict crop development stages, pest emergence, and harvest timing. Essential for phenology tracking, variety selection, and timing agricultural operations. AI agents should reference this when users ask "calculate GDD for my corn field this season", "track crop development stages", or need heat unit accumulation data for agricultural planning. Date format: YYYY-MM-DD.

Calculate Growing Degree Days (GDD) for crop development tracking
- **get_historical_ndvi**: Returns time-series NDVI values showing vegetation health progression, stress detection, and recovery patterns. Essential for seasonal crop performance comparison, drought impact assessment, and long-term field health monitoring. AI agents should reference this when users ask "show me NDVI trends for my field over the growing season", "compare vegetation health between seasons", or need historical vegetation index data for agricultural trend analysis. Date format: YYYY-MM-DD.

Get historical NDVI trends for seasonal vegetation health analysis
- **get_ndvi**: NDVI ranges from -1 to 1, with higher values (0.6-0.9) indicating healthy dense vegetation and lower values (0.2-0.5) indicating stressed or sparse vegetation. Essential for crop health monitoring, growth stage assessment, and yield prediction. AI agents should use this when users ask "what is the NDVI for my field on this date", "check crop vegetation health", or need satellite-based vegetation index data for agricultural analysis. Date format: YYYY-MM-DD.

Get NDVI (Normalized Difference Vegetation Index) for crop health assessment
- **get_satellite_imagery**: Returns imagery metadata and access URLs for visual crop assessment, field boundary verification, and change detection analysis. Essential for remote field monitoring, damage assessment, and visual crop health evaluation. AI agents should use this when users ask "get satellite imagery for my field", "show me the latest satellite view of my farm", or need visual imagery for agricultural monitoring. Date format: YYYY-MM-DD. Zoom: 1-16.

Get satellite imagery for visual crop assessment and field monitoring
- **get_weather_history**: Essential for comparing current conditions with historical patterns, analyzing crop performance under past weather conditions, and validating crop models. AI agents should use this when users ask "what was the weather like on this date last year", "show me historical weather for my field", or need past weather data for agricultural analysis. Date format: Unix timestamp (seconds since 1970).

Get historical weather data for crop analysis and trend assessment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenWeather Agro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the NDVI for my corn field at coordinates 41.8780, -93.0977 on April 1st?"

**🤖 AI Agent:**
> Fetching NDVI data for Iowa corn field (41.8780, -93.0977) on 2026-04-01... NDVI value: 0.28 (low vegetation cover, expected for early season). This indicates bare soil or very early emergence stage. Historical comparison: Same date last year was 0.25, so emergence is slightly ahead. Recommendation: Continue monitoring weekly as canopy develops. Target NDVI for mid-season corn is 0.75-0.85. Would you like historical NDVI trends to compare this season's progress?

---

**👤 You:**
> "Calculate the growing degree days for my wheat field from March 1 to today."

**🤖 AI Agent:**
> Calculating Growing Degree Days (GDD) for wheat field (base 0C)... Period: March 1 to April 7, 2026. Total accumulated GDD: 285. Wheat development stage: Tillering to early stem extension. Average daily GDD: 7.5. Comparison to normal: 12% above average for this period. At this rate, heading stage expected around May 15. Recommendation: Apply nitrogen top-dressing now to support stem development. Monitor for early pest emergence due to warmer than normal accumulation.

---

**👤 You:**
> "Is there frost risk for my vineyard tonight? I need to know if I should turn on the wind machines."

**🤖 AI Agent:**
> Checking frost risk for your vineyard location... FROST RISK: HIGH tonight. Predicted low temperature: -1.8°C (28.8°F) around 5:00 AM. Soil temperature: 4.2°C. Wind speed: 2 km/h (calm conditions increase frost risk). Dew point: -3.1°C. Recommendation: Activate frost protection measures immediately. Wind machines should be turned on by 3:00 AM (before temperature drops below critical threshold). If available, supplement with irrigation for additional 1-2°C protection. Monitor conditions hourly through dawn.


## Installation & Usage

To install and use the **OpenWeather Agro** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openweather-agro](https://vinkius.com/mcp/openweather-agro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
