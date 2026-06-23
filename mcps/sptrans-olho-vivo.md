# SPTrans Olho Vivo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sptrans-olho-vivo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time public transit data for São Paulo — track bus positions, check arrival forecasts, and locate stops across the city.

## Description
Connect to the **SPTrans Olho Vivo** API to bring real-time urban mobility intelligence to your AI agent. Monitor the entire São Paulo bus fleet and provide precise transit information through natural conversation.

### What you can do

- **Line & Stop Discovery** — Search for bus lines by name or number and find specific stops by address or corridor.
- **Real-time GPS Tracking** — Fetch the exact coordinates of active buses on any given line or across the entire city fleet.
- **Arrival Forecasts** — Get accurate predictions for when the next bus will arrive at a specific stop or for all stops along a route.
- **Corridor & Company Info** — List intelligent bus corridors and operating companies to understand the city's transit infrastructure.
- **Garage Status** — Monitor vehicles currently in the garage for specific companies and lines.

### How it works

1. Subscribe to this server
2. Enter your SPTrans Olho Vivo API Token
3. Start querying São Paulo's transit system from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Commuters & Residents** — Get instant updates on bus arrivals and locations without switching between multiple transit apps.
- **Urban Planners & Researchers** — Analyze real-time fleet distribution and corridor efficiency directly through AI-driven data extraction.
- **Developers** — Integrate São Paulo's transit data into workflows or tools using simple natural language commands.


## Available Tools (13)
- **get_forecast_by_line**: Get arrival forecast for all stops on a specific line
- **get_forecast_by_stop**: Get arrival forecast for all lines arriving at a specific stop
- **get_forecast**: Get arrival forecast for a specific stop and line
- **get_positions_by_line**: Get real-time GPS positions for buses on a specific line
- **get_positions_in_garage**: Get real-time GPS positions for buses currently in the garage
- **get_all_positions**: Get real-time GPS positions for all active buses
- **list_companies**: List bus operating companies by area
- **list_corridors**: List all intelligent bus corridors in São Paulo
- **search_lines_by_direction**: Search for bus lines filtered by direction
- **search_lines**: Search for bus lines by number or name
- **search_stops_by_corridor**: Get all stops in a specific intelligent corridor
- **search_stops_by_line**: Get all stops for a specific bus line
- **search_stops**: Search for bus stops by name or address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SPTrans Olho Vivo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for bus lines related to 'Lapa'."

**🤖 AI Agent:**
> I found several lines for 'Lapa', including line 8000-10 (Terminal Lapa) with code 33657. Would you like to see the current bus positions for this line?

---

**👤 You:**
> "What are the arrival forecasts for stop code 650005666?"

**🤖 AI Agent:**
> For stop 650005666, the next bus on line 8000-10 is expected in 5 minutes. There is also a bus for line 8615-10 arriving in 12 minutes.

---

**👤 You:**
> "Show me the real-time positions of buses on line 33657."

**🤖 AI Agent:**
> There are currently 4 buses active on line 33657. Two are near Terminal Lapa, one is on Rua Clélia, and one is approaching the city center.


## ❓ FAQ

**Q: How do I find the specific code for a bus line?**
Use the `search_lines` tool with the line number or name (e.g., '8000' or 'Lapa'). The agent will return the line code (`cl`), which is required for tracking positions or forecasts.

**Q: Can I see the arrival times for all buses at a particular stop?**
Yes! Use the `get_forecast_by_stop` tool with the stop code (`cp`). It will list all upcoming bus arrivals for that location in real-time.

**Q: Is it possible to track the live location of buses on a map?**
While the MCP returns raw coordinates, you can use `get_positions_by_line` to get the latitude and longitude of every active bus on a line, which your AI can then describe or plot.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sptrans-olho-vivo](https://vinkius.com/mcp/sptrans-olho-vivo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SPTrans Olho Vivo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sptrans-olho-vivo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SPTrans Olho Vivo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sptrans-olho-vivo": {
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
