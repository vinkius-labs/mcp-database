# MapQuest MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mapquest)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mapquest-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mapquest-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Mapping and location services via MapQuest — geocoding, directions, and POI search.

## Description
Connect your AI agent to MapQuest, one of the pioneers in online mapping. This integration provides essential geographic tools, from converting addresses to coordinates to calculating detailed travel routes.

### What you can do

- **Geocoding** — Convert street addresses into precise latitude and longitude coordinates
- **Reverse Geocoding** — Identify the human-readable address for any GPS coordinate
- **Detailed Directions** — Get turn-by-turn routing for driving, walking, or cycling, including distance and time estimates
- **POI Search** — Find nearby businesses and points of interest like restaurants, gas stations, or parks
- **Static Maps** — Generate URLs for visual map images centered on any location

### How it works

1. Subscribe to this server
2. Enter your **MapQuest Consumer Key** (available at the MapQuest Developer Network)
3. Use natural language to ask for directions or geographic lookups

### Who is this for?

- **Travelers** — quickly get directions and travel times during planning
- **Logistics Managers** — automate coordinate lookups and routing calculations
- **Local Researchers** — find businesses and services in any specific area


## Available Tools
- **geocode_address**: Convert an address into geographic coordinates (latitude and longitude)
- **get_directions**: Get driving, walking, or cycling directions between two locations
- **get_static_map_url**: Generate a static map image URL for a specific location
- **reverse_geocode**: Convert geographic coordinates (latitude and longitude) into a human-readable address
- **search_points_of_interest**: Search for specific places (restaurants, gas stations, etc.) around a location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MapQuest** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the coordinates for the White House?"

**🤖 AI Agent:**
> The coordinates for 1600 Pennsylvania Ave NW are latitude 38.897675 and longitude -77.036547.

---

**👤 You:**
> "Get driving directions from New York to Philadelphia."

**🤖 AI Agent:**
> The estimated travel time is 1 hour and 45 minutes (approx. 94 miles). The route starts via I-95 South...


## Installation & Usage

To install and use the **MapQuest** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mapquest](https://vinkius.com/mcp/mapquest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
