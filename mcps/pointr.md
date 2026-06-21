# Pointr MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pointr)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pointr-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pointr-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Grant your AI access to precision indoor mapping. Navigate buildings, track BLE beacons, and find POIs.

## Description
Bring deep indoor location intelligence directly to your AI operations using the **Pointr** network. This MCP integration securely bridges your LLM to complex structural databases plotting multi-floor layouts, indoor geo-fencing, and Bluetooth Low Energy (BLE) beacon networks. Instead of navigating complicated dashboards to audit facility paths, simply instruct your local Agent to parse physical building parameters perfectly.

### What you can do

- **Facility Exploration** — Understand global deployments natively. Run `list_buildings` and `list_levels` to mathematically visualize vertical architectures and floor limits.
- **Precision Wayfinding** — Query active Point of Interest objects. The agent leverages `search_pois` to find specific gates/stores, and dynamically invokes `calculate_path` predicting multi-floor walking paths avoiding structural walls.
- **Infrastructure Auditing** — Ask the AI to evaluate BLE hardware mesh footprints using the `list_beacons` utility, verifying precisely where physical network sensors reside inside map geometries.
- **Geo-Fence Parsing** — Interrogate proactive indoor trigger zones. `list_geofences` brings back complex logical polygons mapping where local alerts fire globally.

### How it works

1. Append the Pointr connector directly into your MCP cluster
2. Introduce your explicit Enterprise Bearer Token into the configuration vault
3. Begin instructing your LLM to dissect and verify massive indoor mapping models natively

### Who is this for?

- **Facilities Managers** — script AI routines to passively ping `list_beacons` and cross-reference them against active floor geometries to spot offline hardware.
- **Spatial Data Engineers** — command the assistant to extract massive layout configurations using `get_level_map` isolating routing constraints directly into code context.
- **Aviation & Retail Planners** — ask the LLM to run batch test queries calling `calculate_path` to simulate crowd flow and optimal step logic across massive airport or mall nodes.


## Available Tools
- **calculate_path**: Calculate the optimal indoor wayfinding path between two points
- **get_building**: Retrieve detailed configuration for a specific Pointr building
- **get_level_map**: Retrieve the floor plan map data for a specific building level
- **get_poi**: Retrieve detailed information for a specific Pointr POI
- **list_beacons**: List all BLE beacons deployed and registered in the Pointr platform
- **list_buildings**: List all buildings registered in the Pointr indoor intelligence platform
- **list_geofences**: List all indoor geofences configured in the Pointr platform
- **list_levels**: List all floor levels for a specific Pointr building
- **list_pois**: List all Points of Interest (POIs) registered in the Pointr platform
- **search_pois**: Search for indoor Points of Interest by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pointr** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active building deployments registered in our Pointr instance."

**🤖 AI Agent:**
> Command dispatched calling `list_buildings`. Extracted active mapping footprint indicating 3 explicit registered geographic facilities. Node list comprises `London HQ`, `Terminal B (Miami)`, and `Dubai Mall`. Do you hold operations over a specific building id to extract further details?

---

**👤 You:**
> "Search for all restrooms securely listed under building ID `b1b2-c3c4`."

**🤖 AI Agent:**
> Fuzzy node invocation engaged using `search_pois`. Tied keyword explicitly to building UUID parameter. The payload digested successfully revealing an array of 6 distinctly leveled 'Restroom' entities covering the Ground up to Level 3 boundaries natively. Mapping nodes cached.

---

**👤 You:**
> "Calculate indoor path from POI `poi_origin` to `poi_destination`."

**🤖 AI Agent:**
> Graph pathing computations dispatched under `calculate_path`. Pointr core algorithm solved spatial routing effectively spanning a 128-meter walking progression mapped across 2 floor transitions involving escalator node identifiers. Total array sequences delivered.


## Installation & Usage

To install and use the **Pointr** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pointr](https://vinkius.com/mcp/pointr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
