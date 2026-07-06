# EPA ECHO (Enforcement & Compliance) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/epa-echo-enforcement-compliance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access US EPA environmental compliance data — search facilities, inspect air/water permits, and analyze enforcement history directly.

## Description
Connect to the **EPA ECHO (Enforcement and Compliance History Online)** database to retrieve real-time environmental data. This server allows AI agents to query millions of records regarding facility compliance with the Clean Air Act, Clean Water Act, and hazardous waste regulations.

### What you can do

- **Multi-Program Search** — Use `search_all_facilities` to find entities across all environmental programs using names, cities, or zip codes.
- **Media-Specific Audits** — Narrow down searches to Air (`search_air_facilities`), Water (`search_water_facilities`), or Hazardous Waste (`search_hazardous_waste_facilities`) to find specific permit holders.
- **Detailed Facility Reporting** — Use `get_detailed_facility_report` to fetch a comprehensive compliance history, including violations and enforcement actions for a specific ID.
- **Effluent Analysis** — Access `get_effluent_chart` to retrieve dynamic data on permitted wastewater discharge limits and actual releases.
- **Drinking Water Safety** — Query `search_drinking_water_systems` to monitor public water systems regulated under the SDWA.

### How it works

1. Subscribe to this server
2. No complex API keys are required for public ECHO web services (enter 'PUBLIC' in the token field)
3. Start auditing environmental records from your AI client

### Who is this for?

- **Environmental Researchers** — quickly aggregate facility data across different states and regions.
- **Compliance Officers** — monitor permit statuses and historical violations without manual portal navigation.
- **Legal Professionals** — retrieve official enforcement records and effluent charts for litigation or due diligence.


## Available Tools (7)
- **get_effluent_chart**: Get dynamic charts and tables of permitted effluent limits, releases, and violations for CWA wastewater discharge permits
- **search_air_facilities**: Search for stationary sources regulated under the Clean Air Act (CAA)
- **search_all_facilities**: ) using location or name.

Search across all environmental program records available in ECHO
- **search_hazardous_waste_facilities**: Search for hazardous waste handlers regulated under the Resource Conservation and Recovery Act (RCRA)
- **search_drinking_water_systems**: Search for public drinking water systems regulated under the Safe Drinking Water Act (SDWA)
- **search_water_facilities**: Search for facilities regulated under the Clean Water Act (CWA) and managed under the NPDES program
- **get_detailed_facility_report**: Get a comprehensive report for a single facility across all available environmental program records


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EPA ECHO (Enforcement & Compliance)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all EPA-regulated facilities in Austin, TX."

**🤖 AI Agent:**
> I've found several facilities in Austin, TX. Notable ones include the 'Austin Water Utility' and various manufacturing sites. Would you like to see the detailed report for a specific one?

---

**👤 You:**
> "Get a detailed compliance report for facility ID 110000310211."

**🤖 AI Agent:**
> Fetching the Detailed Facility Report for 110000310211... This facility is regulated under the Clean Air Act and RCRA. It has had 2 informal enforcement actions in the last 5 years and is currently listed as 'In Compliance'.

---

**👤 You:**
> "Show me the effluent discharge chart for permit ID TX0004567."

**🤖 AI Agent:**
> Generating effluent chart data for TX0004567... I've retrieved the permitted limits vs. actual measurements for parameters like Nitrogen and TSS. There was one exceedance recorded in Q3 of last year.


## ❓ FAQ

**Q: How can I get the full compliance history for a specific facility?**
Use the `get_detailed_facility_report` tool with the specific Facility ID (p_id). This returns a comprehensive 'Detailed Facility Report' (DFR) covering all environmental programs, violations, and inspections.

**Q: Can I search for facilities by city or state?**
Yes! Tools like `search_all_facilities` or `search_water_facilities` accept `p_ct` (City) and `p_st` (State abbreviation) parameters to filter results geographically.

**Q: What information is included in the effluent charts?**
The `get_effluent_chart` tool provides data on permitted discharge limits, actual measured releases, and any exceedances or violations for Clean Water Act (NPDES) permits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epa-echo-enforcement-compliance](https://vinkius.com/mcp/epa-echo-enforcement-compliance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EPA ECHO (Enforcement & Compliance)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `epa-echo-enforcement-compliance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EPA ECHO (Enforcement & Compliance)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "epa-echo-enforcement-compliance": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
