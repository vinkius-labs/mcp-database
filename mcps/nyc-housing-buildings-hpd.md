# NYC Housing & Buildings (HPD) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-housing-buildings-hpd)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless NYC housing data: HPD HMC complaints, NYCHA HMC violations, repair & vacate orders, housing litigation, DOB open-market order charges, building jurisdiction programs and heat-sensor buildings — no API key.

## Description
New York City housing and building-maintenance records, keyless.

### What you can do
- **HMC complaints** — housing maintenance complaints received, with the maintenance category, HMC problem code, status (OPEN/CLOSE) and address, within a received-date window (90 days by default)
- **Top problem codes** — the most reported HMC problem codes in a window, ranked
- **NYCHA HMC violations** — violations at NYCHA developments with hazard class and inspection date
- **Repair & vacate orders** — HPD orders with the vacate reason, type, effective date and number of vacated units
- **Housing litigation** — cases by type, status, judgement text and respondent
- **Open-market order charges** — DOB OMO charges with the award amount, work type and lifecycle stage
- **Building jurisdiction programs** — the program and record status of one building by building ID
- **Heat-sensor buildings** — buildings equipped with HPD heat sensors, by borough or status

### Who is this for
Housing research, code enforcement, property due diligence and urban policy. The HPD complaints table is very large, so complaint searches and problem-code rankings are always scoped to a received-date window; the litigation and charge tables are large but answer fast, and the NYCHA, vacate-order, jurisdiction and heat-sensor tables are small.


## Available Tools (8)
- **list_heat_sensor_buildings**: g. "Active"), the postcode and coordinates. The list is small (a few hundred buildings) — no date window is applied. Filter by borough (title case, e.g. "Brooklyn") or current status.

List buildings with HPD heat sensors
- **lookup_building_programs**: g. "PVT" private), the record status (e.g. "Inactive"), the building address, the BBL, the NTA and the coordinates. building_id is required — it is the DOB building ID (borough-block-lot form, e.g. "1-00016-3859"). Management program and record status narrow the result.

Look up a building's jurisdiction program status
- **search_hmc_complaints**: g. "MANHATTAN"), the major/minor maintenance category, the HMC problem code, the complaint status ("OPEN" or "CLOSE") and coordinates. The dataset is very large, so a received-date window is always applied: after defaults to 90 days ago when omitted. Filters are exact matches; borough values are stored uppercase and the tool uppercases the borough and complaint_status inputs for you.

Search HPD Housing Maintenance Code complaints
- **search_housing_litigations**: g. "CLOSED"), the judgement text, the respondent, the case open date and the building address. Filter by case type, case status, respondent (exact match) or building ID. The dataset is a few hundred thousand cases; filter it — results are the matching rows in dataset order.

Search housing litigation cases
- **search_nycha_violations**: g. "RED HOOK WEST"), the violation description, the hazard class, the inspection date, the BBL and coordinates. A small dataset (a few thousand rows) — no date window is applied. The development_name filter is an exact match and the tool uppercases it, since development names are stored uppercase.

Search NYCHA HMC violations
- **search_omo_charges**: g. "PLUMB"), the lifecycle stage (e.g. "Standing Building"), the service-charge flag and the building address (borough is title case, e.g. "Brooklyn"). The dataset is a half million rows; always pass a filter and a limit.

Search DOB open-market order charges
- **search_vacate_orders**: The dataset is small (under ten thousand orders) — no date window is applied.

Search HPD repair and vacate orders
- **top_hmc_problem_codes**: days defaults to 90 (max 365) — the dataset is large, so the window is always applied. Each row is one problem code with its complaint count in the window.

Most reported HMC problem codes in a window


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Housing & Buildings (HPD)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the most common HMC complaint codes in the past 90 days?"

**🤖 AI Agent:**
> top_hmc_problem_codes with days: '90' returns the problem codes ranked by complaint count inside the 90-day window; widen it with days up to 365.

---

**👤 You:**
> "Find open HMC complaints about heat and hot water in Manhattan."

**🤖 AI Agent:**
> search_hmc_complaints with borough: "Manhattan", major_category: "Heat & Hot Water" and complaint_status: "OPEN" returns the open complaints in the default 90-day window; pass after (and before) to shift it.

---

**👤 You:**
> "Which buildings participate in the HPD heat-sensor program?"

**🤖 AI Agent:**
> list_heat_sensor_buildings with current_status: "Active" returns the active buildings with their unit count, program start date, address and coordinates; add borough to narrow to one borough.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: Why do HMC complaint searches use a date window?**
The HPD HMC complaints table is very large, so search_hmc_complaints applies a received-date window by default (90 days back; pass after to shift it) and top_hmc_problem_codes ranks codes over a days window (90 by default, max 365). The other datasets are small and need no window.

**Q: Which borough values do the housing datasets use?**
They differ per dataset: HMC complaints store boroughs in UPPERCASE ("MANHATTAN"), the OMO charge table in title case ("Brooklyn"), and vacate orders use two-letter codes ("BK"). Text filters are case-insensitive partial matches, so "manhattan" works in the HMC table.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-housing-buildings-hpd](https://vinkius.com/en/ai-agent-connect/nyc-housing-buildings-hpd)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Housing & Buildings (HPD)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-housing-buildings-hpd` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Housing & Buildings (HPD)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-housing-buildings-hpd": {
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
