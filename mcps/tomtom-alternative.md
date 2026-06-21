# TomTom MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tomtom-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tomtom-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tomtom-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [geocoding-maps](../categories/geocoding-maps.md)

Access global mapping, geocoding, and routing services. Search for addresses, calculate optimal routes, and retrieve map tiles directly through AI.

## Description
Connect **TomTom**'s industry-leading location technology to your AI agent to unlock powerful spatial intelligence and navigation capabilities.

### What you can do

- **Fuzzy Search** — Find addresses, points of interest (POIs), and streets using flexible, free-text queries.
- **Geocoding** — Convert structured addresses into precise geographic coordinates for mapping and analysis.
- **Smart Routing** — Calculate optimal paths between locations with support for real-time traffic, vehicle types (truck, car, bicycle), and travel modes.
- **Advanced Logistics** — Use advanced routing for route reconstruction with supporting points and avoid specific country vignettes.
- **Map Visualization** — Retrieve raster map tiles (basic, hybrid, or labels) to visualize locations in different styles like 'main' or 'night'.

### How it works

1. Subscribe to this server
2. Enter your TomTom API Key
3. Start querying locations and routes from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Fleet Managers** — optimize delivery routes and calculate travel times based on vehicle profiles.
- **Travel & Hospitality** — help users find points of interest and navigate between destinations.
- **Developers** — integrate location-based context into applications without leaving the chat or IDE.


## Available Tools
- **calculate_advanced_route**: Calculate an advanced route with supporting points or avoid vignettes
- **calculate_route**: Calculate a route between origin and destination
- **geocode**: Convert addresses into geographic coordinates
- **get_map_tile**: Returns the URL to the tile image.

Get a raster map tile URL
- **fuzzy_search**: Single-line fuzzy search for addresses and POIs
- **get_traffic_incidents**: Get real-time traffic incidents and flow information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TomTom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Eiffel Tower' in Paris using fuzzy search."

**🤖 AI Agent:**
> I found the Eiffel Tower at Champ de Mars, 5 Av. Anatole France, 75007 Paris, France. Coordinates: 48.8584, 2.2945.

---

**👤 You:**
> "Calculate a car route from 52.509,13.429 to 52.502,13.438."

**🤖 AI Agent:**
> The fastest route by car is approximately 1.2km and will take about 4 minutes with current traffic conditions.

---

**👤 You:**
> "Get a basic map tile URL for zoom level 15 at x=17600, y=10700."

**🤖 AI Agent:**
> Here is the URL for the requested map tile: https://api.tomtom.com/map/1/tile/basic/main/15/17600/10700.png?key=YOUR_API_KEY


## Installation & Usage

To install and use the **TomTom** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tomtom-alternative](https://vinkius.com/mcp/tomtom-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
