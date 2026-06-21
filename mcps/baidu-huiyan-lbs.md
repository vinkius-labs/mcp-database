# Baidu Huiyan LBS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/baidu-huiyan-lbs)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/baidu-huiyan-lbs-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/baidu-huiyan-lbs-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Analyze population mobility via Baidu Huiyan — track migration flows, urban crowd density, and perform precision geocoding from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Baidu Huiyan LBS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the crowd density data for the Sanlitun area in Beijing."

**🤖 AI Agent:**
> Querying Huiyan density data... The Sanlitun area (ID: BJ_110105X8) shows a crowd density index of 8.2, at approximately 90% peak capacity. This indicates very high footfall in the retail and entertainment district. Would you like to check adjacent neighborhoods?

---

**👤 You:**
> "Analyze the inbound migration flow to Shanghai for this week."

**🤖 AI Agent:**
> Analyzing migration data for Shanghai (310000)... The inbound flow index averages 7.15 this week. The top origin city is Suzhou at 28% of total inflow, followed by Hangzhou at 15%. Would you like to see the full city ranking or compare with last week?

---

**👤 You:**
> "Geocode 'The Bund, Zhongshan East 1st Road, Huangpu, Shanghai' in BD09ll format."

**🤖 AI Agent:**
> Geocoding complete. Address resolved to: Latitude 31.239722, Longitude 121.493888. Confidence: 99%. Coordinate system: BD09ll (Baidu proprietary). Would you like to reverse-geocode these coordinates or search for nearby POIs?


## Installation & Usage

To install and use the **Baidu Huiyan LBS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baidu-huiyan-lbs](https://vinkius.com/mcp/baidu-huiyan-lbs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
