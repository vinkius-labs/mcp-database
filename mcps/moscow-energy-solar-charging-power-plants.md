# Moscow Energy: Solar, Charging & Power Plants MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moscow-energy-solar-charging-power-plants)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [energy](../categories/energy.md)

Keyless Moscow energy: solar resource per month (ERA5), monthly climate averages, EV charging stations, fuel stations by grade, and the city’s power plants.

## Description
Energy in and around Moscow, keyless — how much sun the city gets, where to charge or refuel, and the cogeneration plants (ТЭЦ) that supply the city’s heat and power.

### What you can do
- **solar_resource** — how much sun Moscow gets: hourly ERA5 shortwave radiation for one month, collapsed into per-day mean and peak in W/m² plus the month total in kWh/m²
- **seasonal_averages** — monthly climate averages for any year 1940–2025 from ERA5 daily data — temperature, precipitation and snowfall
- **find_charging_stations** — EV charging stations (about 400) with socket types, output, fee and operator — filterable by operator, free charging and open now
- **find_fuel_stations** — fuel stations by brand and grade — diesel, octane 95, octane 98, LPG, CNG or electric
- **find_power_plants** — power plants in the Moscow area (about 400) — mostly the gas-fired cogeneration stations, with operator, source, output and coordinates

### Who is this for
Drivers (EV or fuel), energy planners and the solar-curious: where to charge, what a Moscow roof could produce, and how the city keeps the lights on.


## Available Tools (5)
- **find_charging_stations**: Each row carries the name, the operator (e.g. "Мосэнерго", "Россети", "Энергия+"), the mapped socket types and counts (socket:type2, socket:type2_combo, socket:chademo, socket:ccs, socket:tesla_supercharger), the output in kW when recorded, plus the fee flag and the centre coordinate. Filter by operator fragment, fee ("no" for free charging) or by proximity to a point. Coverage reflects what the map records — the real network is larger.

Find EV charging stations in Moscow
- **find_fuel_stations**: Each row carries the name, brand, operator, the fuel grades mapped (fuel:diesel, fuel:octane_95, fuel:octane_98, fuel:lpg, fuel:cng, fuel:electric), the shop and cafe flags and the centre coordinate. Filter by brand fragment, by a specific fuel grade, or by proximity to a point.

Find fuel stations in Moscow
- **find_power_plants**: Each row carries the name, the operator (e.g. "Мосэнерго"), the mapped generation source, the output in MW when recorded and the centre coordinate. Filter by source — generator:source "gas" (default-gas dominates), "coal", "oil", "solar", "wind", "hydro", "nuclear", "biomass", "waste" or "geothermal" — or by name fragment.

Find power plants in the Moscow region
- **seasonal_averages**: Year defaults to 2025 (the last complete year), any year 1940–2025. Use it for "how long is the heating season", "when does the snow arrive" and energy-demand planning.

Monthly climate averages of Moscow (ERA5)
- **solar_resource**: Defaults to July 2025 (the last complete year) — pass month 1–12 and any year from 1940 to 2025. Use it to judge a photovoltaic or solar-water setup, or to compare Moscow's sun against another city. Radiation is global horizontal (GHI) at the coordinate, which defaults to the city centre.

Solar resource of Moscow (ERA5)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moscow Energy: Solar, Charging & Power Plants** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is a solar panel worth it in Moscow?"

**🤖 AI Agent:**
> solar_resource for a summer month (e.g. month: 7) gives the per-day mean and peak W/m² and the month total in kWh/m²; compare it against a winter month for the seasonal spread.

---

**👤 You:**
> "Where can I charge my EV for free?"

**🤖 AI Agent:**
> find_charging_stations with fee: "no" lists the free mapped stations with socket types and output; add your lat/lon to sort them around you.

---

**👤 You:**
> "What powers Moscow — where are its plants?"

**🤖 AI Agent:**
> find_power_plants lists the mapped plants (about 400, mostly gas cogeneration — ТЭЦ) with operator, source and output; filter by source to separate gas, oil or renewables.


## ❓ FAQ

**Q: Do I need an API key?**
No. Every source is keyless and global: OpenStreetMap (Overpass + Nominatim), Open-Meteo and Russian Wikipedia. The MCP defines no credentials.

**Q: Is the solar data measured or modelled?**
Modelled — the ERA5 reanalysis from Copernicus, served keyless by Open-Meteo. It is global horizontal radiation at the coordinate, so a real roof also depends on tilt, orientation and shading.

**Q: Why are only about 400 charging stations listed?**
That is what OpenStreetMap records for the city. The real network is larger — treat the list as the mapped subset, not the full network.

**Q: Can I find charging or fuel near me?**
Pass lat + lon (and optionally km, 0.1–25) and the query narrows to a radius instead of the whole city. Do it before a long list — a citywide scan is capped at 200 rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moscow-energy-solar-charging-power-plants](https://vinkius.com/en/ai-agent-connect/moscow-energy-solar-charging-power-plants)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moscow Energy: Solar, Charging & Power Plants** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moscow-energy-solar-charging-power-plants` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moscow Energy: Solar, Charging & Power Plants** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moscow-energy-solar-charging-power-plants": {
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
