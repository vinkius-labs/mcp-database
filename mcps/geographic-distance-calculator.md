# Geographic Distance Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/geographic-distance-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate precise distances, bearings, and waypoints using Haversine, Vincenty, and Euclidean models.

## Description
A high-precision geospatial utility for calculating distances, bearings, waypoints, and bounding areas. This MCP server provides specialized tools to compute the distance between two coordinates using multiple mathematical models: `calculate_distance` (Haversine, Vincenty, or Euclidean), `compute_destination` for finding a point based on bearing and travel distance, `get_midpoint` for geographic centers, `get_bearing_stats` for initial and final bearings, and `generate_bounding_box` to define rectangular areas around a radius.


## Available Tools (5)
- **get_bearing_stats**: Get bearing statistics between two points
- **generate_bounding_box**: Generate a bounding box for a circular area
- **compute_destination**: Compute a destination point based on bearing and distance
- **calculate_distance**: Calculate the distance between two geographic points
- **get_midpoint**: Find the midpoint between two points


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Geographic Distance Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the distance between New York (40.7128, -74.0060) and London (51.5074, -0.1278) using the Haversine formula?"

**🤖 AI Agent:**
> The distance between New York and London is approximately 5,570 km (3,461 miles or 3,007 nautical miles).

---

**👤 You:**
> "Calculate the destination if I start at (0, 0) and travel 1000 meters at a bearing of 90 degrees."

**🤖 AI Agent:**
> The destination coordinates are Latitude: 0.0, Longitude: 0.00899 (approximately 1km East).

---

**👤 You:**
> "Find the midpoint between Tokyo (35.6895, 139.6917) and Sydney (-33.8688, 151.2093)."

**🤖 AI Agent:**
> The geographic midpoint is located at approximately Latitude: -0.145, Longitude: 145.45.


## ❓ FAQ

**Q: Which calculation method should I use for distance?**
Use `haversine` for most general-purpose needs as it is efficient and accurate. Use `vincenty` when high precision is required for long-distance navigation, as it accounts for the Earth's ellipsoidal shape. Use `euclidean` only for extremely short distances where curvature is negligible.

**Q: Can I find the center point between two cities?**
Yes, you can use the `get_midpoint` tool to find the geographic center along the great-circle path between any two sets of coordinates.

**Q: Does the server support different distance units?**
Yes, all distance results from `calculate_distance` are returned in meters, kilometers, miles, and nautical miles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/geographic-distance-calculator](https://vinkius.com/mcp/geographic-distance-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Geographic Distance Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `geographic-distance-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Geographic Distance Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "geographic-distance-calculator": {
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
