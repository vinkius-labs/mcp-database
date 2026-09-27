# Air Quality in the Paris Region (Airparif) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/air-quality-in-the-paris-region-airparif)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environment](../categories/environment.md)

Île-de-France air quality via the official Airparif API: the daily air-index forecast per commune/intercommunality, the forecasters' bulletin, high-pollution episodes, and the Hor'Air hourly forecast, history and route modules. Free API key, X-Api-Key header.

## Description
The Île-de-France region's official air quality, from Airparif's open API (api.airparif.fr). One free API key (required) authenticates every call in the X-Api-Key header.

### What you can do
- **air_index_forecast** — the daily air-quality index forecast for communes (INSEE codes, e.g. Paris 75056, sectors 75101–75104): overall index plus per-pollutant indices as quality words (Bon..Très mauvais)
- **air_index_interco** — the same daily forecast at the intercommunality (EPCI/EPT) level by SIREN code
- **air_index_colors** — the official color legend for the quality words, for rendering
- **air_bulletin** — the forecasters' narrative bulletin for the coming days
- **air_high_pollution_episodes** — the in-progress and planned high-pollution episodes: active status, today/tomorrow status per pollutant, the official messages in English and French
- **air_hourly_history** — hourly index/concentration history at one point (latitude/longitude) over a lookback (default 72 h, max 500 h)
- **air_hourly_route** — hourly index forecast along a route (at least two "lon,lat" points) for one date
- **air_key_info** — the configured key's expiration and granted rights, for 403 diagnostics

Pollutants are one or more of: indice, no2, o3, pm10, pm25. Use air_key_info first whenever a call fails with a 403. Route forecasts are per point per hour — plan around the values, they are a forecast, not a guarantee.


## Available Tools (8)
- **air_index_colors**: Use it to render or translate the quality words returned by the forecast tools into the official color scale.

Get the official air-index color legend
- **air_key_info**: Use it first when a call fails with a 403 to tell whether the key is missing, invalid or expired, and to see which API rights the key carries.

Check the Airparif API key
- **air_bulletin**: Use it to answer "what do the forecasters expect" alongside the numeric index forecasts.

Get the Airparif forecasters' air-quality bulletin
- **air_high_pollution_episodes**: Use it to answer "is there a pollution episode / what restrictions are in place".

Get high-pollution episodes in progress and planned
- **air_hourly_history**: Use it to answer "what was the air like here yesterday". latitude/longitude are decimal degrees (Paris center is about 48.856, 2.352); date_max defaults to now and hours defaults to 72 (max 500); pollutant takes one or more of indice, no2, o3, pm10, pm25, comma-separated (indice only by default).

Get hourly air-quality history at a point
- **air_hourly_route**: Use it to answer "which route today has better air / plan a bike trip around the air quality". date is the date-time to forecast (defaults to now); points takes at least two decimal "lon,lat" pairs separated by semicolons, e.g. "2.352,48.856;2.367,48.865;2.388,48.874" (longitude first — the API expects [lon, lat] pairs); pollutant takes one or more of indice, no2, o3, pm10, pm25, comma-separated (indice only by default).

Get hourly air-quality forecast along a route
- **air_index_forecast**: Use it to answer "what is the air quality going to be in Paris / in commune X". The insee parameter takes one or more 5-digit INSEE codes, comma-separated (Paris main commune 75056; the four Paris sectors 75101–75104; Boulogne-Billancourt 92012, Clichy 92019, etc.). Pass insee to narrow the call; without it the platform returns its default scope.

Get the daily air-index forecast for communes
- **air_index_interco**: Use it for territory-level forecasts instead of commune-level. The siren parameter takes one or more 9-digit SIREN codes, comma-separated.

Get the daily air-index forecast for intercommunalities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Air Quality in the Paris Region (Airparif)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will the air quality be in central Paris tomorrow?"

**🤖 AI Agent:**
> air_index_forecast with insee: "75056" returns the daily index forecast for the Paris commune for the coming days, with the overall index and per-pollutant indices as quality words; air_index_colors translates those words into the official color scale, and air_bulletin adds the forecasters' narrative.

---

**👤 You:**
> "Is there a high-pollution episode in effect?"

**🤖 AI Agent:**
> air_high_pollution_episodes returns whether an episode is active, the status for today and tomorrow per pollutant, and the official message (English + French) — the basis for any "should I avoid cycling today" answer.

---

**👤 You:**
> "Plan a bike trip across Paris this Sunday around the air quality"

**🤖 AI Agent:**
> air_hourly_route with date set to Sunday and points as the "lon,lat" pairs of the route (at least two) returns the hourly index per point for that day; pollutant can add no2/o3/pm10/pm25 concentrations. Combine it with air_high_pollution_episodes to know whether an episode caps the options.


## ❓ FAQ

**Q: Do I need an API key, and is it free?**
Yes — one key, free: Airparif issues it for its open API. This MCP requires the AIRPARIF_API_KEY credential; every call sends it in the X-Api-Key header. Without it the calls fail with a 403 "Api Key missing" — run air_key_info to check the configured key's state.

**Q: Which pollutants can I request?**
One or more of: indice (the air quality index itself), no2, o3, pm10, pm25 — comma-separated in the pollutant parameter of the hourly tools. The default is indice only.

**Q: How do I get the INSEE / SIREN codes for a place?**
The Paris commune is INSEE 75056 and the four Paris sectors are 75101–75104; other communes keep their standard 5-digit INSEE code. Intercommunalities (EPCI/EPT) are keyed by their 9-digit SIREN code. air_index_forecast falls back to the platform's default scope when insee is omitted.

**Q: What do the 403 responses mean?**
A 403 "Api Key missing" means no credential is configured; a 403 "Invalid key" means the key is not accepted by the platform. In both cases, start from air_key_info, which returns the key's expiration timestamp and its granted rights.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/air-quality-in-the-paris-region-airparif](https://vinkius.com/en/ai-agent-connect/air-quality-in-the-paris-region-airparif)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Air Quality in the Paris Region (Airparif)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `air-quality-in-the-paris-region-airparif` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Air Quality in the Paris Region (Airparif)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "air-quality-in-the-paris-region-airparif": {
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
