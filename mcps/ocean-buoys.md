# Ocean Buoys MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ocean-buoys)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [weather-climate](../categories/weather-climate.md)

Live sea state and marine weather from NOAA NDBC buoys and C-MAN stations — wind, waves, swell, water temperature and pressure at over a thousand stations worldwide.

## Description
Connect any AI agent to **live ocean observations** — the readings NOAA's National Data Buoy Center pulls straight off its buoys and coastal stations, refreshed every 10 minutes. No key required.

### What you can do

- **Ask what the sea is doing anywhere there is a buoy** — wind speed, direction and gusts, wave height, swell period and direction, sea and air temperature, and pressure, with the last few readings so the trend shows
- **Get the sea state for surf or swell questions** — significant wave height, dominant and average wave period, mean wave direction and water temperature
- **Check the wind for sailing, kite surfing or aviation** — current speed, direction and gusts plus recent readings to see whether it is building or easing
- **Find the nearest buoy to any place** — over a thousand active stations, ordered by distance from your latitude and longitude

### How it works

1. Subscribe to this server — no account, no key
2. Ask your agent: "What's the sea state outside New York Harbor?", "Find the buoy nearest Lisbon and tell me the wind", "How big are the waves at buoy 41001?"
3. The agent reads the latest observation from that station and answers in plain language

### Good to know

Not every station has every sensor — a harbour buoy may report wind but no waves, and this server says so plainly instead of inventing a number. Wave height is the significant wave height, the average of the highest third of waves; individual waves can be roughly twice as high. Times are UTC. Coverage is densest in US waters and the North Atlantic.

### Who is this for

- **Surfers, sailors and kite surfers** — "is it firing at my spot?" answered from the buoy that sits there
- **Marine and coastal operators** — real sea state for a route, a port approach or a work window
- **Weather apps and dashboards** — add live marine observations without a paid marine API
- **Anyone with a chat window** — "how warm is the water where I'm going?" answered by the instrument that measures it


## Available Tools (4)
- **get_buoy_conditions**: Station ids are short alphanumeric codes, e.g. 44065 for New York Harbor or 41001 for East Hatteras. Discover an id with list_buoy_stations. Fields shown as "?" are not reported by that station — a harbour station often has wind but no wave sensor. Times are UTC and the buoy reports every 10 minutes.

Get the latest live weather and sea observation from a NOAA NDBC buoy or C-MAN station, plus the previous few readings for trend — wind speed, direction and gusts, wave height, wave period and direction, sea and air temperature, and pressure
- **get_sea_state**: Significant wave height is the average of the highest third of waves; individual waves can be roughly twice as high.

Get the sea state at a buoy: significant wave height, dominant and average wave period, mean wave direction and water temperature. Use this for swell, surf and sea-state questions rather than wind
- **get_wind_conditions**: Direction is the direction the wind is coming from. Throws when the station has no anemometer — pick a nearby station from list_buoy_stations.

Get the current wind at a buoy: speed, direction and gusts, plus recent readings to see whether it is building or easing. Use this for sailing, kite surfing, aviation and marine-safety questions
- **list_buoy_stations**: The full list is over a thousand stations worldwide, so pass a point or a limit. Types include buoy, C-MAN, fixed and drifting.

List active NOAA NDBC buoys and C-MAN stations. Filter by station type, or pass a latitude and longitude to get the stations nearest that point, ordered by distance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ocean Buoys** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the sea state at buoy 44065? Give me the wave height, swell period and water temperature, plus the last few readings."

**🤖 AI Agent:**
> At buoy 44065 the significant wave height is 1.0 m with a dominant period near 4 s, and the sea temperature is 22.1 °C. The last few readings show the swell holding steady, with winds from the ESE around 6 m/s.

---

**👤 You:**
> "Find the buoy nearest 38.7, -9.1 and tell me the wind and waves there right now."

**🤖 AI Agent:**
> The buoy nearest 38.7, -9.1 is listed below. Right now it reports wind around 8 m/s with the sea near 18 °C and wave heights under a metre — typical for the Portuguese coast in a settled spell. Full station details and the latest reading follow.

---

**👤 You:**
> "What's the sea-surface temperature off Cape Fear right now?"

**🤖 AI Agent:**
> Buoy 41013 — Frying Pan Shoals, NC (33.436N, 77.764W) — reads 27.9 °C sea-surface temperature at 05:40 UTC on 20 Sep 2026, against an air temperature of 25.6 °C, so the water is running about 2.3 °C warmer than the air. Winds are light at 5.0 m/s from 40° with 1.1 m seas and pressure 1015.0 hPa — late-summer Gulf Stream warmth under a settled ridge.


## ❓ FAQ

**Q: Does this need an API key?**
No. All endpoints used here are NOAA's public buoy and station products. Subscribe and ask away.

**Q: My station shows no wave height. Is it broken?**
Probably not. NDBC stations report what their sensors can see, and a station in a harbour or on a river often has an anemometer but no wave rider. The response marks those fields as unavailable rather than guessing. Ask for the stations nearest your point and pick an open-ocean buoy instead.

**Q: How fresh is the data, and how far back can I look?**
Each station reports every 10 minutes and NOAA publishes the newest reading within minutes, so the latest observation is usually under 15 minutes old. This server caches each station's file for 6 minutes so it does not re-download it on every question. The files hold roughly the last 45 days of history.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ocean-buoys](https://vinkius.com/en/ai-agent-connect/ocean-buoys)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ocean Buoys** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ocean-buoys` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ocean Buoys** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ocean-buoys": {
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
