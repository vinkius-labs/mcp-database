# USGS Earthquakes MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/usgs-earthquakes)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/usgs-earthquakes-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/usgs-earthquakes-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Tap into the USGS real-time seismic network. Monitor global earthquakes, filter by magnitudes, and run historical analyses instantly.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **USGS Earthquakes** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the most significant earthquakes in the world from the last 30 days."

**🤖 AI Agent:**
> I've pulled the recent significant earthquakes from USGS. We've recorded an M 6.8 near Taiwan and an M 7.2 off the coast of Alaska. There are currently no tsunami warnings.

---

**👤 You:**
> "Count the number of earthquakes above magnitude 2.5 in California in 2023."

**🤖 AI Agent:**
> Based on the USGS database, there were exactly 4,312 earthquakes above magnitude 2.5 within the California coordinate bounds throughout 2023.

---

**👤 You:**
> "Check if there are any current tsunami warnings globally."

**🤖 AI Agent:**
> I checked the USGS sensors. No events currently trigger a tsunami warning. The highest alert level across all oceanic faults in the last 24 hours remains green.


## Installation & Usage

To install and use the **USGS Earthquakes** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/usgs-earthquakes](https://vinkius.com/mcp/usgs-earthquakes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
