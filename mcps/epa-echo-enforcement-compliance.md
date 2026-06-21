# EPA ECHO (Enforcement & Compliance) MCP Server

Access US EPA environmental compliance data — search facilities, inspect air/water permits, and analyze enforcement history directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/epa-echo-enforcement-compliance)

## Overview
**Category:** government-public-data
**Tools Count:** 7

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


## Installation & Usage

To install and use the **EPA ECHO (Enforcement & Compliance)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epa-echo-enforcement-compliance](https://vinkius.com/mcp/epa-echo-enforcement-compliance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
