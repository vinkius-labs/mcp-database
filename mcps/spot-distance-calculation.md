# Spot Distance Calculation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/spot-distance-calculation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate great-circle distances, bearings, and travel times using spherical geometry.

## Description
This MCP server provides precise navigational calculations based on the Haversine formula. It allows AI agents to determine the shortest distance between two geographic points, calculate the required compass bearing, and estimate travel time based on speed. Use `get_distance_and_bearing` to find distance and direction, `calculate_estimated_travel_time` for duration, `verify_navigation_feasibility` to check heading constraints, and `get_distance_to_landmark_collection` to find the nearest point in a list.


## Available Tools (4)
- **verify_navigation_feasibility**: Verifies if the target bearing is within the allowed deviation
- **calculate_estimated_travel_time**: Calculates the estimated travel time in minutes
- **get_distance_and_bearing**: Calculates the great-circle distance and bearing between two points
- **get_distance_to_landmark_collection**: Finds the closest landmark in a collection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spot Distance Calculation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How far is it from latitude 40.7128, longitude -74.0060 to latitude 34.0522, longitude -118.2437?"

**🤖 AI Agent:**
> The distance is approximately 3935.74 km with a bearing of 259.32 degrees.

---

**👤 You:**
> "If I am 100 km away and traveling at 50 kph, how long will it take to arrive?"

**🤖 AI Agent:**
> It will take 120 minutes to reach your destination.

---

**👤 You:**
> "I am facing 90 degrees. Is it feasible to reach a target at 100 degrees if my max deviation is 15 degrees?"

**🤖 AI Agent:**
> No, the angular difference is 10 degrees, which is within the 15 degree limit, so it is feasible.


## ❓ FAQ

**Q: How is the distance calculated?**
The distance is calculated using the Haversine formula, which accounts for the Earth's curvature to provide the shortest great-circle distance.

**Q: Can I find the closest landmark from a list?**
Yes, you can use the `get_distance_to_landmark_collection` tool to identify the nearest landmark from a provided array of coordinates.

**Q: Does it support bearing calculations?**
Yes, the `get_distance_and_bearing` tool provides the compass bearing (0-360 degrees) required to reach a target destination.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/spot-distance-calculation](https://vinkius.com/ai-agent-connect/spot-distance-calculation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spot Distance Calculation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spot-distance-calculation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spot Distance Calculation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spot-distance-calculation": {
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
