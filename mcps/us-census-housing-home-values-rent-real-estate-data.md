# U.S. Census Housing — Home Values, Rent & Real Estate Data MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-census-housing-home-values-rent-real-estate-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/us-census-housing-home-values-rent-real-estate-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/us-census-housing-home-values-rent-real-estate-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Access the definitive source for U.S. residential real estate data. Extract median home values, median gross rent, ownership vs. renting rates, and vacancy data at the state and county level. Create full socioeconomic profiles.

## Description
U.S. Census housing data.

### 5 Tools
- **Housing by State** — Values, rent, ownership
- **Housing by County** — Drill down into local markets
- **State Profile** — Full socioeconomic snapshot
- **County Profile** — Deep dive into specific counties
- **Query Census** — Run any custom API query

### Authentication
Requires a free API key from the Census Bureau.


## Available Tools
- **get_housing_by_state**: renter-occupied, and vacant units for every state. The #1 dataset for real estate market analysis.

Get housing data for all states — home values, rent, ownership rates, vacancies
- **get_housing_by_county**: Essential for real estate investors, developers, and market researchers.

Get housing data for all counties in a state — values, rent, ownership
- **get_state_profile**: One query = complete state intelligence.

Get a comprehensive socioeconomic profile for a state — population, income, housing, demographics
- **get_county_profile**: Get a comprehensive profile for a specific county
- **query_census**: Specify ACS variables (e.g., B01003_001E for population), geography (state:*, county:*, place:*), optional in-clause for filtering, year, and dataset path. See api.census.gov/data.html for all available datasets and variables.

Run a custom Census API query — any dataset, variables, and geography


## 💬 Prompt Examples

Here are some examples of how you can interact with the **U.S. Census Housing — Home Values, Rent & Real Estate Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the median home value in California?"

**🤖 AI Agent:**
> 📊 **U.S. Census Bureau: Housing by State**

**California (06):**
- Median Home Value: $611,400
- Median Gross Rent: $1,768
- Owner-Occupied: 7,330,227
- Renter-Occupied: 5,903,115

---

**👤 You:**
> "How many houses are vacant in Nevada?"

**🤖 AI Agent:**
> 📊 **Housing by State**

**Nevada (32):**
- Total Housing Units: 1,310,211
- Occupied Units: 1,180,388
- Vacant Housing Units: 129,823 (9.9%)

---

**👤 You:**
> "Use a custom query to find the renter to ownership ratio in Ohio"

**🤖 AI Agent:**
> 📊 **Census: B25003_002E,B25003_003E for state:39**

**Ohio (39):**
- Owner-Occupied: 3,241,180 (67.1%)
- Renter-Occupied: 1,589,455 (32.9%)


## Installation & Usage

To install and use the **U.S. Census Housing — Home Values, Rent & Real Estate Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-census-housing-home-values-rent-real-estate-data](https://vinkius.com/mcp/us-census-housing-home-values-rent-real-estate-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
