# Baidu Huiyan LBS MCP Server

Analyze population mobility via Baidu Huiyan — track migration flows, urban crowd density, and perform precision geocoding from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/baidu-huiyan-lbs)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Connect your AI agents to **Baidu Huiyan** (百度慧眼), Asia's leading macro-scale location intelligence platform. This MCP provides 10 tools to analyze population mobility, urban density patterns, and perform precision geocoding using Baidu's massive LBS data ecosystem.

### What you can do

- **Migration Flow Analysis** — Track population migration patterns between cities and provinces, with daily scale indexes and directional flows
- **Urban Density Monitoring** — Query real-time and historical crowd density data to identify hotspots for event management and commercial planning
- **Precision Geocoding** — Convert addresses to coordinates (BD09ll) and perform reverse geocoding within China's geographic boundaries
- **Area Demographics** — Retrieve population profiles and behavioral patterns for any administrative region
- **POI Search** — Search points of interest within specific regions using Baidu Maps

### How it works

1. Create a developer account on the [**Baidu LBS Open Platform**](https://lbsyun.baidu.com/)
2. Register an application to obtain your **AK (Access Key)**
3. Enable **SN Verification** in the console to generate your **SK (Secret Key)**
4. Enter both keys below — the engine automatically computes the required MD5 SN signature for every request

### Who is this for?

- **Urban Planners** — audit population movement metrics to optimize transit networks
- **Retail Analysts** — identify high-footfall zones for store location planning
- **Logistics Teams** — monitor crowd congestion patterns for route optimization


## Available Tools
- **geocode_address**: Convert a street address to latitude/longitude coordinates
- **get_area_profile**: Get demographic and behavioral profile of a geographic area
- **get_migration_city_rank**: Direction: "in" or "out".

Rank cities by migration flow volume relative to a target area
- **get_migration_province_rank**: Rank provinces by migration flow volume relative to a target area
- **get_migration_scale**: Direction: "in" or "out".

Get population migration intensity index for an area
- **get_population_density**: Get real-time population density heatmap data for an area
- **get_population_flow**: Get population inflow/outflow volumes for an area
- **get_stay_duration**: Get average visitor stay duration for a geographic area
- **reverse_geocode**: Convert latitude/longitude to a structured address
- **search_poi**: Search Points of Interest near a location or region


## Installation & Usage

To install and use the **Baidu Huiyan LBS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baidu-huiyan-lbs](https://vinkius.com/mcp/baidu-huiyan-lbs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
