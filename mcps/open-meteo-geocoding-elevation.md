# Open-Meteo Geocoding & Elevation MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-meteo-geocoding-elevation)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/open-meteo-geocoding-elevation-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/open-meteo-geocoding-elevation-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Resolve any city, village, or address into GPS coordinates instantly: multilingual search, population data, timezones, and terrain elevation at 90m precision — the perfect companion for all weather tools.

## Description
The essential **utility server** that powers location-aware AI agents.

### What you can do
- **Global Search** — Find any city or village by name in any language, get lat/lon, elevation, population, timezone, and postal codes
- **Terrain Elevation** — Get precise elevation in meters for any GPS coordinate using a 90-meter digital elevation model
- **Country Filtering** — Search locations within specific countries using ISO codes

### Who is this for?
Developers, data engineers, travel apps, logistics platforms, and any AI agent that needs to convert place names into actionable coordinates.


## Available Tools
- **search_location**: Supports any language.

Search for cities and locations globally
- **get_elevation**: Get terrain elevation for any coordinates
- **search_location_by_country**: g., US, BR, DE, FR).

Search locations filtered by country


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open-Meteo Geocoding & Elevation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where exactly is Machu Picchu? Give me coordinates and elevation."

**🤖 AI Agent:**
> 📍 **Machu Picchu**

Latitude: -13.1631
Longitude: -72.5450
Elevation: 2,430m above sea level
Timezone: America/Lima (UTC-5)
Country: Peru 🇵🇪
Admin region: Cusco

---

**👤 You:**
> "Find all cities named 'Springfield' in the United States"

**🤖 AI Agent:**
> 🏘️ **Springfield — US Results**

1. Springfield, IL — Pop: 114,394 (39.80°N, 89.64°W)
2. Springfield, MO — Pop: 169,176 (37.22°N, 93.29°W)
3. Springfield, MA — Pop: 155,929 (42.10°N, 72.59°W)
4. Springfield, OH — Pop: 58,662
5. Springfield, OR — Pop: 62,979

10 results found across 10 different states.

---

**👤 You:**
> "What's the elevation of Mount Kilimanjaro's summit?"

**🤖 AI Agent:**
> 🏔️ **Mount Kilimanjaro — Uhuru Peak**

Elevation: 5,895m (19,341 ft)
Coordinates: -3.0674°S, 37.3556°E
Country: Tanzania 🇹🇿

Highest point in Africa and the tallest free-standing mountain in the world.


## Installation & Usage

To install and use the **Open-Meteo Geocoding & Elevation** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-meteo-geocoding-elevation](https://vinkius.com/mcp/open-meteo-geocoding-elevation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
