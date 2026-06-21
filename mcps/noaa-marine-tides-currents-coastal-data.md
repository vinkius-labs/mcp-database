# NOAA Marine — Tides, Currents & Coastal Data MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/noaa-marine-tides-currents-coastal-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/noaa-marine-tides-currents-coastal-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/noaa-marine-tides-currents-coastal-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

US coastal oceanographic data: real-time water levels (tides), tide predictions, ocean currents, water temperature, coastal meteorological conditions, and multi-decade sea level rise trends from NOAA CO-OPS stations.

## Description
Complete US coastal data from NOAA's Center for Operational Oceanographic Products and Services.

### What you can do
- **Water Levels** — Real-time tides from 200+ stations
- **Tide Predictions** — Hi/lo tide forecasts
- **Currents** — Speed and direction
- **Water Temperature** — Coastal water temps
- **Met Data** — Air temp, wind, pressure at coastal stations
- **Sea Level Trends** — Decades of sea level rise data


## Available Tools
- **get_water_levels**: Data in meters relative to station datum. Provide a CO-OPS station ID (e.g., 8518750 for The Battery, NYC; 9414290 for San Francisco).

Get observed water levels (tides) at a US coastal station
- **get_tide_predictions**: Provides predicted high and low tide times and heights. Useful for fishing, boating, coastal activities. Default is next 48 hours.

Get tide predictions (hi/lo) for a US coastal station
- **get_currents**: Available at select CO-OPS stations with current meters.

Get observed ocean current speed and direction at a US coastal station
- **get_water_temperature**: Useful for marine biology, fishing, surfing, and coastal research.

Get water temperature at a US coastal station
- **get_meteorological**: Complements water-level data for a complete coastal picture.

Get coastal meteorological data: air temp, wind, pressure at a station
- **get_sea_level_trends**: Shows long-term relative sea level trends calculated from decades of tide gauge data. Critical for climate research.

Get long-term sea level rise trends for a US coastal station


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NOAA Marine — Tides, Currents & Coastal Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the tide predictions for today at The Battery, NYC?"

**🤖 AI Agent:**
> 🌊 **The Battery (8518750) — Tide Predictions**

| Time | Type | Height |
|------|------|--------|
| 5:42 AM | Low | 0.12 m |
| 11:58 AM | High | 1.52 m |
| 6:15 PM | Low | 0.08 m |
| 12:22 AM | High | 1.48 m |

Tidal range: 1.44 m. Semi-diurnal pattern.

---

**👤 You:**
> "What is the current water temperature in San Francisco Bay?"

**🤖 AI Agent:**
> At the San Francisco station (9414290), the current water temperature is 57.2°F (14.0°C). Air temperature is 59°F, with winds blowing from the WNW at 15 knots.

---

**👤 You:**
> "Show me the sea level rise trend for Miami over the last 50 years."

**🤖 AI Agent:**
> At the Virginia Key station in Miami (8723214), relative sea level has been rising at an average rate of 3.01 millimeters per year based on data from 1931 to present.


## Installation & Usage

To install and use the **NOAA Marine — Tides, Currents & Coastal Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/noaa-marine-tides-currents-coastal-data](https://vinkius.com/mcp/noaa-marine-tides-currents-coastal-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
