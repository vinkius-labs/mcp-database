# HUD Fair Market Rents MCP Server

Access official US Department of Housing and Urban Development (HUD) data for Fair Market Rents and Income Limits.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hud-fair-market-rents)

## Overview
**Category:** real-estate
**Tools Count:** 8

## Description
Connect directly to the **U.S. Department of Housing and Urban Development (HUD)** API to retrieve critical housing and economic data through natural conversation. This server provides comprehensive access to Fair Market Rents (FMR) and Income Limits (IL) across the United States.

### What you can do

- **Geographic Discovery** — List all states, counties, and metropolitan areas with their corresponding FIPS and CBSA codes.
- **Fair Market Rents (FMR)** — Fetch detailed rent data for specific counties or metro areas, or retrieve entire statewide datasets for comparative analysis.
- **Income Limits (IL)** — Access median income data and limits for very low, extremely low, and low-income families by entity ID.
- **MTSP Data** — Retrieve Multifamily Tax Subsidy Project income limits for specific housing projects.
- **Historical Analysis** — Query data for specific years to track housing market trends.

### How it works

1. Subscribe to this server
2. Enter your HUD User API Key
3. Start querying housing data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Real Estate Professionals** — Quickly verify current market rents for property valuations and rental listings.
- **Policy Analysts & Researchers** — Gather large-scale housing data for economic research and urban planning.
- **Housing Agencies** — Instantly check income eligibility limits for housing assistance programs.


## Available Tools
- **get_fmr_data**: Get Fair Market Rent (FMR) data by entity ID
- **get_il_data**: Get Income Limits (IL) data by entity ID
- **get_mtsp_il_data**: Get Multifamily Tax Subsidy Project (MTSP) Income Limits data
- **get_state_fmr_data**: Get Statewide Fair Market Rent (FMR) data
- **get_state_il_data**: Get Statewide Income Limits (IL) data
- **list_counties**: List all counties in a specific state
- **list_metro_areas**: List all Metropolitan areas
- **list_states**: List all states and territories


## Installation & Usage

To install and use the **HUD Fair Market Rents** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hud-fair-market-rents](https://vinkius.com/mcp/hud-fair-market-rents)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
