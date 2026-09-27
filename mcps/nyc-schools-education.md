# NYC Schools & Education MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-schools-education)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Keyless NYC DOE education data: School Quality Report metrics, chronic absenteeism by school and citywide, enrollment capacity, the public high school directory and 2019-20 performance ratings — no API key.

## Description
New York City Department of Education records, keyless.

### What you can do
- **School quality metrics** — one row per school metric (name, value, student count) for a school year and report year
- **Chronic absenteeism by school** — end-of-year attendance and chronic-absent statistics for one DBN, by grade and category
- **Citywide absenteeism** — the same statistics aggregated citywide
- **Enrollment capacity** — enrollment vs. target capacity and utilization at building and organization level, by district
- **High school directory** — 2019-20 public high schools with overview, transit, grades offered and contact
- **High school performance** — 2019-20 School Quality Guide ratings, benchmark percentages and demographics for one DBN

### Who is this for
Education research, school selection, equity analysis and journalism. Schools are identified by their 6-digit DBN (e.g. "04M479"). Attendance data covers school years 2016-17 through 2022-23; report years run 2016 to 2025.


## Available Tools (6)
- **get_high_school_performance**: g. "04M479"): enrollment, the survey and quality-report ratings, the percent scoring at or above benchmark in ELA and Math, and demographic shares. Returns an error if the DBN has no record in the guide.

2019-20 School Quality Guide performance ratings for one high school
- **get_citywide_absenteeism**: School years are "YYYY-YY" (2016-17 through 2022-23); defaults to the most recent year.

Citywide chronic absenteeism and attendance statistics
- **get_school_chronic_absenteeism**: g. "04M479"): total days, days absent/present, attendance rate and chronic-absent counts, broken down by grade and category. school years are "YYYY-YY" (2016-17 through 2020-21).

Chronic absenteeism and attendance for one school (by DBN)
- **list_high_schools**: Filter by borough or school name (partial match).

List NYC DOE public high schools (directory)
- **search_enrollment_capacity**: Filter by building name (partial match), organization name or district.

DOE building and organization enrollment capacity and utilization
- **search_school_quality_metrics**: Identify schools by DBN (the 6-digit code, e.g. "04M479") or school name; filter by metric variable name or report year.

Search NYC DOE School Quality Report metrics by school


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Schools & Education** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the chronic absenteeism for school 04M479 in 2020-21."

**🤖 AI Agent:**
> get_school_chronic_absenteeism with dbn: "04M479" and year: "2020-21" returns the end-of-year attendance and chronic-absent rows for that school, broken down by grade and category.

---

**👤 You:**
> "What metrics did a school report in 2024?"

**🤖 AI Agent:**
> search_school_quality_metrics with the dbn (or a school name) and report_year: "2024" returns each metric row with its display name, value and student count; metric_variable_name narrows to one metric.

---

**👤 You:**
> "What is the citywide chronic absenteeism rate?"

**🤖 AI Agent:**
> get_citywide_absenteeism returns the citywide end-of-year attendance and chronic-absent statistics by grade and category, optionally pinned to one school year; the most recent year is used when omitted.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: How are schools identified?**
By their 6-digit DBN code (e.g. "04M479"). get_school_chronic_absenteeism and get_high_school_performance require the DBN; the other tools can search by school name (partial match).

**Q: What year formats do the education datasets use?**
School Quality Reports use 4-digit report years (2016–2025). Attendance and absenteeism datasets use school years in "YYYY-YY" form ("2016-17" through "2022-23"). The high school directory and the performance ratings are the 2019-20 editions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-schools-education](https://vinkius.com/en/ai-agent-connect/nyc-schools-education)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Schools & Education** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-schools-education` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Schools & Education** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-schools-education": {
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
