# EPA ECHO (Enforcement & Compliance) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/epa-echo-enforcement-compliance)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/epa-echo-enforcement-compliance-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/epa-echo-enforcement-compliance-mcp)
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


## Available Tools
- **get_detailed_facility_report**: Get a comprehensive report for a single facility across all available environmental program records
- **get_effluent_chart**: Get dynamic charts and tables of permitted effluent limits, releases, and violations for CWA wastewater discharge permits
- **search_air_facilities**: Search for stationary sources regulated under the Clean Air Act (CAA)
- **search_all_facilities**: ) using location or name.

Search across all environmental program records available in ECHO
- **search_hazardous_waste_facilities**: Search for hazardous waste handlers regulated under the Resource Conservation and Recovery Act (RCRA)
- **search_drinking_water_systems**: Search for public drinking water systems regulated under the Safe Drinking Water Act (SDWA)
- **search_water_facilities**: Search for facilities regulated under the Clean Water Act (CWA) and managed under the NPDES program


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


## Installation & Usage

To install and use the **EPA ECHO (Enforcement & Compliance)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epa-echo-enforcement-compliance](https://vinkius.com/mcp/epa-echo-enforcement-compliance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
