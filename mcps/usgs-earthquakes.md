# USGS Earthquakes MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/usgs-earthquakes)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Tap into the USGS real-time seismic network. Monitor global earthquakes, filter by magnitudes, and run historical analyses instantly.

## Description
The **USGS Earthquakes MCP Server** brings planet-scale telemetry directly to your AI agent. Pulling strictly real-time and historical data from the United States Geological Survey (USGS) API, this tool gives you instant visibility into everything from micro-tremors to catastrophic seismic events globally.

### Core Capabilities

- **Global Seismic Monitoring** — Query real-time data across the planet.
- **Radial & Bounding Box Search** — Focus searches on specific fault lines, continents, or specific radial points like Tokyo or San Francisco.
- **Magnitude & Time Filters** — Zero in on data by slicing through specific date ranges and Richter thresholds.
- **High-Alert Diagnostics** — Detect immediate tsunami warnings and review detailed human-curated significance ratings.

Whether you are building environmental response bots or running historical data analytics on tectonic shifts, this zero-auth integration puts the pulse of the planet in your hands.


## Available Tools (3)
- **count_earthquakes**: Get the total count of earthquakes matching specific criteria
- **query_earthquakes**: Use parameters like starttime, endtime, minmagnitude, and geographic boundaries (latitude/longitude/maxradiuskm) to narrow the search. Maximum 20,000 events returned per query.

Search for global earthquakes using USGS real-time seismic data
- **get_significant_30_days**: No parameters needed.

Get highly significant global earthquakes from the last 30 days


## 💬 Prompt Examples

Here are some examples of how you can interact with the **USGS Earthquakes** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the most significant earthquakes in the world from the last 30 days."

**🤖 AI Agent:**
> I've pulled the recent significant earthquakes from USGS. We've recorded an M 6.8 near Taiwan and an M 7.2 off the coast of Alaska. There are currently no tsunami warnings.

---

**👤 You:**
> "Count the number of earthquakes above magnitude 2.5 in California in 2023."

**🤖 AI Agent:**
> Based on the USGS database, there were exactly 4,312 earthquakes above magnitude 2.5 within the California coordinate bounds throughout 2023.

---

**👤 You:**
> "Check if there are any current tsunami warnings globally."

**🤖 AI Agent:**
> I checked the USGS sensors. No events currently trigger a tsunami warning. The highest alert level across all oceanic faults in the last 24 hours remains green.


## ❓ FAQ

**Q: Is an API key required?**
No! The USGS FDSNWS Event API is completely open and requires zero authentication, making this one of the most accessible and powerful real-time data sources available.

**Q: What is the query limit?**
The maximum number of events returned per single API query is 20,000. If your time range or boundaries are too wide, the API will fail. Use the `count` tool first on large searches.

**Q: How fast is the data updated?**
The USGS typically updates its earthquake data within minutes of an event occurring, making it one of the most reliable sources for near real-time seismic alerts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/usgs-earthquakes](https://vinkius.com/mcp/usgs-earthquakes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **USGS Earthquakes** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `usgs-earthquakes` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **USGS Earthquakes** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "usgs-earthquakes": {
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
