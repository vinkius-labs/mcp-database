# Aurora Forecast MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/aurora-forecast)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [weather-climate](../categories/weather-climate.md)

Live aurora and space weather from NOAA SWPC — Kp index, storm scales, solar wind, and the OVATION model's aurora probability at any location.

## Description
Connect any AI agent to **live space weather** — the same data NOAA's Space Weather Prediction Center uses to issue its own aurora alerts. No key required.

### What you can do

- **Ask "can I see the aurora tonight?"** — give it your latitude and longitude and get the current Kp index, the NOAA storm level, the solar wind, and the OVATION model's aurora probability directly overhead your spot, with a plain-language verdict
- **Watch the Kp index** — the last week of 3-hourly measurements, plus the 3-day forecast, with the peak of the window highlighted so you know when to go out
- **Read NOAA's storm scales** — the R/S/G scales for today and the next 3 days, with NOAA's own probability percentages
- **Check issued alerts** — warnings, watches and alerts as NOAA issued them, filterable by type
- **Read the solar wind** — speed, magnetic field Bt and Bz, and the F10.7 radio flux; a sustained southward Bz is what opens the door to aurora

### How it works

1. Subscribe to this server — no account, no key
2. Ask your agent: "Can I see the aurora from Reykjavik tonight?", "What's the Kp forecast for the next 3 days?", "Has NOAA issued a geomagnetic warning?"
3. The agent answers from live measurements — refreshed every few minutes for the Kp index and solar wind, roughly every 10 minutes for the aurora model

### Good to know

Aurora needs three things: high geomagnetic activity, a dark sky, and clear weather. This server reports the first one — the other two are still on you. A probability of 50 or more means the aurora is likely overhead, not that it will be visible through clouds.

### Who is this for

- **Aurora chasers and photographers** — stop refreshing three different dashboards; ask one question and get the verdict for your exact spot
- **Tour operators in high latitudes** — build "is tonight a good night?" into your customer comms
- **Ham radio operators and auroral-effect watchers** — the R/S/G scales and solar wind numbers without the NOAA website
- **Anyone with a chat window** — "is the northern hemisphere lit up right now?" answered from real measurements, not a vibes guess


## Available Tools (7)
- **list_space_weather_alerts**: Filter with product_id — a prefix match, case-insensitive: "K04" for Kp-4 warnings, "K05" for Kp-5, "A20" for the 20cm radio burst watch, and so on. Without a filter you get the most recent 10 of everything. Useful for "has a storm warning been issued?" — pair with list_kp_forecast for timing.

List space weather alerts, watches and warnings issued by NOAA SWPC, most recent first
- **get_aurora_conditions**: Returns the latest 3-hourly planetary Kp index, its NOAA G-scale level, the geomagnetic latitude down to which aurora is typically visible, today's R/S/G storm scales, and the live solar wind. Pass latitude and longitude to add a point forecast: the OVATION model's aurora probability directly overhead that spot, plus the strongest value within 2 degrees of it. A probability of 50 or more means aurora is likely overhead; under 25 means it is not worth travelling for. This is a nowcast of the sky, not a weather forecast — a high probability still needs clear, dark skies.

Report current aurora and geomagnetic conditions: live Kp index, NOAA storm scale, solar wind, and aurora chance at a location
- **list_kp_forecast**: By default returns the most recent 32 values; the window covers roughly 7 days back and 3 days forward. The peak row in the returned window is highlighted — that is the best moment to plan an aurora watch around. Predicted Kp is a model output and shifts as new observations arrive, so re-check shortly before going out.

List the observed and predicted Kp index — about a week of history plus 3 days of forecast, 3-hourly
- **list_recent_kp_index**: By default returns the most recent 8 values (24 hours); raise limit for a longer history. Kp 4 means active conditions, 5 starts the G1 minor storm scale, 9 is extreme. For what is coming next rather than what already happened, use list_kp_forecast.

List recent planetary Kp index values — the last week of 3-hourly measurements, latest last
- **get_aurora_probability**: The model grid is 1 degree resolution, so the neighbourhood value catches arcs that fall between cells. Use get_aurora_conditions instead when you also want the Kp index and storm scales; this tool is for checking many points cheaply. The value refreshes roughly every 10 minutes.

Get the OVATION model's aurora probability at one exact latitude/longitude, right now
- **get_storm_scales**: Each runs 1 (minor) to 5 (extreme). This returns the current scale for today plus the 3 forecast days, including NOAA's own percentage chances for minor and major events. The G scale is the one that matters for aurora: G1 reaches 60 degrees geomagnetic latitude, G5 can reach 40.

Get NOAA space weather scales (R/S/G) for today and the next 3 days, with probabilities for each level
- **get_solar_wind**: 7 cm radio flux in solar flux units. Bz matters most for aurora — sustained negative (southward) Bz lets solar wind energy into the magnetosphere and drives the storms that push aurora equatorward. Values are point-in-time measurements refreshed every few minutes.

Get the latest solar wind speed, magnetic field strength and F10.7 radio flux from NOAA


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aurora Forecast** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can I see the aurora from 64.8, -147.7 tonight? Give me the current conditions and the Kp forecast for the next 24 hours."

**🤖 AI Agent:**
> Right now the Kp index is 1.7, which NOAA rates as quiet — the aurora oval sits near 70° latitude, so from 64.8, -147.7 the OVATION model gives a low probability overhead. No geomagnetic warning is in effect. Over the next 24 hours the forecast peaks around Kp 3, so conditions may improve slightly after dark.

---

**👤 You:**
> "Has NOAA issued any geomagnetic storm warnings recently? List the latest alerts and today's NOAA space weather scales."

**🤖 AI Agent:**
> No geomagnetic warnings are in effect right now. Today’s NOAA scales put the G1 (minor storm) probability at a few percent over the next 24 hours, with radio blackout R1 and solar radiation S1 probabilities also low. The most recent issued alert is listed below; nothing in it rises to warning level for high latitudes.

---

**👤 You:**
> "What is the solar wind doing right now? Is a fast stream arriving?"

**🤖 AI Agent:**
> At 06:09 UTC on 20 Sep 2026 the solar wind is slow and quiet — 408 km/s proton speed with a total field of 5 nT and Bz at −3 nT (GSM). A stream that would drive aurora typically needs 500 km/s or more and a sustained southward Bz, so nothing is arriving. The F10.7 radio flux, a proxy for how much EUV the Sun is feeding the upper atmosphere, was 97 solar flux units at 20:00 UTC yesterday.


## ❓ FAQ

**Q: Does this need an API key?**
No. All endpoints used here are NOAA's public space weather products. Subscribe and ask away.

**Q: The aurora probability at my location is high but I see nothing. Why?**
The probability comes from NOAA's OVATION model, which reports what the upper atmosphere is doing. It cannot see your clouds or your midnight sun. You still need a dark, clear sky — and aurora near the equator edge of the oval is often faint, low on the horizon, and best photographed with a long exposure rather than judged by eye.

**Q: How often does the data refresh?**
The Kp index and solar wind summaries refresh every few minutes. The OVATION aurora model refreshes roughly every 10 minutes, and this server caches the ~1 MB grid for that long so it does not re-download it on every question.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/aurora-forecast](https://vinkius.com/en/ai-agent-connect/aurora-forecast)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aurora Forecast** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aurora-forecast` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aurora Forecast** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aurora-forecast": {
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
