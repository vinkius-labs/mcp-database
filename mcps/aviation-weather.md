# Aviation Weather MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/aviation-weather)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [aerospace-aviation](../categories/aerospace-aviation.md)

Live aviation weather from NOAA — decoded METAR observations, TAF forecasts, SIGMET/AIRMET hazards, and pilot turbulence reports for any airport, keyless.

## Description
Connect any AI agent to **official aviation weather from the NOAA Aviation Weather Center** — the same decoded METAR and TAF products that dispatchers and pilots file against. No key required.

### What you can do

- **Check one airport** — the decoded observation (wind, visibility, cloud ceiling, flight category) plus its terminal forecast in one call
- **List observations** — METARs for stations or a bounding box, newest first, paged, with the flight category for each
- **Read forecasts** — Terminal Aerodrome Forecasts as issued, with validity windows
- **See hazards** — every SIGMET and AIRMET in force over the contiguous United States, with altitude, movement and the polygon covered
- **Hear from crews** — pilot reports of turbulence and icing actually met in flight, near an airport or inside an area
- **Find airports** — turn a place into its ICAO code, with tower status and frequencies
- **Glance at an area** — counts by flight category, the SIGMETs covering it and the turbulence pilots reported there, in one request

### Why it matters

The flight category turns raw meteorology into a decision: VFR is fine visually, MVFR is marginal, and IFR or LIFR means instrument conditions and low ceilings that hold departures and diversions. Pilot reports are the only source of in-flight turbulence — a report names the aircraft type, the flight level and an intensity like LGT-MOD or SEV. SIGMETs and AIRMETs are the hazards that re-route flights.


## Available Tools (7)
- **get_airport_weather**: g. KLAX. Use it for "what is the weather doing at the airport" and "is my flight likely to be delayed" — flight_category is VFR, MVFR, IFR or LIFR, where IFR and LIFR mean instrument conditions and low ceilings that hold departures. The TAF raw text is included as issued for pilots. Three-letter codes like LAX or ORD are IATA/FAA codes and are not resolved by the source; call find_airports with a bounding box first to get the ICAO code.

Read the current weather at one airport — the decoded METAR observation (wind, visibility, ceiling, flight category) plus its terminal forecast (TAF), from NOAA Aviation Weather Center
- **find_airports**: Coverage is the United States and its territories. Results are paged with offset and amount.

Find airports inside a bounding box — ICAO and IATA codes, name, tower status and radio frequencies, from the FAA airport database via NOAA Aviation Weather Center
- **list_terminal_forecasts**: Give station_ids (4-letter ICAO codes) or a bounding_box. The raw text is returned verbatim: groups begin with a time (FM201800 = from 20:18Z), and TEMPO marks temporary fluctuations. A station that publishes only a METAR (many untowered fields) has no TAF — an empty answer there is real. Results are paged with offset and amount.

List Terminal Aerodrome Forecasts (TAF) for stations or an area — the forecast wind, weather and cloud conditions at an airport for the next day, as issued, from NOAA Aviation Weather Center
- **list_observations**: Results are paged: defaults give 25 from offset 0 and has_more says whether to call again with a higher offset. hours is how far back to look, 1.5 by default, up to 24. Use summarize_area_conditions instead when you want the whole picture for a region in one call.

List decoded METAR weather observations for stations or an area — wind, visibility, cloud ceiling, temperature and flight category for each, newest first, from NOAA Aviation Weather Center
- **get_pilot_reports**: Give airport_id (a 4-letter ICAO code) plus distance in nautical miles (e.g. KORD with 200), or a bounding_box — not both. age is how far back, 1 hour by default. An empty answer means nobody filed anything, which usually means smooth air, not missing data.

List pilot reports (PIREPs) near an airport or inside an area — the turbulence and icing that crews actually met in flight, at a stated flight level, from NOAA Aviation Weather Center
- **list_significant_weather**: Filter with product (sigmet or airmet) and hazard (conv, turb, ice, ifr). Each entry carries the polygon it covers, its altitude band and the direction it is moving. Coverage is the contiguous US only — the source does not publish international SIGMETs. Call summarize_area_conditions to see only what covers a region.

List the SIGMETs and AIRMETs in force right now over the contiguous United States — convective, turbulence, icing and low-ceiling hazards, with altitude, movement and the raw product text
- **summarize_area_conditions**: The answer aggregates three sources in one request: the observations in the box, the SIGMETs whose polygon reaches into it, and the pilot reports filed there. It is the right first call when the question is "is it flyable around here" or "why are flights held". hours is the observation window, 3 by default. For a single airport, get_airport_weather is cheaper.

One glance at flying conditions across an area — counts by flight category (VFR/MVFR/IFR/LIFR), the SIGMETs and AIRMETs covering it, and the turbulence and icing pilots reported there


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aviation Weather** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the weather doing at Los Angeles International right now, and is it likely to hold for an arrival this evening?"

**🤖 AI Agent:**
> At KLAX the observation at 1500Z is flight category MVFR — wind 190° at 3 kt, visibility 10 statute miles, a scattered layer at 1,900 ft and an overcast ceiling at 2,400 ft, 21°C with a dewpoint of 17°C. The terminal forecast valid 1500Z today to 1800Z tomorrow holds the overcast near 2,500 ft, with winds picking up to 12 kt from 250° after 2000Z and cloud scattering. The marginal category is driven by that low ceiling rather than wind or rain, and the TAF keeps it above IFR thresholds through the evening, so an arrival this evening looks fine but the ceiling is worth re-checking closer to the time.

---

**👤 You:**
> "Is it flyable around Chicago this afternoon, or are flights being held?"

**🤖 AI Agent:**
> Summarising the box around Chicago: 42 stations reported, of which 28 are VFR, 9 MVFR, 4 IFR and 1 LIFR. The worst is IFR, concentrated along the lakeshore where the ceiling sits around 700 ft. No SIGMET or AIRMET covers the box, and the pilot reports filed in the last three hours mention only light turbulence below 6,000 ft. So visual flying is workable away from the lake, but approaches into the lakeshore airports are likely to be instrument ones, and a few arrivals could see spacing delays from that low ceiling rather than from any storm.

---

**👤 You:**
> "Are there any SIGMETs in force right now, and is the turbulence over the Rockies real?"

**🤖 AI Agent:**
> Eight convective SIGMETs are in force over the contiguous United States, the strongest of which — SIGMET 95C — covers a polygon over Colorado and Wyoming with tops to 35,000 ft, moving towards 240° at 20 kt, valid until 1555Z. Pilot reports within 200 nautical miles of Denver confirm it is being felt: 41 reports in the last hour, mostly light-to-moderate clear-air turbulence between 14,000 and 17,000 ft, with a couple of moderate rides above 20,000 ft. The convective tops are the part that re-routes jets, so flights crossing that polygon this afternoon are likely to be vectored around it.


## ❓ FAQ

**Q: Do I need an API key?**
No. This reads the public NOAA Aviation Weather Center Data API, which requires no key or account.

**Q: Why is my airport code rejected?**
The observation endpoints take the 4-letter ICAO code only — KLAX, not LAX or ORD. Call find_airports with a bounding box (south,west,north,east) around the place and read the ICAO column; "@TX" is also accepted as a station list meaning every station in Texas.

**Q: What do VFR, MVFR, IFR and LIFR mean?**
They are flight categories the source derives from ceiling and visibility: VFR is fine for visual flying, MVFR is marginal, IFR requires instrument qualification and LIFR is the worst — the conditions that hold departures and divert arrivals. summarize_area_conditions counts them across a region.

**Q: What is a pilot report and why would I trust it?**
A PIREP is what a crew actually met in flight — turbulence or icing at a stated flight level, with the aircraft type and an intensity from LGT to SEV. It is the only measurement of conditions between the ground and cruise, and it is voluntary: an empty answer usually means nobody found anything worth reporting.

**Q: Why are there no SIGMETs for my region outside the United States?**
This reads the domestic SIGMET and AIRMET products, which cover the contiguous United States. Observations themselves are global — METARs are filed for airports worldwide — but the hazard products are US-only, so summarize_area_conditions lists SIGMETs only for boxes over the US.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/aviation-weather](https://vinkius.com/en/ai-agent-connect/aviation-weather)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aviation Weather** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aviation-weather` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aviation Weather** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aviation-weather": {
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
