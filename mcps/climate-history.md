# Climate History MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/climate-history)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [weather-climate](../categories/weather-climate.md)

Daily weather history for over 130,000 stations worldwide from NOAA NCEI GHCN-Daily — temperatures, precipitation and wind for any past date, keyless.

## Description
Connect any AI agent to **measured weather history** — the daily station records NOAA's National Centers for Environmental Information has collected since the 1700s. Not a forecast, not a model: what the thermometer actually recorded, where it stood. No key required.

### What you can do

- **Find the station for any place** — over 130,000 stations worldwide, searched by name or by nearest latitude and longitude
- **Pull the daily record** — max, min and average temperature, precipitation, snowfall and wind, day by day, for any range up to ten years
- **Summarize a period** — mean and extreme temperatures, total precipitation, wet-day count, and the warmest, coldest and wettest days in one answer

### Why it matters

The record answers questions a forecast cannot: how hot the summer of 2003 was in Lisbon, how much rain fell in Mumbai last monsoon, whether last winter in Chicago was unusual. Coverage is densest in the United States but every country has stations.


## Available Tools (3)
- **find_weather_station**: Over 130,000 stations are indexed worldwide, densest in the United States. The id returned here (e.g. USW00094728) is what get_daily_weather_history and get_weather_summary take. The two-letter prefix is a country code.

Find a GHCN weather station by latitude and longitude, or by name — the first call for any historical weather question, since the other tools need a station id
- **get_daily_weather_history**: Values are GHCN-Daily station readings, not gridded reanalysis: a dash means the station did not report that element that day, and some stations report temperature but never precipitation. For a single-month or single-year overview, prefer get_weather_summary — it aggregates the same data. Station ids come from find_weather_station.

Get the day-by-day weather record for a station over a date range — daily max, min and average temperature, precipitation, snowfall and wind, converted to readable units
- **get_weather_summary**: Reads the same cached data, so the pair costs one upstream request. A station that reports no temperature or precipitation over the range is reported as such rather than guessed at.

Summarize the weather over a date range for a station — mean and extreme temperatures, total precipitation, wet-day count and the warmest, coldest and wettest days. The answer to "what was the weather like there then"


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Climate History** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the weather like in Lisbon in July 2003?"

**🤖 AI Agent:**
> The station nearest Lisbon is PO000008535 (Lisbon Geofisica). July 2003 there had a mean daily maximum of 29.4 °C and a mean minimum of 18.1 °C, with the hottest day reaching 36.2 °C on the 18th. Total precipitation was 1.8 mm across 2 wet days — a dry, hot month, consistent with the European heatwave that year.

---

**👤 You:**
> "Find the weather station for Central Park, New York."

**🤖 AI Agent:**
> The station is USW00094728 — NEW YORK CNTRL PARK TWR (US), at 40.78, -73.97 and 12.2 m elevation. It is the longest continuous record in Central Park. Pass that id with a date range to get daily temperatures and precipitation.

---

**👤 You:**
> "How much rain did Death Valley get during Hurricane Hilary in August 2023?"

**🤖 AI Agent:**
> The station is USC00042319 — DEATH VALLEY (US), and the answer is 55.9 mm on 2023-08-20, with 0.5 mm the day before. Hilary dumped roughly a year's worth of rain on the driest place in North America in a single day, and the daily record from that station shows it directly.


## ❓ FAQ

**Q: Do I need an API key?**
No. This reads NOAA's public GHCN-Daily dataset, which requires no key or account.

**Q: How far back does the data go?**
It depends on the station. The oldest records reach the 1700s; many US stations start in the late 1800s; stations elsewhere often begin in the mid-1900s. If a range returns nothing, the station simply does not cover those dates.

**Q: Is this a forecast?**
No. GHCN-Daily is the observed past — actual thermometer and rain-gauge readings. It says nothing about the future.

**Q: Why does a day show a dash for some values?**
The station did not report that element that day. Some stations measure temperature but never precipitation, and individual days are missing in every long record.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/climate-history](https://vinkius.com/en/ai-agent-connect/climate-history)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Climate History** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `climate-history` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Climate History** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "climate-history": {
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
