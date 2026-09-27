# NYC Parking & Enforcement MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-parking-enforcement)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless NYC parking data: open (current) parking citations, recently issued citations by fiscal year, official violation-code definitions, and parking meter status — no API key.

## Description
Municipal Parking Enforcement and DOP parking records, keyless.

### What you can do
- **Open citations** — current, unresolved parking tickets with plate, street, violation code, amount and status
- **Recently issued citations** — parking tickets issued in fiscal year 2026 or 2027 with the same detail
- **Violation codes** — the official definition and per-area amounts for every enforcement code (e.g. expired display, double parking, no standing zone)
- **Parking meters** — meter locations with status, pay-by-cell numbers and facility info

### Who is this for
Drivers checking citations, enforcement-pattern research, city operations analysis and jurisdiction comparisons of violation definitions and amounts.

Note: the open-citation set changes as tickets are paid or contested, so treat counts as a point-in-time snapshot, not a historical total.


## Available Tools (6)
- **count_open_violations**: The open-violations view cannot be counted in full, so a lower date bound is always applied: issue_after defaults to 90 days ago when omitted. Use it to gauge how many unresolved tickets a plate or area carries before listing rows.

Count open parking violations within a date window
- **list_parking_meters**: Filter by meter number, facility name, borough or street.

List NYC parking meters with status and pay-by-phone number
- **lookup_parking_code**: Codes are 2-3 digit numbers like "19" or "128".

What a parking violation code means and its fine amounts
- **search_parking_violations_issued**: Rows include the summons number, plate_id, violation code and description, vehicle make and street location. Resolve a violation code's fine with lookup_parking_code.

Search issued parking violations for one fiscal year
- **search_open_parking_violations**: Filter by plate (state-optional format), summons number, county or a date window. The plate column is "plate", not plate_id — that belongs to the issued datasets.

Search open (unresolved) parking violations and CitiCam
- **top_open_violation_types**: Optionally restrict to one county.

Most common open parking violation types over a look-back window


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Parking & Enforcement** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many open parking tickets are there citywide right now?"

**🤖 AI Agent:**
> count_open_violations returns the count of unresolved tickets within a date window (defaults to the last 90 days, since the open view cannot be scanned in full); top_open_violation_types shows which codes are the most common over the same window.

---

**👤 You:**
> "What does violation code 24 mean?"

**🤖 AI Agent:**
> lookup_parking_code("24") returns the official definition plus the Manhattan-below-96th and all-other-areas amounts for that code.

---

**👤 You:**
> "Are the parking meters on 5th Ave in Brooklyn working?"

**🤖 AI Agent:**
> list_parking_meters with on_street "5th Ave" (or lat/lon bounds) returns each meter with status, pay-by-cell number and facility.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: What is a citation?**
A parking citation (or ticket) is a written notice of a parking violation issued by the city. The open-citation set is the live, unresolved population — it changes as tickets are paid, reduced or contested, so any count is a snapshot.

**Q: Where do the fine amounts come from?**
The violation-code table carries the official definition of each code and the amount in Manhattan below 96th Street versus all other areas — the city's two-tier enforcement pricing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-parking-enforcement](https://vinkius.com/en/ai-agent-connect/nyc-parking-enforcement)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Parking & Enforcement** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-parking-enforcement` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Parking & Enforcement** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-parking-enforcement": {
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
