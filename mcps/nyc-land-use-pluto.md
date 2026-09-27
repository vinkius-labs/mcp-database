# NYC Land Use (PLUTO) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-land-use-pluto)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless NYC land-use data: PLUTO tax lots by zoning, building class, land use, owner and assessments, plus the PLUTO change file — no API key.

## Description
New York City's official land-record system, PLUTO, keyless.

### What you can do
- **Tax lot lookup** — the full PLUTO record for one borough-block-lot: zoning district, building class, land use, owner, lot/building areas, unit counts, year built, assessments and coordinates (the BBL is passed plainly, "4-08786-0042", and PLUTO's float storage is handled for you)
- **Tax lot search** — lots filtered by borough (name or two-letter code), community district, ZIP, zoning district, building class, land use or street address
- **Lot count** — a fast count of lots matching a filter, to gauge size before listing
- **Top land uses** — land-use codes ranked by lot count, citywide or for one community district
- **PLUTO changes** — the change file: field-level changes per lot with old/new values, change type, reason and the PLUTO version applied

### Who is this for
Real-estate research, urban planning and zoning analysis. PLUTO carries the current version of the land records (about 850,000 lots), and the change file shows how the records were corrected since the last publication.


## Available Tools (5)
- **count_tax_lots**: A single fast count — use it to gauge result size before listing lots.

Count NYC PLUTO tax lots matching a filter
- **lookup_tax_lot**: Pass the BBL as a plain 10-digit code ("4087860042") or with hyphens ("4-08786-0042") — hyphens are stripped automatically. PLUTO stores the BBL in a float form, which the lookup handles for you.

Look up a NYC tax lot (PLUTO)
- **search_pluto_changes**: g. "Zero lot area") and the PLUTO version it applied to (e.g. "26v2"). The change file stores the BBL as a plain digit string (unlike PLUTO itself, which stores the float form) — hyphens are stripped automatically. Filter by BBL, changed field, change type, reason (exact match) or version.

Search PLUTO change-file records
- **search_tax_lots**: Filters: borough (by name "Brooklyn" or two-letter code "BK" — PLUTO stores the two-letter code), community district "cd" (three-digit code, e.g. "413"), ZIP code, zoning district (e.g. "R1-2"), building class (e.g. "A5"), land use (e.g. "1" one-family dwelling) and street address (exact match, e.g. "W 42 ST"). No date window applies; pass a filter and bound with limit.

Search NYC PLUTO tax lots
- **top_land_use**: Each row is one land-use code with its lot count. Optionally restrict to one borough or one community district "cd". The aggregation runs citywide and returns fast — no date window is needed.

Top land uses across NYC (PLUTO)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Land Use (PLUTO)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is zoned and built on tax lot 4-08786-0042?"

**🤖 AI Agent:**
> lookup_tax_lot with bbl: "4-08786-0042" returns the full PLUTO record: zoning district, building class, land use, owner, areas, unit counts, year built, assessments and coordinates.

---

**👤 You:**
> "How many one-family dwelling lots are in community district 413?"

**🤖 AI Agent:**
> count_tax_lots with cd: "413" and landuse: "1" returns the count of PLUTO lots in that community district with land use "1" (one-family dwelling); it is the fast way to gauge size before listing lots.

---

**👤 You:**
> "What changed in PLUTO for lot 1-00001-0301?"

**🤖 AI Agent:**
> search_pluto_changes with bbl: "1-00001-0301" returns the change-file rows for that lot: the changed field, old and new values, the change type, the reason and the PLUTO version the change applied to.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: How are tax lots identified?**
By the 10-digit borough-block-lot code (BBL), e.g. "4-08786-0042". Dashes are optional and stripped. PLUTO itself stores the BBL in a float form, which lookup_tax_lot and search_tax_lots handle for you; the PLUTO change file stores plain digit BBLs, which search_pluto_changes normalizes the same way.

**Q: Which borough values does PLUTO use?**
PLUTO stores boroughs as two-letter codes — MN (Manhattan), BX (Bronx), BK (Brooklyn), QN (Queens), SI (Staten Island). The tools accept the full name ("Manhattan") and convert it to the code automatically; the raw code works too.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-land-use-pluto](https://vinkius.com/en/ai-agent-connect/nyc-land-use-pluto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Land Use (PLUTO)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-land-use-pluto` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Land Use (PLUTO)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-land-use-pluto": {
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
