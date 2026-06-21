# USGS Earthquakes MCP Server

Tap into the USGS real-time seismic network. Monitor global earthquakes, filter by magnitudes, and run historical analyses instantly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/usgs-earthquakes)

## Overview
**Category:** the-unthinkable
**Tools Count:** 3

## Description
The **USGS Earthquakes MCP Server** brings planet-scale telemetry directly to your AI agent. Pulling strictly real-time and historical data from the United States Geological Survey (USGS) API, this tool gives you instant visibility into everything from micro-tremors to catastrophic seismic events globally.

### Core Capabilities

- **Global Seismic Monitoring** — Query real-time data across the planet.
- **Radial & Bounding Box Search** — Focus searches on specific fault lines, continents, or specific radial points like Tokyo or San Francisco.
- **Magnitude & Time Filters** — Zero in on data by slicing through specific date ranges and Richter thresholds.
- **High-Alert Diagnostics** — Detect immediate tsunami warnings and review detailed human-curated significance ratings.

Whether you are building environmental response bots or running historical data analytics on tectonic shifts, this zero-auth integration puts the pulse of the planet in your hands.


## Available Tools
- **count_earthquakes**: Get the total count of earthquakes matching specific criteria
- **query_earthquakes**: Use parameters like starttime, endtime, minmagnitude, and geographic boundaries (latitude/longitude/maxradiuskm) to narrow the search. Maximum 20,000 events returned per query.

Search for global earthquakes using USGS real-time seismic data
- **get_significant_30_days**: No parameters needed.

Get highly significant global earthquakes from the last 30 days


## Installation & Usage

To install and use the **USGS Earthquakes** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/usgs-earthquakes](https://vinkius.com/mcp/usgs-earthquakes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
