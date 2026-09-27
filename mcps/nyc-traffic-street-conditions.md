# NYC Traffic & Street Conditions MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-traffic-street-conditions)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless NYC street data: DOT motor-vehicle crashes with per-person injuries, pothole work orders, bike & pedestrian sensor counts, sensors and the city's bike route network — no API key.

## Description
Street-surface reality from the Department of Transportation's open datasets, keyless.

### What you can do
- **Search crashes** — DOT motor-vehicle crash reports: date, borough, street, injuries/kills and the primary contributing factor
- **Crash person detail** — every recorded person in one collision: type, injury severity, age, safety equipment
- **Pothole work orders** — closed DOT pothole work orders by street or letter code, plus one order's full segments
- **Bike/ped counts** — interval volumes from the city's sensor network, by sensor and travel mode
- **Sensor detail** — location, coverage and data range of one count sensor
- **Bike routes** — segments of the protected/signed bike network with facility class
- **Top crash factors** — most frequent primary contributing factors in a trailing window

### Who is this for
Urban planning, mobility analysis, road-maintenance tracking and newsroom data journalism on street safety.


## Available Tools (8)
- **get_bike_ped_sensor**: Use the sensor_id from search_bike_ped_counts.

Details of one bike/ped count sensor (location, coverage, data range)
- **get_crash_injuries**: Give the collision_id from search_traffic_crashes. Person counts per crash are small, so results are complete.

All persons (injuries) recorded in one crash, by collision id
- **get_pothole_work_order**: A work order can span multiple street segments, so several rows may come back.

One pothole work order (all segments) by its defnum
- **list_bike_routes**: ). Filter by boro, exact street or facility class.

City protected/signed bike route segments with facility class
- **search_bike_ped_counts**: sensor_id identifies the sensor (look it up with get_bike_ped_sensor); travelmode is "Bike" or "Pedestrian". timestamps are ISO; counts is the interval volume for that direction/flow.

Hourly/interval bike & pedestrian counts from NYC sensor network
- **search_pothole_work_orders**: boro is a single-letter code, not a name. defnum is the work-order number (starts with "DB").

Search closed DOT pothole work orders (street conditions)
- **search_traffic_crashes**: Filter by borough, zip_code or a crash_date window ("YYYY-MM-DD"). For the per-person detail of one crash, use get_crash_injuries with the collision_id.

Search NYC motor vehicle crashes (DOT) with injury counts
- **top_crash_factors**: Widen or narrow with days. Counts cover all of the city; use search_traffic_crashes to drill into one borough or street.

Most frequent primary contributing factors in crashes over a window


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Traffic & Street Conditions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Most crash-prone areas in the last year"

**🤖 AI Agent:**
> top_crash_factors with days=365 returns the leading contributing factors citywide; search_traffic_crashes with a borough filter then narrows to streets.

---

**👤 You:**
> "How busy is the bike lane on 6th Ave, Midtown?"

**🤖 AI Agent:**
> search_bike_ped_counts with travelmode "Bike" and a sensor id covering that stretch (find it via the sensor dataset) returns interval volumes; list_bike_routes shows which segments carry protected lanes.

---

**👤 You:**
> "When was the pothole on 14th St fixed?"

**🤖 AI Agent:**
> get_pothole_work_order with the work-order defnum returns every segment with rptdate and rptclosed — the close date shows when it was fixed.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: How current is the data?**
Each dataset is updated on its own cadence (311 daily, trip records yearly, tonnage monthly, ...). The get tools and search_datasets expose the last update timestamp, and the rows you read are the platform's current state.

**Q: What do the crash injury numbers mean?**
Each crash row carries the counts of persons/pedestrians/cyclists/motorists injured and killed, plus the recorded contributing factors for up to five vehicles. The per-person detail (severity, age, equipment) is a separate dataset, joined by collision_id.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-traffic-street-conditions](https://vinkius.com/en/ai-agent-connect/nyc-traffic-street-conditions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Traffic & Street Conditions** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-traffic-street-conditions` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Traffic & Street Conditions** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-traffic-street-conditions": {
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
