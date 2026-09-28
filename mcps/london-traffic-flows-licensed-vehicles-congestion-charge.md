# London Traffic: Flows, Licensed Vehicles & Congestion Charge MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/london-traffic-flows-licensed-vehicles-congestion-charge)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless London traffic data: borough vehicle flows on the road network 1993-2025 (cars or all vehicles), licensed vehicles per borough 2019-2022, and the congestion-charge zone's monthly camera captures and confirmed vehicles since July 2010.

## Description
Three official London transport datasets — keyless, straight from the London open-data platform (data.london.gov.uk).

### What you can do
- **traffic_flows / traffic_flow_lookup / traffic_flows_ranking** — annual vehicle flows on each borough's major roads, 1993 to 2025: cars only or all vehicles, with a merged 33-year series for one local authority and the ranking of authorities on a given year
- **licensed_vehicles / licensed_vehicle_lookup** — vehicles licensed to each borough for 2019, 2020, 2021 and 2022: company and private plate groups (PLG), the PLG total, and the disabled-exempt splits; one authority's four-year side by side
- **congestion_charge_monthly / congestion_charge_overview** — the congestion-charge zone month by month: camera captures, confirmed vehicles and charging days, plus per charging-year totals with the busiest month
- **traffic_overview** — the city-wide aggregate in one call: the 2025 London flows, the 2022 London licensed-vehicle counts and the most recent congestion-charge month

### Who is this for
Transport planners, mobility journalists and anyone benchmarking how a borough's traffic, fleet and central-London charge have moved. The flow table's rows are the 33 London boroughs plus a London aggregate and a Great Britain row; the charge zone's months run from Jul-10 on, where July-to-December belongs to the charging year that started in July of the previous calendar year.


## Available Tools (8)
- **congestion_charge_monthly**: Month labels look like "Jul-10". Optional month filter (case-insensitive) plus limit/offset paging.

Monthly TfL congestion-charge enforcement activity
- **congestion_charge_overview**: ), plus the month with the most confirmed vehicles. Charging years run from 2010/11 to 2025/26.

Congestion-charge enforcement totals per charging year
- **licensed_vehicle_lookup**: la is required, matched case-insensitively.

DVLA licensed-vehicle counts for one local authority
- **licensed_vehicles**: year is required (2019-2022); la is an optional exact, case-insensitive match. Page with limit/offset.

Vehicles licensed per London local authority (2019-2022)
- **traffic_flow_lookup**: la is required, matched case-insensitively.

Full 1993-2025 traffic-flow series for one local authority
- **traffic_flows**: Rows include the 33 London LAs plus aggregate rows (London, England, regions, Great Britain). The year parameter is a calendar year (1993-2025, default 2025); la is an exact, case-insensitive match on the authority name. Page with limit/offset.

Average daily road-traffic flows per London local authority
- **traffic_flows_ranking**: Aggregate rows (London, England, regions, Great Britain) are included in the ranking so they can be filtered out when needed. Optional top-N (max 45).

Rank local authorities by average daily traffic flow in one year
- **traffic_overview**: Useful as a starting point before drilling into the individual tools.

Headline numbers across the London traffic datasets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **London Traffic: Flows, Licensed Vehicles & Congestion Charge** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many cars pass Westminster's major roads in 2025?"

**🤖 AI Agent:**
> Call traffic_flow_lookup with la "Westminster" — the merged 33-year series comes back with cars and all-vehicles side by side; the last row is 2025.

---

**👤 You:**
> "Which boroughs have the most vehicles on the road?"

**🤖 AI Agent:**
> Run traffic_flows_ranking for the latest year — the top rows are the busiest authorities; add vehicle_type "all_vehicles" to include buses and HGVs.

---

**👤 You:**
> "How many vehicles were confirmed in the congestion zone in 2024?"

**🤖 AI Agent:**
> Run congestion_charge_overview — the per charging-year block gives the confirmed-vehicles total; Jul-24 through Jun-25 is the 2024/25 charging year.


## ❓ FAQ

**Q: Do I need an API key?**
No. data.london.gov.uk publishes every dataset as an anonymous file download (CSV or Excel). This MCP defines no credentials and needs nothing configured.

**Q: "Cars" vs "all vehicles" — what is the difference?**
The flow table has two cuts of the same counts: the cars-only series and the all-vehicles series (cars plus buses, HGVs and everything else). Pick the vehicle_type that matches your question; the ranking and lookup tools honour the same choice.

**Q: What is a "charging year"?**
The congestion charge runs Jul 2010 through Jul 2026 in the dataset. A charging year bundles one July to the next June: Jul-10 to Jun-11 is the 2010/11 charging year, and so on. congestion_charge_overview groups the monthly rows by that label and reports the busiest month of each.

**Q: Where do the vehicle-flow counts come from?**
Annual road counts on each borough's major roads, published by the city, 1993 through 2025. The table rows are the 33 boroughs, a London aggregate and a Great Britain row; trailing empty rows in the source file are dropped by the tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/london-traffic-flows-licensed-vehicles-congestion-charge](https://vinkius.com/en/ai-agent-connect/london-traffic-flows-licensed-vehicles-congestion-charge)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **London Traffic: Flows, Licensed Vehicles & Congestion Charge** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `london-traffic-flows-licensed-vehicles-congestion-charge` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **London Traffic: Flows, Licensed Vehicles & Congestion Charge** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "london-traffic-flows-licensed-vehicles-congestion-charge": {
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
