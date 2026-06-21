# HUD Fair Market Rents MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hud-fair-market-rents)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hud-fair-market-rents-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hud-fair-market-rents-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Access official US Department of Housing and Urban Development (HUD) data for Fair Market Rents and Income Limits.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HUD Fair Market Rents** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all US states and their codes."

**🤖 AI Agent:**
> I've retrieved the list of states. You can find codes like Alabama (AL, FIPS: 01), California (CA, FIPS: 06), and New York (NY, FIPS: 36). Which state would you like to explore further?

---

**👤 You:**
> "Show me the Fair Market Rent data for the state of Florida."

**🤖 AI Agent:**
> Fetching statewide FMR data for Florida (FL)... I have the data for all metro areas and counties. For example, in the Miami-Miami Beach-Kendall area, the FMR for a 2-bedroom apartment is $2,100. Would you like the full breakdown?

---

**👤 You:**
> "What are the income limits for entity ID 0603799999?"

**🤖 AI Agent:**
> Querying Income Limits for entity 0603799999 (Los Angeles County)... The median family income is $98,200. The 'Very Low Income' (50%) limit for a family of four is $59,500. Do you need the limits for other family sizes?


## Installation & Usage

To install and use the **HUD Fair Market Rents** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hud-fair-market-rents](https://vinkius.com/mcp/hud-fair-market-rents)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
