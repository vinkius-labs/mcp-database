# NYC Emergency Response (FDNY & EMS) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-emergency-response-fdny-ems)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless NYC emergency data: FDNY EMS and fire incident dispatches, firehouse and alarm-box locations, monthly FDNY response times, fire-company incidents and line-of-duty deaths — no API key.

## Description
New York City emergency-response records, keyless.

### What you can do
- **EMS dispatches** — ambulance incident dispatches with call type, severity level, response times and borough, within a date window (90 days by default)
- **Fire dispatches** — fire incident dispatches with classification, highest alarm level and response time
- **FDNY firehouses** — station locations by borough, with address, postcode and coordinates
- **Fire-company incidents** — incidents responded to by fire companies, by incident type, borough or fire box
- **Monthly response times** — average FDNY response time per incident classification and borough, one calendar month at a time (historical, back to 2009)
- **Alarm boxes** — in-service FDNY alarm box locations by borough, box type or zip
- **Line-of-duty deaths** — the historical FDNY memorial list, filterable by rank or unit

### Who is this for
Emergency-services research, response-time analysis, urban safety planning and journalism. Dispatch data lags a few months, so recent months may be empty.


## Available Tools (7)
- **get_fdny_response_times**: year_month is "YYYY-MM" (data is historical, back to 2009).

FDNY average response times for one month, by classification and borough
- **list_alarm_boxes**: Filter by borough, box type or zip.

List in-service FDNY alarm box locations
- **list_fdny_duty_deaths**: A small memorial dataset; filter by rank or unit.

List FDNY line-of-duty deaths
- **list_fdny_firehouses**: Filter by borough.

List FDNY firehouse locations
- **search_ems_dispatches**: The borough value is uppercase (BRONX, BROOKLYN, MANHATTAN, QUEENS, "RICHMOND / STATEN ISLAND", UNKNOWN). The dataset is large, so a date window is always applied: after defaults to 90 days ago when omitted (data lags a few months).

Search FDNY EMS incident dispatches with response times
- **search_fire_company_incidents**: Filter by incident type, borough (title case) or fire box.

Search incidents responded to by FDNY fire companies
- **search_fire_dispatches**: The dataset is large, so a date window is always applied: after defaults to 90 days ago when omitted (data lags a few months).

Search FDNY fire incident dispatches


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Emergency Response (FDNY & EMS)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many fire dispatches happened in the Bronx in the last 30 days?"

**🤖 AI Agent:**
> search_fire_dispatches with borough: "BRONX" (uppercase in dispatch data) and after set to 30 days ago returns the incident dispatches with classification, highest alarm level and response time.

---

**👤 You:**
> "What was the average FDNY response time in June 2025?"

**🤖 AI Agent:**
> get_fdny_response_times with year_month: "2025-06" returns the average response time in seconds and incident counts per classification and borough for that month; optional classification or borough filters narrow it further.

---

**👤 You:**
> "List the FDNY firehouses in Staten Island."

**🤖 AI Agent:**
> list_fdny_firehouses with borough: "Staten Island" (title case in location lists) returns every station with address, postcode, community council and coordinates.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: How current are the dispatch datasets?**
Dispatch rows lag a few months behind real time (the newest rows stop around mid-2026), so both dispatch search tools apply a 90-day window by default. Monthly response-time statistics are historical, back to 2009, and are stored as "YYYY/MM" — the year_month parameter accepts "YYYY-MM" and normalizes it.

**Q: Which borough values should I use?**
Dispatch data stores boroughs in UPPERCASE — "BRONX", "BROOKLYN", "MANHATTAN", "QUEENS", "RICHMOND / STATEN ISLAND" (Staten Island), UNKNOWN. Location lists (firehouses, alarm boxes, fire-company incidents) use title case — "Staten Island", "Manhattan". Each tool states its case in its description.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-emergency-response-fdny-ems](https://vinkius.com/en/ai-agent-connect/nyc-emergency-response-fdny-ems)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Emergency Response (FDNY & EMS)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-emergency-response-fdny-ems` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Emergency Response (FDNY & EMS)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-emergency-response-fdny-ems": {
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
