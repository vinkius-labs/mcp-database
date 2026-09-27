# NYC Crime & Shootings MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-crime-shootings)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Keyless NYC crime data: shooting incidents with offender and victim detail, incident counts and top precincts, bias-motive crime complaints, and the historic NYPD complaint dataset — no API key.

## Description
Official city crime records, keyless, built for analysis and verification.

### What you can do
- **List shootings** — gunshot incidents with date, borough, location, precinct and lat/lon
- **Count shootings** — totals by borough, precinct or date window
- **Offender / victim detail** — the suspected offenders and victims of one incident (age groups, sex, fatality flag)
- **Hate crimes** — bias-motive complaints with offense and motive descriptions
- **Historic NYPD complaints** — the city's complaint system of record with offense descriptions and law categories
- **Top shooting precincts** — the precincts with the most incidents in a trailing window

### Who is this for
Civic safety analysis, journalism, urban research and any agent that must verify a crime claim against official records.


## Available Tools (7)
- **count_shootings**: Use it to size a question before listing incidents; for "which precincts" use top_shooting_precincts.

Count shooting incidents with filters
- **list_hate_crimes**: Filter by patrol_borough_name, offense_category or complaint_year_number (e.g. "2025").

List bias-motive (hate) crime complaints
- **list_shooting_offenders**: Give the incident_key from list_shootings. Ages are ranges, not exact values.

Suspected offenders recorded in one shooting incident
- **list_shooting_victims**: Give the incident_key from list_shootings.

Victims recorded in one shooting incident
- **list_shootings**: Each incident has an incident_key that keys the offender and victim detail tables — use it with list_shooting_offenders / list_shooting_victims. boro values are UPPERCASE (BROOKLYN, QUEENS, ...); dates are ISO "YYYY-MM-DD".

List NYC gunshot/shooting incidents with location and precinct
- **search_nypd_complaints**: Filter by boro_nm, ofns_desc (exact offense text), law_cat_cd, or a cmplnt_fr_dt window. This is the historic system of record — newer complaints use a different format.

Search historic NYPD complaint data (arrests and non-arrests)
- **top_shooting_precincts**: Widen or narrow with days. Precinct codes come back as numbers; use list_shootings with precinct to inspect them.

Precincts with the most shooting incidents in a recent window


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Crime & Shootings** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many shootings in Brooklyn last year?"

**🤖 AI Agent:**
> count_shootings with boro "BROOKLYN" and an occur_date window returns the total; list_shootings then shows the incidents themselves.

---

**👤 You:**
> "Show the top shooting precincts over five years"

**🤖 AI Agent:**
> top_shooting_precincts with days=1825 ranks precincts by incident count in that window.

---

**👤 You:**
> "What happened in shooting incident INC-KEY-123?"

**🤖 AI Agent:**
> list_shooting_offenders and list_shooting_victims with that incident_key return the recorded suspects and victims (age groups, sex, fatality flag).


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: Are these official records?**
Yes. All datasets are published on NYC Open Data by the city: shooting incident/offender/victim extracts from NYPD reporting, the bias-motive complaints series and the historic complaint system of record.

**Q: How are ages and races reported?**
Offender and victim tables report age groups (not exact ages) plus sex and race, as recorded in the incident. The victim table carries a fatality flag (stat_murder_flg).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-crime-shootings](https://vinkius.com/en/ai-agent-connect/nyc-crime-shootings)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Crime & Shootings** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-crime-shootings` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Crime & Shootings** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-crime-shootings": {
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
