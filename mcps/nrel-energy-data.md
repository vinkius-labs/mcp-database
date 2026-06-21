# NREL Energy Data MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nrel-energy-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nrel-energy-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nrel-energy-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access renewable energy and fuel data via NREL — track fuel stations, solar resources, and utility rates directly from your AI agent.

## Description
Connect to the **National Renewable Energy Laboratory (NREL)** API through your AI agent and explore a vast archive of sustainable energy data and analysis tools using natural conversation.

### What you can do

- **Alternative Fuels** — List and locate alternative fuel stations (Electric, Hydrogen, E85) globally, or find the nearest one to any address.
- **Solar Production** — Run PVWatts® estimates to calculate the potential energy production of photovoltaic systems based on specific system configurations.
- **Resource Intelligence** — Access detailed solar radiation data (GHI, DNI) and check geothermal resource potential for any coordinate.
- **Utility Oversight** — Retrieve residential and industrial electricity rates and identify which utility companies serve a specific area.
- **Incentives & Laws** — Browse federal and state laws and incentives for alternative fuels and energy-efficient vehicles.
- **Deep Inspection** — Fetch complete metadata and station details using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your NREL Developer API Key (get one for free at developer.nrel.gov/signup)
3. Start exploring renewable energy data from Claude, Cursor, or any MCP client

### Who is this for?

- **Sustainability Researchers** — quickly retrieve solar and geothermal resource data for environmental analysis.
- **EV & Fleet Managers** — locate charging infrastructure and alternative fuel stations along routes.
- **Energy Consultants** — automate the retrieval of utility rates and solar production estimates for client reporting.


## Available Tools
- **get_geothermal_resource**: Check geothermal resource potential
- **get_nearest_stations**: Find nearest fuel stations
- **get_pvwatts_estimates**: Estimate solar energy production
- **get_solar_data_query**: Check solar dataset availability
- **get_solar_resource**: Get solar radiation data
- **get_station_details**: Get specific station details
- **get_utility_companies**: Identify local utility companies
- **get_utility_rates**: Get average electricity rates
- **list_alt_fuel_stations**: ) in the database.

List all alternative fuel stations
- **list_transportation_incentives**: List alternative fuel incentives


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NREL Energy Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all electric vehicle charging stations in Asheville, NC."

**🤖 AI Agent:**
> Searching NREL database... I've found several EV charging stations in Asheville, NC, including 'Asheville City Hall' and 'Whole Foods Market'. Would you like the detailed access info and charging levels for any of these?

---

**👤 You:**
> "Estimate solar energy production for a 5kW system at latitude 35.6, longitude -82.5."

**🤖 AI Agent:**
> Running PVWatts® estimation... For a 5kW system at those coordinates, the estimated annual AC energy production is approximately 7,200 kWh. The average monthly production peaks in July. Shall I provide the full monthly breakdown?

---

**👤 You:**
> "What are the average electricity rates for residential buildings in zip code 28801?"

**🤖 AI Agent:**
> Retrieving utility rates... For zip code 28801, the average residential electricity rate is $0.12 per kWh. The commercial rate is $0.10 and the industrial rate is $0.08. Would you like to identify the utility companies serving this area?


## Installation & Usage

To install and use the **NREL Energy Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nrel-energy-data](https://vinkius.com/mcp/nrel-energy-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
