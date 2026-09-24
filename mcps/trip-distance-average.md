# Trip Distance Average MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/trip-distance-average)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [transportation](../categories/transportation.md)

Calculate average distances for individual travel legs and entire fleets.

## Description
This MCP server provides tools to analyze travel segment distances. You can use `get_trip_average_distance` to find the mean distance of legs within a specific journey, `get_fleet_average_distance` to calculate averages across all trips in your dataset, `get_trip_stats` for a full distribution summary including shortest and longest legs, or `get_leg_details` to list every individual segment's distance.


## Available Tools (4)
- **get_fleet_average_distance**: Answers "What is the average leg distance across all trips in the dataset?"
- **get_leg_details**: Answers "What are the individual distances for every segment in a trip?"
- **get_trip_average_distance**: Answers "What was the average distance of each segment in this specific trip?"
- **get_trip_stats**: Answers "Give me a summary of the distance distribution for a specific trip."


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Trip Distance Average** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the average distance of each segment in trip T123?"

**🤖 AI Agent:**
> The average distance for the segments in trip T123 was 15.5 km across 3 legs.

---

**👤 You:**
> "Give me a summary of the distance distribution for trip T456."

**🤖 AI Agent:**
> For trip T456, the shortest leg was 2.0 km, the longest leg was 45.0 km, and the average distance was 18.5 km over 4 legs.

---

**👤 You:**
> "What are the individual distances for every segment in trip T789?"

**🤖 AI Agent:**
> The segments for trip T789 are: leg_001 (10.2 km), leg_002 (5.5 km), and leg_003 (12.3 km).


## ❓ FAQ

**Q: How do I get the average distance for a specific trip?**
Use the `get_trip_average_distance` tool and provide the unique trip ID.

**Q: Can I filter fleet averages by date?**
Yes, the `get_fleet_average_distance` tool allows you to provide optional start and end dates to filter the trips analyzed.

**Q: What kind of statistics can I get for a trip?**
The `get_trip_stats` tool provides the shortest leg, longest leg, average distance, and the total number of legs in the trip.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/trip-distance-average](https://vinkius.com/en/ai-agent-connect/trip-distance-average)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Trip Distance Average** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `trip-distance-average` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Trip Distance Average** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trip-distance-average": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
