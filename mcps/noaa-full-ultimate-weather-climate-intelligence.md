# NOAA Full — Ultimate Weather & Climate Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/noaa-full-ultimate-weather-climate-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/noaa-full-ultimate-weather-climate-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/noaa-full-ultimate-weather-climate-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

The definitive NOAA Mega-Server: 36 tools spanning weather forecasts, severe alerts, current observations, aviation METARs/TAFs, marine tides and currents, space weather aurora and solar wind, and decades of historical climate records — all from 5 official NOAA APIs.

## Description
The **ultimate NOAA Mega-Server** — 36 tools across 7 domains from 5 official APIs.

### 36 Tools
- 🌤️ Forecast (5) — Daily, hourly, grid, AFD, metadata
- ⚠️ Alerts (4) — By state, zone, point, types
- 📡 Observations (5) — Stations, current, history, radar
- ✈️ Aviation (5) — METAR, TAF, PIREP, SIGMET, station
- 🌊 Marine (6) — Tides, predictions, currents, water temp, met, sea level
- ☀️ Space (6) — Kp, forecast, solar wind, aurora, flux, Dst
- 📊 Climate (5) — Daily, monthly, yearly, normals, station search

### No API Key Required


## Available Tools
- **get_active_alerts**: Filter by state (2-letter code: TX, FL, CA), severity (Extreme, Severe, Moderate, Minor), urgency (Immediate, Expected, Future), or event type (Tornado Warning, Hurricane Warning, etc.).

Get active weather alerts by US state or severity
- **get_alerts_by_zone**: g., TXZ211, FLZ050). Zone IDs can be found via the get_point_metadata tool. Useful for focused monitoring of a specific area.

Get active weather alerts for a specific NWS zone
- **get_alerts_by_point**: Internally resolves the location to find active alerts in that area.

Get active weather alerts for a specific US latitude/longitude
- **get_alert_types**: ). Use this to discover valid event type values for filtering alerts.

List all NWS weather alert types available
- **get_metar**: Provide ICAO codes comma-separated (KJFK, EGLL, LFPG). Returns temperature, wind, visibility, clouds, pressure, weather phenomena. Optionally retrieve past hours of data.

Get METAR (current airport weather) for any airport worldwide by ICAO code
- **get_taf**: Includes forecast groups with wind, visibility, clouds, and weather changes. ICAO codes only.

Get TAF (airport weather forecast) for any airport worldwide by ICAO code
- **get_pirep**: Filter by age (hours).

Get PIREPs (Pilot Reports) for turbulence, icing, and weather conditions
- **get_sigmet**: These define areas of significant weather hazards for aviation: convection, turbulence, icing, IFR conditions, mountain obscuration.

Get SIGMETs and AIRMETs — significant aviation weather hazards
- **get_aviation_station**: Use ICAO codes (KJFK, EGLL, LFPG, SBGR).

Get aviation weather station information by ICAO code
- **get_daily_data**: This is the planet's largest archive of daily weather records. Filter by station, data types (TMAX, TMIN, PRCP, SNOW, SNWD), and date range. Stations are worldwide but densest coverage is in the US.

Get daily weather data (GHCN-Daily): temperatures, precipitation, snow
- **get_monthly_summary**: Monthly aggregates of temperature averages, precipitation totals, and degree days. Less granular than daily but ideal for climate trend analysis.

Get monthly climate summary (GSOM): average temp, total precipitation, heating degree days
- **get_yearly_summary**: Yearly temperature averages, precipitation totals, and extreme values. Perfect for long-term climate analysis spanning decades.

Get annual climate summary (GSOY): yearly averages and extremes
- **get_climate_normals**: This is the statistical baseline that defines "normal" weather for any location.

Get 30-year climate normals — the baseline for what is "normal" weather
- **search_stations**: Returns station IDs, names, and locations for use with other climate tools.

Search NCEI weather stations by location bounding box or keyword
- **get_forecast**: Provide latitude and longitude for any US location. Returns high/low temps, wind speed/direction, precipitation probability, and detailed narrative.

Get 7-day weather forecast for a US location by latitude and longitude
- **get_hourly_forecast**: 5 days. Includes temperature, wind, humidity, precipitation, and sky condition for each hour. US locations only.

Get hour-by-hour weather forecast (156 hours) for a US location
- **get_forecast_discussion**: Use the 3-letter WFO code (e.g., OKX=New York, LAX=Los Angeles, MFL=Miami). Lists recent product IDs — retrieve the latest for full text.

Get the Area Forecast Discussion (AFD) from a NWS Weather Forecast Office
- **get_grid_data**: Useful for programmatic analysis. US only.

Get raw NWS grid weather data: temperature, precipitation, wind, humidity arrays
- **get_point_metadata**: US locations only.

Get NWS metadata for a US location: responsible WFO, grid coordinates, zones
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
- **get_stations**: Each station has a 4-character ID (e.g., KJFK, KLAX). US only. Use station IDs with get_latest_observation.

Find nearby NWS weather observation stations by latitude/longitude
- **get_latest_observation**: Provide a 4-character station ID such as KJFK, KLAX, KORD, KDFW.

Get current weather conditions from a specific NWS station
- **get_observation_history**: Useful for seeing temperature trends, wind changes, and weather evolution over recent hours.

Get recent observation history for a NWS station
- **get_station_metadata**: Useful for understanding where a station is and what data it provides.

Get metadata about a specific NWS weather station
- **get_radar_stations**: List all NWS radar stations and their status
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NOAA Full — Ultimate Weather & Climate Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Full weather briefing: NYC forecast, alerts, airport conditions, and tides"

**🤖 AI Agent:**
> 🗽 **NYC Full Briefing**

🌤️ Forecast: Partly cloudy, High 72°F, T-storms Thursday
⚠️ Alerts: None active for NYC metro
✈️ KJFK METAR: 22°C, SW 12kt, SCT030, VIS 10+
🌊 Battery Tide: High 1.52m at 11:58 AM

4 NOAA systems queried simultaneously.

---

**👤 You:**
> "Is there any space weather activity and can I see the aurora?"

**🤖 AI Agent:**
> 🌌 **Space Weather + Aurora Check**

Kp: 4 (Active), Forecast: 5 tonight
Solar Wind: 520 km/s, Bz: -6 nT ✅
Dst: -42 nT (mild disturbance)
F10.7 Flux: 155 SFU (elevated)

Aurora visible tonight from northern US states and southern Canada.


## Installation & Usage

To install and use the **NOAA Full — Ultimate Weather & Climate Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/noaa-full-ultimate-weather-climate-intelligence](https://vinkius.com/mcp/noaa-full-ultimate-weather-climate-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
