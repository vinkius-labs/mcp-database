# Pointr MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pointr)
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


## ❓ FAQ

**Q: Can the agent calculate walking paths across multiple floors?**
Yes. When triggering `calculate_path` supplied with explicit coordinate pairings spanning different Level UUIDs, the Pointr engine bridges the wayfinding automatically. It factors in fixed transitions like elevators or stairs natively, feeding the Agent the comprehensive turn-by-turn array in JSON format seamlessly.

**Q: Is it possible to extract the giant raw map shapes for a given floor?**
Absolutely. By initiating the query `get_level_map` tied securely to a single level UUID, the interface processes and downloads massive explicit geometries mapping out physical walls, traversable space nodes, and internal partitions explicitly generated by the Pointr pipeline.

**Q: Can I search for specific stores or bathrooms using text queries?**
Yes. Pointr exposes dense fuzzy logic matching indexes. When the Agent executes `search_pois` feeding a literal keyword alongside the Target Building ID, it reliably unearths precisely mapped nodes conforming to 'Restroom', 'Exit', or custom store names embedded dynamically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pointr](https://vinkius.com/mcp/pointr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pointr** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pointr` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pointr** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pointr": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
