# Amsterdam City Status & Incidents MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/amsterdam-city-status-incidents)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Keyless access to Amsterdam's live city status: electricity outages, road works, citizen reports and public street-light & clock incidents — no API key.

## Description
Amsterdam's incident and public-service status data, keyless, straight from the city's DSO open-data platform. The stroomstoringen, wior, meldingen and storingsmeldingen_ovl_en_klokken services are public — no credentials.

### What you can do
- **Power outages** — electricity outage reports by status, energy type and outage type
- **Road works** — planned and executing road construction/repair works by type, status and project
- **Citizen reports** — the city's register of citizen incident reports, by theme, category, neighbourhood and status
- **Street light & public clock status** — outages on the public lighting and public clocks network, by object type and status

### Who is this for
City-operations agents, incident monitoring, local disruption alerts and dashboards on Amsterdam public infrastructure.


## Available Tools (5)
- **get_power_outages**: g. opgelost = resolved, actief = active), energy type (Elektriciteit / Gas), cause, reported / estimated / end dates, affected postcodes, streets, places and the affected area polygon (EPSG:28999). Filter by status or energy type.

Get electricity and gas outage reports in Amsterdam
- **list_road_works**: g. Uitvoering = in execution) and work type (e.g. Vervanging = replacement), with the work area polygon (EPSG:28999). Filter by work type, status or project name.

List road works and construction notices on Amsterdam streets
- **search_citizen_reports**: Filter by theme, main category, neighbourhood code or external status.

Search citizen trouble reports registered with the city
- **list_street_light_status**: g. Gevel Armaturen), object number, out-of-service status (storingstatus, 0 = OK) and report status (meldingstatus), with latitude / longitude and geometry. Filter by object type or status codes.

List public street light fixtures and their status
- **list_public_clocks**: g. Klok), object number, out-of-service and report status codes, with latitude / longitude and geometry. Filter by type or status codes.

List public clocks and their status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amsterdam City Status & Incidents** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show the open electricity outages right now."

**🤖 AI Agent:**
> get_power_outages filtered by open status returns the current outage reports: affected area, outage type, energy type, start time and current status (e.g. in progress vs resolved).

---

**👤 You:**
> "Which road works are currently in execution?"

**🤖 AI Agent:**
> list_road_works filtered by main status (in execution) returns the work rows: work type, main status, project name, location description and period.

---

**👤 You:**
> "How many open citizen reports are there for the 'water' theme?"

**🤖 AI Agent:**
> search_citizen_reports filtered by the theme returns the open report rows: theme, category, neighbourhood, external status and report datetime. Page through with page/page_size.


## ❓ FAQ

**Q: Do I need an API key?**
No. The stroomstoringen, wior, meldingen and storingsmeldingen_ovl_en_klokken services of the city's DSO open-data platform are public (OPENBAAR) and work without credentials.

**Q: How fresh is the data?**
Outages and road works are updated by the city's own incident systems on a regular basis and are a near-real-time view of public incidents; citizen reports reflect the register at its sync interval. Treat status values as the official Dutch terms and map them to your own states.

**Q: Why are the status values in Dutch?**
The city publishes the data in Dutch; for example outage status uses values like 'opgelost' (resolved) and road works main status uses 'In uitvoering' (in execution). The tools return the raw values — translate or map them in your agent rather than filtering on a guessed English term.

**Q: Can I filter outages by postal code?**
No. The affected-postcodes field on outage records is a semicolon-joined string, so exact-match filtering by postal code is not meaningful. Filter by status, energy type, outage type or affected area instead, and narrow client-side if you need a specific postal code.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/amsterdam-city-status-incidents](https://vinkius.com/en/ai-agent-connect/amsterdam-city-status-incidents)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amsterdam City Status & Incidents** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amsterdam-city-status-incidents` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amsterdam City Status & Incidents** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amsterdam-city-status-incidents": {
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
