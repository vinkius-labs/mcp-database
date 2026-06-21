# Renfe Data MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/renfe-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/renfe-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/renfe-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Access real-time train positions, trip updates, and open datasets from Renfe, Spain's national railway operator.

## Description
Connect to the **Renfe Data** portal to monitor the Spanish railway network in real-time. This server provides comprehensive access to both live operational data and static historical datasets through the official CKAN infrastructure.

### What you can do

- **Real-time Tracking** — Get precise GPS locations and movement status for Cercanías (commuter) and Long Distance (AVE/LD/MD) trains.
- **Trip Updates & Delays** — Monitor live delays, cancellations, and platform changes to keep travelers informed.
- **CKAN Portal Access** — List, search, and inspect metadata for thousands of railway datasets and resources.
- **Service Alerts** — Retrieve real-time information on accessibility issues, track incidents, or bus substitutions.
- **Static Schedules** — Fetch direct download URLs for GTFS schedules and station lists for offline analysis.

### How it works

1. Subscribe to this server
2. Enter your Renfe Data API Key
3. Start querying Spanish railway data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Transport Analysts** — track fleet movements and analyze network performance metrics.
- **Travel App Developers** — integrate real-time Spanish train data and GTFS schedules into custom applications.
- **Data Scientists** — access open government data for urban mobility research and visualization.


## Available Tools
- **ckan_datastore_search**: Search for data within a resource
- **ckan_package_list**: List all dataset names in Renfe Data
- **ckan_package_show**: Get metadata for a specific dataset
- **ckan_resource_show**: Get metadata for a specific resource
- **get_avisos**: Get planned service modifications (Avisos)
- **get_static_datasets**: List URLs for static datasets (Schedules & Stations)
- **rt_alerts_cercanias**: Updates every 20 seconds.

Get real-time service alerts for Cercanías
- **rt_trip_updates_cercanias**: Updates every 20 seconds.

Get real-time trip updates for Cercanías
- **rt_trip_updates_ld**: Updates every 30 seconds.

Get real-time trip updates for AV / LD / MD
- **rt_vehicle_positions_cercanias**: Updates every 20 seconds.

Get real-time vehicle positions for Cercanías
- **rt_vehicle_positions_ld**: Updates every 15 minutes.

Get real-time vehicle positions for AV / LD / MD


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Renfe Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available dataset names in the Renfe Data portal."

**🤖 AI Agent:**
> I've retrieved the list of datasets. There are several available, including 'Estaciones', 'Horarios-GTFS', and 'Ocupacion-Trenes'. Which one would you like to explore further?

---

**👤 You:**
> "Show me the current real-time positions of Cercanías trains."

**🤖 AI Agent:**
> Fetching live GPS data... I found 42 trains currently active. For example, train C-4 is currently moving near Madrid-Atocha (Lat: 40.406, Lon: -3.692). Would you like a full list or a specific line?

---

**👤 You:**
> "Are there any trip updates or delays for Long Distance trains right now?"

**🤖 AI Agent:**
> Checking trip updates for AV/LD/MD... I see a 10-minute delay for the AVE 03122 from Barcelona to Madrid due to a technical check. Other services are running on time. Should I check for alerts in specific regions?


## Installation & Usage

To install and use the **Renfe Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/renfe-data](https://vinkius.com/mcp/renfe-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
