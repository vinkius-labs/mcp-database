# FAA (Federal Aviation Administration) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/faa-federal-aviation-administration)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access real-time aviation data directly from the FAA — including NOTAMs, TFRs, UAS facility maps, and METAR/TAF weather reports.

## Description
Connect your AI agent to the **Federal Aviation Administration (FAA)** data services to retrieve critical flight safety and weather information through natural language.

### What you can do

- **NOTAM Search** — Retrieve Notice to Air Missions (NOTAMs) by location, number, or date to stay informed about airport conditions and hazards.
- **Flight Restrictions** — List active Temporary Flight Restrictions (TFRs) by state or type to ensure compliance with airspace regulations.
- **UAS & Drone Safety** — Access UAS Facility Maps (LAANC) to identify permitted drone operation areas based on geographic coordinates.
- **Aviation Weather** — Fetch real-time Meteorological Aerodrome Reports (METAR) and Terminal Aerodrome Forecasts (TAF) for specific stations.

### How it works

1. Subscribe to this server
2. Enter your FAA API Key
3. Query aviation safety and weather data directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Pilots & Dispatchers** — Quickly check NOTAMs and weather forecasts during pre-flight planning without leaving your workflow.
- **Drone Operators** — Verify LAANC facility maps and local flight restrictions before takeoff.
- **Aviation Developers** — Integrate official FAA data into your agentic workflows for safety analysis and reporting.


## Available Tools
- **get_metar**: Get METAR (Meteorological Aerodrome Reports)
- **get_taf**: Get TAF (Terminal Aerodrome Forecasts)
- **list_tfrs**: List Active Temporary Flight Restrictions (TFRs)
- **list_uas_facilities**: Get UAS Facility Maps (LAANC)
- **search_notams**: Search Notice to Air Missions (NOTAMs)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FAA (Federal Aviation Administration)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for active NOTAMs at KJFK airport."

**🤖 AI Agent:**
> I've retrieved the NOTAMs for KJFK. There are currently 3 active notices, including a runway closure on 4L/22R and taxiway lighting maintenance. Would you like the full details for any of these?

---

**👤 You:**
> "Are there any active TFRs in Florida right now?"

**🤖 AI Agent:**
> Checking active TFRs for Florida (FL)... I found one Security TFR near Cape Canaveral effective until 22:00 UTC. No other major restrictions are listed for the state at this time.

---

**👤 You:**
> "Get the latest METAR and TAF for KORD."

**🤖 AI Agent:**
> For KORD (Chicago O'Hare): The latest METAR shows winds at 10kts, visibility 10SM, and clear skies. The TAF forecast predicts increasing cloud cover and a chance of light rain starting after 18:00Z.


## ❓ FAQ

**Q: How can I check for Temporary Flight Restrictions (TFRs) in a specific state?**
You can use the `list_tfrs` tool and provide the two-letter state code (e.g., 'CA' for California). The agent will return a list of all active restrictions and their types.

**Q: Can I get both current weather and forecasts for an airport?**
Yes. Use `get_metar` for real-time reports and `get_taf` for terminal forecasts by providing the ICAO station code (e.g., 'KJFK').

**Q: Does this tool help with drone flight planning?**
Absolutely. The `list_uas_facilities` tool provides geographic data for UAS facility maps (LAANC), showing where drone operations are permitted based on your coordinates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/faa-federal-aviation-administration](https://vinkius.com/mcp/faa-federal-aviation-administration)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FAA (Federal Aviation Administration)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `faa-federal-aviation-administration` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FAA (Federal Aviation Administration)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "faa-federal-aviation-administration": {
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
