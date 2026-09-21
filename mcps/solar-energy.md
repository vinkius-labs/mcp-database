# Solar Energy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/solar-energy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [energy-utilities](../categories/energy-utilities.md)

How much electricity solar panels would generate at any location on Earth — yearly and monthly yield, the optimal tilt and orientation, hourly output profiles and the typical climate year, from the European Commission JRC PVGIS database. Keyless.

## Description
Connect any AI agent to **PVGIS**, the Photovoltaic Geographical Information System maintained by the European Commission's Joint Research Centre. It is the reference dataset behind national solar calculators across Europe and covers the whole planet from satellite and reanalysis weather records. No key required.

### What you can do

- **Estimate the yield** — monthly and yearly kilowatt-hours for any site, at any system size, with the sunlight that reaches the plane of the modules and the year-to-year variability
- **Find the ideal mounting** — the optimal tilt and orientation PVGIS computes for the latitude, and what that ideal orientation would generate
- **Compare mountings side by side** — several tilts and orientations in one call, sorted by yearly yield, to weigh an existing roof against a purpose-built frame
- **See when power actually arrives** — the mean output for each hour of a chosen month, for battery sizing and self-consumption
- **Read the climate itself** — the typical meteorological year, independent of any panel system: monthly temperature, humidity, sunshine split into direct and diffuse, wind and pressure

### Why it matters

A yield figure only means something next to the assumptions behind it. Every answer reports the tilt, orientation, system losses, radiation database and year window PVGIS actually used, so a number can be quoted with its basis attached. The monthly spread matters as much as the total: a site that delivers two thirds of its energy in summer needs different storage and tariff thinking than one with an even profile.

The figures are long-term averages from the weather record, typically 2005–2023, not a forecast for the coming year, and they model a fixed free-standing array — PVGIS does not support tracking systems in this API.


## Available Tools (5)
- **compare_configurations**: Give configurations as a comma-separated list of label:slope or label:slope:azimuth — for example "Flat:0,South-35:35:0,Roof:20:-30,Optimal" — where azimuth is degrees from south (0 south, -90 east, 90 west) and a bare label like Optimal asks PVGIS to choose the best angle. The answer sorts by kWh per year and shows how far each option trails the best. Useful for weighing yield against installation cost: a roof a few percent off ideal often beats the price of a frame.

Compare several panel tilts and orientations side by side, sorted by yield — how much each mounting option would generate per year, in one call
- **estimate_pv_generation**: Give latitude and longitude in decimal degrees; peak_power_kw defaults to 1 kWp so a question about the site needs no system size, and the answer scales linearly — 10 kWp is ten times the figures. Leave slope out to have PVGIS choose the optimal tilt and orientation, and the answer reports which angles it picked. slope is degrees from horizontal (0 flat, 90 vertical) and azimuth is degrees from south — 0 south, -90 east, 90 west; a compass letter like W also works. system_loss_pct defaults to 14, typical for a grid-connected system. radiation_database is PVGIS-ERA5 (global, the default) or PVGIS-SARAH3 (Europe, Africa, Asia). Errors carry PVGIS's own reason, which lists the valid values when one is wrong.

Estimate how much electricity a solar panel system would generate at any location on Earth — monthly and yearly kilowatt-hours, plus the sunlight available, from the European Commission JRC PVGIS database
- **find_optimal_tilt**: Returns the optimal slope in degrees from horizontal and the azimuth in degrees from south, together with the yearly and monthly yield that orientation gives. A shallow tilt favours summer, a steeper one winter — compare_configurations shows that trade-off across several angles. Only fixed free-standing mountings are modelled; this version of PVGIS does not support tracking systems.

The best tilt and orientation for solar panels at a location, and how much electricity that ideal mounting would generate
- **get_monthly_profile**: PVGIS serves 8760 hourly records per year; this aggregates them into one average day for the month asked about, so the response stays small. month is 1–12 and year defaults to the most recent year PVGIS holds. The shape of the day matters more than the peak for storage: read how many hours carry power and how much lands midday versus evening.

When in the day a solar system would actually deliver power — the mean output for each hour of a chosen month, plus the month's total, from the PVGIS hourly series
- **get_typical_meteorological_year**: Returns monthly means plus the yearly total of horizontal sunshine, split into direct and diffuse — a site with a high diffuse share is cloudier and favours different modules than a direct-beam site. A typical year is twelve representative real months, not a forecast of the coming season; it is the right input for sizing, not for predicting.

The typical meteorological year for a location — monthly temperature, humidity, sunshine, wind and pressure, built from the long-term climate record by PVGIS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Solar Energy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My roof in Lisbon has a 25-degree pitch facing southeast. What would a 6 kWp solar system generate there, and is it worth re-tilting the panels?"

**🤖 AI Agent:**
> A 6 kWp system on a 25-degree southeast-facing roof in Lisbon would generate about 9,650 kWh a year — roughly 560 kWh in January and 1,070 kWh in July, from PVGIS weather data covering 2005–2023. PVGIS computes the ideal mounting for that latitude at a 35-degree tilt facing almost due south, which would give about 10,060 kWh a year. So the existing roof is already within about 4% of the maximum: re-tilting would buy roughly 400 kWh a year, and at typical Portuguese prices that is well below the cost of a mounting frame and the downtime to install it. The roof as built is the better choice; the money is better spent on an extra panel than on changing the angle.

---

**👤 You:**
> "I'm sizing a battery for a cabin near Milan. When in the day does a 5 kWp array actually deliver power in January?"

**🤖 AI Agent:**
> In January, a 5 kWp array near Milan on the optimal tilt produces about 350 kWh over the month, and the hourly profile shows power arriving between roughly 8am and 5pm with a midday peak near 1,900 W — about 460 hours of the month carry non-zero output, and only about a third of the daylight hours are near-clear by the site's own monthly standard. So the array delivers almost nothing before 8am or after 5pm, and the midday surplus is what a battery has to absorb. To cover a winter evening's load you need roughly a day's worth of January consumption in storage, because a heavily overcast January day can cut that midday peak by more than half. July at the same site runs about 680 kWh with a midday peak near 2,800 W and twice the clear share — so the battery sized for January is comfortably large in summer.

---

**👤 You:**
> "We're scoping a small solar farm outside Cape Town. Compare a flat mounting against a 30-degree south-facing frame there."

**🤖 AI Agent:**
> For Cape Town, call the tool with the site coordinates and the two configurations in one compare request — for example "Flat:0" and "Frame:30:0" — and it returns both yearly totals sorted by yield, each with the tilt and orientation PVGIS actually applied. In the southern hemisphere the same tool is used, but the orientation that faces the midday sun is azimuth 180 rather than 0: a 30-degree frame there should be given as "Frame:30:180", because azimuth is measured from south and 180 points the array north. Read the gap between the two yearly figures as the value of the frame: if flat mounts trail by only a few percent, the saving on mounting structures may be worth the small loss; a double-digit gap means the frame pays for the site's latitude.


## ❓ FAQ

**Q: Do I need an API key?**
No. PVGIS is a free public service of the European Commission Joint Research Centre and answers plain requests with no key, account or registration.

**Q: Which locations are covered?**
Everywhere on Earth. The default database, PVGIS-ERA5, is global. PVGIS-SARAH3 is offered as an alternative and is built from satellite observations over Europe, Africa and Asia; requesting it for the Americas is rejected by PVGIS itself, which names the valid values in the error message.

**Q: Are these predictions for the coming year?**
No, and this distinction matters. PVGIS reports the long-term average from its weather record — typically 2005 to 2023 — so the yearly figure is what a system of that size at that orientation should produce in an average year, and the variability field shows how much real years scatter around it. Next year will be sunnier or cloudier than that; the typical-meteorological-year tool exists for exactly this reason, to describe the climate rather than forecast a season.

**Q: Can it model solar tracking systems or concentrate the analysis on one module technology?**
Not in this API. The tools model a fixed free-standing array with a stated tilt and orientation; PVGIS accepts a tracking parameter in this version but ignores it, so no tracking option is exposed rather than return a silently wrong figure. Module technology is likewise treated as crystalline silicon, which is what the standard loss assumptions assume.

**Q: Why does the monthly profile say a month is only partly clear when the sun shone all week?**
The clear-sky share is derived from the irradiance the site itself received, hour by hour, compared against the clearest that hour reached anywhere in the month — PVGIS's own clear-sky flag exists in the raw data but reads zero for every hour in this version, so it cannot be trusted. The threshold counts an hour as near-clear at 70% of that hour's monthly best. It describes how sunny the month was relative to its own ceiling, not an absolute sky condition, and it is a supporting detail next to the kilowatt-hour totals rather than a measurement in its own right.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/solar-energy](https://vinkius.com/en/ai-agent-connect/solar-energy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Solar Energy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `solar-energy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Solar Energy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "solar-energy": {
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
