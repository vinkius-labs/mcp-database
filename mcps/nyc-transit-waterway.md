# NYC Transit & Waterway MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-transit-waterway)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless NYC transit & waterway data: NYC Ferry and Staten Island Ferry ridership, OPT bus breakdowns and school bus routes, bus stop shelters and real-time passenger information signs — no API key.

## Description
Municipal transit and waterway records for New York City, keyless.

### What you can do
- **NYC Ferry ridership** — daily boardings by route (AS, ER, GI, LE, RR, RS, RW, SB, SG, SV), stop and hour
- **Busiest ferry stops** — boardings ranked by stop over a bounded look-back window (90 days by default, up to 730)
- **Staten Island Ferry** — daily ridership between the Port Authority Bus Terminal and St. George
- **School-year bus breakdowns** — OPT bus breakdowns by school year ("2024-25"), borough, company and route
- **Bus stop shelters** — public shelter locations by borough or street
- **Real-time signs** — real-time passenger information (RTPi) sign locations by stop or corner
- **School bus routes** — DOE school bus routes by year, route number or vendor

### Who is this for
Transport planning, multimodal research, transit-oriented analysis and city operations. Ferry daily data runs from 2017; bus breakdowns and school bus routes are organized by school year, not calendar dates.


## Available Tools (8)
- **list_si_ferry_ridership**: George terminals per day. Rows are the most recent days first; optionally pin one date. The dataset is small — no date window needed.

Staten Island Ferry daily ridership counts
- **list_bus_stop_shelters**: Filter by borough name, street or shelter id.

List NYC bus stop shelters with location and evacuation flag
- **list_rtpi_signs**: Filter by stop name, corner or borough.

Real-time passenger information (RTPI) sign locations
- **search_bus_breakdowns**: school_year uses the "YYYY-YY" form (e.g. "2024-25").

OPT school bus breakdowns and running-late incidents
- **search_ferry_ridership**: Filter by route, stop name, direction or a date window (data covers 2017 to present).

Hourly NYC Ferry ridership by route, stop and direction
- **search_school_bus_routes**: Filter by school year ("YYYY-YY"), route number or vendor.

OPT school bus routes, service type and operating vendor
- **top_bus_breakdown_routes**: g. "2024-25"), most troubled routes first.

School bus routes with the most breakdowns in one school year
- **top_ferry_stop_boardings**: Optionally restrict to one route code.

Most boarded NYC Ferry stops over a look-back window


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Transit & Waterway** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which NYC Ferry stop had the most boardings in the last 30 days?"

**🤖 AI Agent:**
> top_ferry_stop_boardings with days: '30' returns stops ranked by total boardings over the window; search_ferry_ridership shows the underlying daily rows for a specific route or stop.

---

**👤 You:**
> "How many riders used the Staten Island Ferry in January 2026?"

**🤖 AI Agent:**
> list_si_ferry_ridership with a date window around January 2026 returns the daily ridership rows between the Port Authority Bus Terminal and St. George; sum the rows for a total.

---

**👤 You:**
> "Show me the school bus routes run by a specific vendor in 2024-25."

**🤖 AI Agent:**
> search_school_bus_routes takes the vendor name and school_year '2024-25' and returns the routes that vendor operated; search_bus_breakdowns can show which of those routes had the most breakdowns.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: Why does top_ferry_stop_boardings use a window?**
Boardings by stop are an aggregate over years of history, so the tool bounds the look-back: 90 days by default, up to 730 days via the days parameter. Pass days: '365' to widen the window.

**Q: Which dates do the transit datasets cover?**
NYC Ferry daily data runs from 2017; Staten Island Ferry rows carry service dates through early 2027; OPT bus breakdowns and school bus routes are organized by school year ("YYYY-YY"). Dispatch records lag a few months, so the newest months can be empty.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-transit-waterway](https://vinkius.com/en/ai-agent-connect/nyc-transit-waterway)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Transit & Waterway** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-transit-waterway` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Transit & Waterway** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-transit-waterway": {
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
