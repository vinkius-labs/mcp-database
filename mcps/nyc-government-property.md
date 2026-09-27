# NYC Government & Property MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-government-property)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless NYC government data: city payroll by fiscal year, open city job postings, City Council bills and local laws, the civil list, city-owned property, property assessments by BBL and City Record notices — no API key.

## Description
New York City government and property records, keyless.

### What you can do
- **City payroll** — employee records by fiscal year (2014–2025): agency, title, salary, overtime and total pay; count records per fiscal year and agency
- **Job postings** — open city jobs with agency, title, level, salary range and posting date
- **City Council legislation** — bills and local laws with matter id, status, sponsor, committee and dates
- **Civil list** — civil appointments (judges and officers) by calendar year, department or name
- **City-owned property (COLP)** — city parcels with owning agency, use type and coordinates, by agency code, use or community district
- **Property assessments** — valuation and assessment records (owner, building/tax class, values by period and year) for one BBL
- **City Record notices** — contract awards, amendments and public-comment notices with agency, type and dates

### Who is this for
Government transparency, workforce and salary research, procurement and real-estate analysis. Payroll is large (over half a million rows per year), so fiscal year is always applied; City Record notices use a 90-day window by default.


## Available Tools (8)
- **count_city_payroll**: Use it to gauge the size of an agency workforce before listing rows.

Count NYC payroll records for a fiscal year and agency
- **search_council_bills**: Filter by matter id, status, sponsor name (partial match) or committee (partial match).

Search NYC City Council bills and local laws
- **list_city_job_postings**: Most recent postings first. Filter by agency, job category, career level, indicator or work location.

List open NYC city job postings with salary ranges
- **list_city_record_notices**: The dataset is current, so a start-date window is always applied: after defaults to 90 days ago when omitted.

List recent City Record notices by agency
- **list_civil_list**: Filter by calendar year, department or name (partial match).

List NYC civil list appointees (judges and civil officers)
- **search_city_owned_property**: The agency column holds short agency codes (e.g. "BLDGS", "ACS", "BOC"); filter by agency code, use type or community district.

Search city-owned and leased property (COLP) parcels
- **search_city_payroll**: Fiscal years run 2014-2025; defaults to 2025. Name filters use partial matching. The dataset is large — always set a fiscal year when counting or aggregating.

Search NYC citywide payroll (employee salary records by fiscal year)
- **search_property_assessments**: The BBL is the 10-digit borough-block-lot code (e.g. "1-00016-3859" or "1000163859"); dashes are optional and stripped. The table covers every tax lot in the city, so a BBL is required.

Look up NYC property valuation and assessment records by BBL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Government & Property** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many employees does the Department of Education have in FY 2025?"

**🤖 AI Agent:**
> count_city_payroll with fiscal_year: "2025" and agency_name: "DEPT OF EDU" returns the record count for that agency in the fiscal year; agency names are the uppercase payroll codes.

---

**👤 You:**
> "What is the assessed value of BBL 1-00016-3859?"

**🤖 AI Agent:**
> search_property_assessments with bbl: "1-00016-3859" returns the valuation/assessment records for that lot: owner, building and tax class, stories, and full valuation/assessment by period and year.

---

**👤 You:**
> "List recent City Record contract award notices."

**🤖 AI Agent:**
> list_city_record_notices (90-day window by default) returns recent notices with agency, notice type, short title and start/end dates; pass agency_name to narrow to one agency.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: Which fiscal years does the payroll data cover?**
Fiscal years 2014–2025. Both payroll tools default to FY 2025 when omitted. The full payroll table is over half a million rows per year, so every count is scoped to a fiscal year (plus optionally an agency) — the dataset itself is never scanned in full.

**Q: What is the BBL format?**
The 10-digit borough-block-lot code, e.g. "1-00016-3859". Dashes are optional and stripped; search_property_assessments validates the code before querying and returns a clear error for a malformed BBL.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-government-property](https://vinkius.com/en/ai-agent-connect/nyc-government-property)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Government & Property** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-government-property` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Government & Property** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-government-property": {
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
