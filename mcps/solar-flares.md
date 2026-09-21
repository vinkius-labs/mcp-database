# Solar Flares MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/solar-flares)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [weather-climate](../categories/weather-climate.md)

Live solar X-ray flux, detected solar flares and GOES magnetometer conditions from NOAA SWPC — the A/B/C/M/X class of the Sun right now, keyless.

## Description
Connect any AI agent to **live solar activity** — the measurements NOAA's GOES satellites beam down every minute, published by the Space Weather Prediction Center. No key required.

### What you can do

- **Ask what the Sun is doing right now** — the current X-ray class (A, B, C, M or X), the peak over the last hour and whether the flux is climbing
- **List detected solar flares** — begin time, peak class and end time for each event SWPC has identified, with a minimum-class filter so you see only M and X events when they matter
- **Pull the X-ray flux curve** — from the last 10 minutes up to seven days, already converted to NOAA classes, sampled to stay small
- **Check the geomagnetic field at the satellite** — the Hp component, its one-hour swing and a quiet/active/storm label, an early warning that a storm is arriving
- **Get a one-look briefing** — current class, biggest recent flare and geomagnetic state in a single answer

### Why it matters

X-class flares can trigger planet-wide radio blackouts; M-class flares disrupt high-frequency radio at the poles. Satellite operators, airlines, grid managers and aurora hunters all watch the same feed.


## Available Tools (5)
- **get_solar_flare_status**: 1–0.8 nm channel, its NOAA class (e.g. "C3.4") and whether the flux is rising or falling. X-class means a major flare; M-class is moderate. Readings flagged for electron contamination are provisional. For the full curve use list_xray_flux_history; for detected events use list_solar_flares.

Get the current solar X-ray class right now — A, B, C, M or X — from the NOAA GOES satellite, plus the peak and the trend over the last hour. This is the "is the Sun active?" headline tool
- **list_xray_flux_history**: Up to 360 minutes reads the 6-hour feed at full one-minute cadence; longer requests read the 7-day feed and sample it down to at most 120 points so the response stays small. Points are oldest-first so the curve reads left to right. Each point carries its NOAA class already computed, so no flux math is needed downstream.

Get the recent solar X-ray flux curve as class-tagged samples — the input to any "how is solar activity evolving" or "when did that flare peak" question
- **get_geomagnetic_conditions**: The level label is derived from the one-hour Hp swing: storm >= 40 nT, active >= 20, unsettled >= 8, otherwise quiet. Readings with the arcjet flag set are contaminated by a station-keeping burn. For aurora probability, pair this with a planetary K-index source.

Get the live GOES magnetometer reading — the Hp component, its swing over the last hour, and a quiet/active/storm label. Use this for "is a geomagnetic storm arriving"
- **get_space_weather_summary**: Follow up with list_solar_flares for event detail or list_xray_flux_history for the curve. If the geomagnetic part is absent the magnetometer feed was momentarily unavailable, not silently dropped.

One-look space weather briefing: current X-ray class, the biggest recent flare, and the geomagnetic state — the right first call for any solar-storm question
- **list_solar_flares**: An event with no end time is still in progress, and an event whose peak is pending shows no class yet — SWPC writes "Unk" for its max_time. Use min_class "M" or "X" when the question is about flares that matter for Earth; C-class events are common and mostly harmless. When nothing clears the minimum, the unfiltered list is returned with a note rather than an error.

List solar flare events detected by NOAA SWPC — begin time, peak class and end time for each, newest first. Pass min_class to see only significant flares


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Solar Flares** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the Sun active right now?"

**🤖 AI Agent:**
> The current solar X-ray class is B3.1 — quiet background activity. The peak over the last hour was C1.2 and the trend is steady across 60 one-minute samples, so no flare is building at the moment. Nothing here would affect radio or satellites.

---

**👤 You:**
> "Were there any big solar flares recently?"

**🤖 AI Agent:**
> The strongest event in the current detection window was an M3.3 flare — it began as B2.9 at 17:57 UTC, peaked at 18:17 UTC and ended as C1.7 at 18:32 UTC. Three C-class or stronger events were detected in total. M-class flares can cause brief high-frequency radio blackouts at the poles but this one is not storm-driving.

---

**👤 You:**
> "Skip the B-class background — show me only the M-class and X-class flares from the latest batch."

**🤖 AI Agent:**
> The current batch on GOES-18 holds a single event: it began at 05:02 UTC on 20 Sep 2026 as B8.8, peaked at B9.3 at 05:06 UTC and closed as B9.0 at 05:08 UTC. Nothing reached the M-class bar, so the filter relaxes and returns that event with a note — a flare that is still building often carries no peak class at all, and an empty answer would hide it. Only M-class and above matters for radio blackouts; B-class is background.


## ❓ FAQ

**Q: Do I need an API key?**
No. This reads NOAA's public Space Weather Prediction Center feeds, which require no key or account.

**Q: What is an X-class flare?**
The classes A, B, C, M and X each mark a range of X-ray flux, and each letter is ten times the previous one. X is the strongest: a major flare that can trigger planet-wide radio blackouts. M-class is moderate; C-class is minor and common.

**Q: How fresh is the data?**
The X-ray and magnetometer feeds publish a new sample every minute. Results are cached for one minute per call.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/solar-flares](https://vinkius.com/en/ai-agent-connect/solar-flares)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Solar Flares** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `solar-flares` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Solar Flares** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "solar-flares": {
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
