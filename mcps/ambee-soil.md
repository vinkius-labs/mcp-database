# Ambee Soil MCP Server

Access real-time soil data via Ambee — monitor soil moisture, temperature, and properties globally for precision agriculture from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ambee-soil)

## Overview
**Category:** the-unthinkable
**Tools Count:** 5

## Description
Connect your **Ambee Soil API** to any AI agent and take full control of real-time soil moisture tracking, temperature monitoring, historical trend analysis, and soil property assessment through natural conversation.

### What you can do

- **Real-Time Soil Data** — Get current soil moisture and temperature for any global location
- **Historical Trends** — Analyze soil moisture and temperature patterns over past days, weeks, or months
- **Radius Analysis** — Retrieve soil data for multiple points within a specified radius for spatial analysis
- **Soil Properties** — Access detailed soil composition including texture, organic carbon, pH, and bulk density
- **Grid Mapping** — Generate structured gridded soil data for GIS integration and precision agriculture mapping

### How it works

1. Subscribe to this server
2. Enter your Ambee Soil API key (from the developer dashboard)
3. Start analyzing soil conditions from Claude, Cursor, or any MCP-compatible client

No more manual soil sensor deployment or complex data extraction. Your AI acts as a dedicated soil scientist and agronomist assistant.

### Who is this for?

- **Farmers** — monitor soil moisture for irrigation scheduling and crop health assessment
- **Agronomists** — analyze soil properties, track historical trends, and advise on soil management
- **Researchers** — access global soil datasets for climate studies and agricultural research
- **Landscapers** — check soil conditions for planting optimization and maintenance planning


## Available Tools
- **get_grid_soil**: Returns gridded data points suitable for creating soil condition maps, GIS analysis, and spatial interpolation. Essential for precision agriculture mapping, variable rate application planning, and geospatial soil analysis. AI agents should use this when users ask "generate a soil moisture grid for mapping", "get gridded soil data for my field", or need structured spatial soil data for GIS integration.

Get soil data on a structured grid for spatial analysis and mapping
- **get_historical_soil**: Essential for analyzing soil condition trends, seasonal patterns, drought assessment, and long-term irrigation planning. AI agents should reference this when users ask "show me soil moisture trends over the past 30 days", "what was the soil temperature last week", or need historical soil data for agricultural analysis.

Get historical soil moisture and temperature data for trend analysis
- **get_latest_soil**: Essential for irrigation planning, crop monitoring, soil health assessment, and precision agriculture. AI agents should use this when users ask "what is the soil moisture at my farm", "check current soil temperature", or need immediate soil condition data for agricultural decision making.

Get real-time soil moisture and temperature for a specific location
- **get_soil_by_radius**: Returns an array of soil readings across the area, enabling spatial analysis of soil conditions. Essential for regional soil assessment, field variability analysis, and precision agriculture zone mapping. AI agents should use this when users ask "show me soil conditions within 10km of my location", "get soil data for my entire farm area", or need spatial soil moisture distribution analysis.

Get soil data for multiple points within a radius of a location
- **get_soil_properties**: Essential for soil classification, crop suitability analysis, fertilizer planning, and long-term soil health monitoring. AI agents should reference this when users ask "what is the soil type and pH at my location", "show me soil organic carbon content", or need comprehensive soil property data for agricultural planning.

Get detailed soil physical and chemical properties for a location


## Installation & Usage

To install and use the **Ambee Soil** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ambee-soil](https://vinkius.com/mcp/ambee-soil)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
