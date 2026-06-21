# NOAA Space Weather — Solar & Geomagnetic Intelligence MCP Server

Real-time space weather intelligence: planetary Kp geomagnetic index, 3-day Kp forecast, solar wind speed and magnetic field, aurora probability forecast (Ovation model), solar flux (F10.7), and Dst storm index from NOAA SWPC.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/noaa-space-weather-solar-geomagnetic-intelligence)

## Overview
**Category:** the-unthinkable
**Tools Count:** 6

## Description
Real-time space weather from NOAA's Space Weather Prediction Center.

### What you can do
- **Kp Index** — Current geomagnetic activity (aurora threshold)
- **Kp Forecast** — 3-day predictions
- **Solar Wind** — Speed (km/s) and Bz from DSCOVR satellite
- **Aurora Forecast** — Ovation probability model (global)
- **Solar Flux** — F10.7 solar activity proxy
- **Dst Index** — Ring current storm intensity

### Who Needs This?
Aurora hunters, satellite operators, HF radio operators, power grid managers, airline operators (polar routes), and space enthusiasts.


## Available Tools
- **get_planetary_k_index**: Kp ranges 0-9. Values ≥5 indicate geomagnetic storms with visible aurora at lower latitudes. Updated every 3 hours. Essential for aurora hunters, satellite operators, and power grid managers.

Get the NOAA Planetary K-index — geomagnetic activity and aurora probability
- **get_k_index_forecast**: Use this to plan for aurora viewing, satellite vulnerabilities, or HF radio propagation impacts.

Get the 3-day Kp index forecast — predicted geomagnetic activity
- **get_solar_wind**: The solar wind drives geomagnetic storms — when speed exceeds 500 km/s with southward Bz, aurora probability increases dramatically.

Get real-time solar wind speed and magnetic field conditions
- **get_aurora_forecast**: Powered by real-time solar wind data. The gold standard for aurora forecasting worldwide.

Get the aurora probability forecast map data (Ovation model)
- **get_solar_flux**: 7 solar flux index. Higher values (>100 SFU) indicate increased solar activity, more sunspots, and higher probability of solar flares and CMEs. Normal quiet-sun values are 70-80 SFU.

Get the 10.7cm solar radio flux — a proxy for solar activity level
- **get_dst_index**: Measures the intensity of the ring current around Earth. Values below -50 nT indicate a moderate storm, below -100 nT a strong storm, below -250 nT a severe storm. Critical for satellite operators and power grid monitoring.

Get the Dst index — real-time geomagnetic storm intensity


## Installation & Usage

To install and use the **NOAA Space Weather — Solar & Geomagnetic Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/noaa-space-weather-solar-geomagnetic-intelligence](https://vinkius.com/mcp/noaa-space-weather-solar-geomagnetic-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
