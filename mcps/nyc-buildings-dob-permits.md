# NYC Buildings & DOB Permits MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-buildings-dob-permits)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Keyless NYC building intelligence: DOB permit filings, DOB NOW permits, building violations, DOB complaints, housing code violations, PLUTO parcel records and vacant storefronts — no API key.

## Description
The city's building-permit and property-record stack on NYC Open Data, in one keyless MCP.

### What you can do
- **Search DOB permits** — filings (New Building, Alteration 1/2/3, Change of Occupancy) with job number, BIN, street, work type, status and filing date
- **Search DOB NOW permits** — the online-permit pipeline (wiring, plumbing, minor work)
- **Search building violations** — open/closed code violations by BIN, type or issue window
- **Search DOB complaints** — public reports of building conditions, by category or status
- **Search housing code violations** — HCB inspections (heat/hot water, lead, fire safety) by building, class and status
- **Search PLUTO** — the city land-use file: zoning, building class, owner and assessed value per parcel
- **Search vacant storefronts** — the annual city survey of vacant commercial ground floors
- **Count permit activity** — total filings matching borough / work type / date filters

### Who is this for
Real-estate research, construction-market tracking, code-enforcement monitoring and property due diligence.


## Available Tools (8)
- **count_permit_activity**: Use it to size construction activity before pulling individual filings with search_dob_permits.

Count DOB permit filings with filters
- **search_dob_complaints**: Filter by complaint_number, bin, house_street or complaint_category; status shows whether the complaint is open or closed.

Search DOB complaints (public reports about buildings)
- **search_dob_permits**: A filing's full identifier is job__ plus job_doc___ (e.g. 12345678901 + 1A01); bin__ is the unique building number. work_type is Building, Interior, Site or Other; job_type includes New Building, Alteration 1/2/3, and Change of Occupancy. Borough values look like "Manhattan" or "Bronx". Dates are ISO "YYYY-MM-DD".

Search NYC DOB building permit filings (Alteration, New Building, ...). Column names like bin__ / job__ carry literal trailing underscores
- **search_dob_violations**: Filter by bin (building), violation_number, issue date range or violation_type (e.g. "Violation of Law", "Administrative"). Rows include the description and disposition date when closed.

Search DOB building violations (code enforcement)
- **search_dobnow_permits**: job_filing_number is the unique identifier; bin is the 10-digit building number. Dates are ISO "YYYY-MM-DD".

Search DOB NOW approved work permits (online-permit platform)
- **search_housing_violations**: class is A, B or C (severity; B = life safety, C = conditions, A = other); violationstatus is Open or Closed. buildingid is the HCB building identifier — a different key from DOB's bin.

Search housing code violations (HCB inspections)
- **search_pluto**: bldgclass codes look like "A" (walkups), "R15" (one-family), "S31" (stores); ownername is the legal owner. Filter by borough + block + lot (the BBL) or by exact street address.

Search PLUTO parcel/property records (the city's land use file)
- **search_vacant_storefronts**: reporting_year is the survey year (values like "2024"); vacant_6_30_or_date_sold says whether the spot was still vacant or sold. Useful for vacancy analysis by borough or street.

Search vacant commercial storefronts (annual city survey)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Buildings & DOB Permits** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Any new building permits in Manhattan this quarter?"

**🤖 AI Agent:**
> search_dob_permits with job_type "New Building", borough "Manhattan" and filing_after set to the start of the quarter returns matching filings with status and issue dates.

---

**👤 You:**
> "Zoning and owner of the lot at 100 Broadway, lower Manhattan"

**🤖 AI Agent:**
> search_pluto with address "100 BROADWAY" returns the parcel's zonedist codes, building class, land use, owner name and assessed values.

---

**👤 You:**
> "How many open housing code B-violations citywide?"

**🤖 AI Agent:**
> Search the housing violations dataset with class "B" and violationstatus "Open" — the tool returns matching rows; count them or group by boro with dataset_stats on the open-data MCP.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: What is a BIN?**
BIN (Building Identification Number) is the city's 10-digit id for one physical building, shared across the DOB and housing datasets. PLUTO keys buildings by borough+block+lot instead.

**Q: Borough values differ across datasets — how do I know the format?**
Formats are dataset-specific: 311 and shootings use UPPERCASE ("QUEENS"), food and sanitation use Title Case ("Queens"), DOT potholes use single-letter codes. Tool descriptions state the expected values, and the errors from a mismatched value are reported verbatim by the platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-buildings-dob-permits](https://vinkius.com/en/ai-agent-connect/nyc-buildings-dob-permits)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Buildings & DOB Permits** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-buildings-dob-permits` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Buildings & DOB Permits** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-buildings-dob-permits": {
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
