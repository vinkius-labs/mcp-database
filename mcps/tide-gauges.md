# Tide Gauges MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tide-gauges)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [weather-climate](../categories/weather-climate.md)

Live water levels and tide predictions from NOAA CO-OPS tide stations — what the sea is actually doing right now, plus the astronomic plan, highs and lows, and flood thresholds.

## Description
Connect any AI agent to **real tide gauge readings** — the water level NOAA's Center for Operational Oceanographic Products and Services measures at its tide stations, refreshed every 6 minutes. No key required.

### What you can do

- **Ask what the sea level is right now** — the latest reading at a station, in metres above the datum you choose, with the last few measurements so the trend shows
- **Get today's tide plan** — the predicted water level curve for any date, at 6-minute resolution
- **Find the highs and lows** — the turning points of the predicted curve, labelled high and low, so you know when the water turns
- **Check the reference levels** — the station's datums (MLLW, MHHW, STND) and its flood thresholds, so a "minor flooding" statement has a number behind it
- **Find a station** — by US state, or the stations nearest any latitude and longitude

### How it works

1. Subscribe to this server — no account, no key
2. Ask your agent: "What's the water level at The Battery right now?", "What are today's high and low tides at 8518750?", "Find the tide station nearest Charleston"
3. The agent reads the live gauge and the astronomic prediction and answers in plain language

### Good to know

Observed level and predicted level are different things and this server keeps them apart. The observed level includes wind setup and storm surge — the prediction is the astronomic plan. Highs and lows are derived from the predicted curve and labelled as such, because CO-OPS does not publish a high-low bulletin for most stations. Coverage is US coastal waters, including the Great Lakes, Puerto Rico and the Pacific islands.

### Who is this for

- **Boaters, anglers and kayakers** — "can I get across that flat at this hour?" answered by the gauge that sits there
- **Coastal residents and flood watchers** — the real level plus the flood threshold, not just a forecast icon
- **Marine operators and harbours** — live water level for a berth, a ramp or a work window
- **Anyone with a chat window** — "is the tide coming in or going out?" answered from measurements, not a table


## Available Tools (6)
- **find_tide_stations**: Two modes: pass a state code ("NY", "HI") to list stations there, or pass latitude and longitude to get the closest stations nationwide with distance implied by ordering. There are about 300 stations, including the Great Lakes, Alaska, Hawaii, Puerto Rico and the Pacific territories; the list is cached so repeat calls are cheap. Defaults to 20 results, max 200.

Find NOAA water level stations — by US state, or the nearest stations to a latitude/longitude
- **get_station_datums**: Needed when a source quotes a depth or clearance against a different datum than the one a water level reading uses.

Get the vertical datums for a tide station — the heights of MHHW, MLLW, MSL and the rest above station datum
- **get_flood_thresholds**: Compare the current water level from get_current_water_level against these to answer "is the harbour flooding today?". Not every station publishes thresholds; coastal ones usually do. Heights are above station datum — fetch the datums first if your reading uses MLLW.

Get the water level heights at which minor, moderate and major coastal flooding begin at a tide station
- **get_tide_highs_and_lows**: Returns each turning point with its time and height, high water marked ▲ and low water ▼. Times and heights are derived from the 6-minute prediction curve, not the official bulletin — close enough for planning a beach trip or a launch window, not for navigation. A semidiurnal station shows roughly two highs and two lows; a diurnal station shows one of each.

Get the high and low water times for a station on one date — when the tide turns and how high it reaches
- **get_tide_predictions**: Date defaults to today and is read as UTC; pass an explicit YYYY-MM-DD for any other day. For just the turn of the tide (when is high water, when is low), call get_tide_highs_and_lows instead — it derives those from this same curve. Predictions are astronomic: they do not include storm surge or wind setup. Compare against get_current_water_level to see how far off plan the sea actually is.

Get the astronomic tide prediction curve for a station on one date — the plan the sea intends to follow
- **get_current_water_level**: Station id is 6-8 digits, e.g. 8518750 for The Battery, New York. Find a station id with find_tide_stations (by state or nearest to a lat/lon). Datum defaults to MLLW — the depth most coastal users care about; use MHHW for the high-water reference or STND for the raw station datum. This is what the sea is actually doing right now, including wind setup and storm surge; for the astronomic plan use get_tide_predictions.

Get the latest observed water level at a NOAA tide station, in metres above a chosen datum


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tide Gauges** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the water level at tide station 8518750 right now? Is the tide coming in or going out?"

**🤖 AI Agent:**
> The water level at The Battery (8518750) is 0.59 m above MLLW and falling — the tide is going out. The last few readings show it dropping steadily, and low water is predicted later today, so the channel will keep shallowing until then.

---

**👤 You:**
> "Find the tide station nearest 32.78, -79.93 and give me today's high and low tides there."

**🤖 AI Agent:**
> The nearest tide station to 32.78, -79.93 is Charleston Harbor (8665530). For today it predicts high water around midday and low water in the early evening, with a range of roughly 1.5 m — the full curve and the exact turning times are in the response below.

---

**👤 You:**
> "What is the tide doing at The Battery for the rest of the day?"

**🤖 AI Agent:**
> Station 8518750 — The Battery, New York — predicts two full cycles today (times UTC, heights above MLLW): low 02:07 at 0.442 m, high 07:55 at 1.154 m, low 14:07 at 0.522 m, and the day's highest high at 20:13 at 1.386 m. The afternoon flood is the bigger of the two, so expect the strongest current in the hours before 20:13.


## ❓ FAQ

**Q: Does this need an API key?**
No. All endpoints used here are NOAA CO-OPS public products. Subscribe and ask away.

**Q: Why is the observed water level different from the prediction?**
The prediction is the astronomic tide — where the water should be from the pull of the moon and sun. The observed level is what the gauge actually measures, and it also carries wind setup, storm surge and changes in air pressure. During a storm the two can be a metre apart, and that gap is exactly what a surge warning looks like.

**Q: Where do the high and low tide times come from?**
They are derived from the predicted water-level curve for the day, by finding where the curve turns. NOAA does not publish a high-low bulletin for most stations, so this is computed rather than transcribed — the response says so. The times are close to the official values but are not themselves an official product.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tide-gauges](https://vinkius.com/en/ai-agent-connect/tide-gauges)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tide Gauges** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tide-gauges` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tide Gauges** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tide-gauges": {
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
