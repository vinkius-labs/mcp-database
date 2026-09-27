# NYC Taxi & Rideshare Trips MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-taxi-rideshare-trips)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Keyless NYC TLC trip data: yellow and green cab trips by year, FHV/ride-hail dispatch logs, taxi zone maps and monthly zone pickup counts — no API key.

## Description
Taxi and Limousine Commission trip records, keyless, for demand analysis and market research.

### What you can do
- **Yellow taxi trips** — 2023 and 2024: pickup/dropoff, times, fare, tip, distance, tolls (per-trip)
- **Green cab trips** — 2024: same per-trip fields, plus E-hail fee and trip type
- **FHV dispatch logs** — 2024–2025 ride-hail (Uber/Lyft class): pickup/dropoff zones, service request flags and dispatching base
- **Taxi zones** — the 263 official taxi zones with their borough and location id
- **Zone pickups by month** — monthly pick-up/drop-off counts per zone and industry (Yellow, Green, FHV High Volume)

### Who is this for
Mobility analysts, ride-hail market research, urban planning work and anyone validating trip-claim or demand claims with official records.

Note: per-trip history is stored year by year, so each tool asks for a trip year — pass the year you want and the tool tells you which years are available.


## Available Tools (6)
- **count_taxi_trips**: Use it to size a query before pulling rows with the search tools.

Count trips in one TLC trip dataset with filters
- **get_taxi_zone**: Zone ids are 3-4 digit numbers like "31" or "228".

Resolve one TLC zone id to its name and borough
- **list_taxi_zones**: Filter by borough to narrow it down.

List all TLC taxi zone ids with names and boroughs
- **search_fhv_trips**: Pick the year (each year is a separate dataset). pulocationid / dolocationid resolve via get_taxi_zone. sr_flag marks trips flagged as "special".

Search TLC For-Hire Vehicle (black car / rideshare) trip records
- **search_taxi_trips**: Pick the color and fiscal year; each year is a separate dataset. pulocationid / dolocationid are the TLC zone ids — resolve them with get_taxi_zone. Fare fields: fare_amount, extra, mta_tax, improvement_surcharge, congestion_surcharge, total_amount. Dates are ISO "YYYY-MM-DD".

Search TLC yellow & green taxi trip records
- **search_zone_pickups**: industry values are "Yellow Taxi", "Green Cab" or "FHV - High Volume"; pickup_dropoff is "Pick-up" or "Drop-off"; metric_month is a first-of-month ISO date. Use this for "which zone had the most pickups in a month" style questions; use the trip datasets for trip detail.

Monthly pickups per TLC zone by industry (yellow, green, FHV)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Taxi & Rideshare Trips** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which taxi zone had the most pickups last month?"

**🤖 AI Agent:**
> search_zone_pickups with month "2026-08-01" (ranked by trip_count) returns the busiest zone counts; list_taxi_zones names the zones.

---

**👤 You:**
> "How much does a Manhattan yellow taxi ride cost on average?"

**🤖 AI Agent:**
> search_taxi_trips with color "yellow" and fiscal_year "2024" returns a sample of trips with fare, tip, tolls and distance — aggregate the sample locally for an average; narrow to a zone with pulocationid.

---

**👤 You:**
> "Where do ride-hail pickups cluster around JFK?"

**🤖 AI Agent:**
> list_taxi_zones finds the JFK zone (id and borough); search_zone_pickups with that zone name over a recent month shows the FHV and yellow volume on both pick-up and drop-off.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: Why do trip tools ask for a year?**
TLC publishes trip history year by year (yellow 2023–2024, green 2024, FHV 2024–2025). Each dataset is a separate view, so every trip tool takes a year parameter and tells you the available years when the one you pass is missing.

**Q: What does the zone data cover?**
The zone table maps the city's 263 taxi zones to boroughs with stable location ids, and the monthly series gives pick-up and drop-off counts per zone and industry. Use them to rank busy taxi areas instead of fetching per-trip rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-taxi-rideshare-trips](https://vinkius.com/en/ai-agent-connect/nyc-taxi-rideshare-trips)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Taxi & Rideshare Trips** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-taxi-rideshare-trips` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Taxi & Rideshare Trips** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-taxi-rideshare-trips": {
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
