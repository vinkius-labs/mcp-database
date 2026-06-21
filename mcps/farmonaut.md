# Farmonaut MCP Server

Access satellite agriculture data via Farmonaut — monitor crop health with NDVI, weather, soil moisture, crop advisory, and deforestation alerts from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/farmonaut)

## Overview
**Category:** the-unthinkable
**Tools Count:** 12

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


## Available Tools
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


## Installation & Usage

To install and use the **Farmonaut** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/farmonaut](https://vinkius.com/mcp/farmonaut)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
