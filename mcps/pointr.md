# Pointr MCP Server

Grant your AI access to precision indoor mapping. Navigate buildings, track BLE beacons, and find POIs.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pointr)

## Overview
**Category:** iot-hardware
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Pointr** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pointr](https://vinkius.com/mcp/pointr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
