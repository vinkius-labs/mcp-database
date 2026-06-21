# U.S. Census Full — Complete Demographic & Economic Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-census-full-complete-demographic-economic-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/us-census-full-complete-demographic-economic-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/us-census-full-complete-demographic-economic-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

The U.S. Census Mega-Server: 14 tools providing comprehensive access to the ACS and County Business Patterns. Analyze population, age, race, income, poverty, education, home values, rent, and businesses across all 50 states, 3,000+ counties, and cities.

## Description
The **ultimate U.S. Census Mega-Server** — 14 tools.

### 14 Tools
- 👥 Population (5) — State, county, city, demographics
- 💰 Income (4) — Income, poverty, education, businesses
- 🏘️ Housing (5) — Values, rent, ownership, full profiles, generic query

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
- **get_income_by_state**: Median income is the single most-used economic indicator from the Census — it determines federal funding, cost-of-living adjustments, and market opportunity analysis.

Get median household income and poverty rates for all states
- **get_income_by_county**: Critical for real estate analysis, business site selection, and understanding economic disparity within a state.

Get median household income and poverty for all counties in a state
- **get_education_by_state**: Education level is a key predictor of income, employment, and economic development.

Get educational attainment for all states — bachelor's degree or higher
- **get_business_patterns**: From County Business Patterns (CBP) — the definitive dataset for understanding local economic activity and business concentration.

Get County Business Patterns — establishments, employees, and payroll by county
- **get_population_by_state**: The ACS is the most comprehensive demographic survey in the U.S., sampling 3.5 million households annually.

Get total population and median age for all 50 U.S. states + DC
- **get_population_by_county**: Use state FIPS codes: CA=06, TX=48, NY=36, FL=12, IL=17, PA=42, OH=39, GA=13, NC=37, MI=26, etc.

Get population and median age for all counties in a state
- **get_population_by_city**: This includes incorporated cities and Census Designated Places.

Get population for all cities/towns/places within a state
- **get_demographics_by_state**: Essential for diversity analysis, market segmentation, and policy research.

Get racial and ethnic demographics for all states — White, Black, Asian, Hispanic, foreign-born
- **get_demographics_by_county**: Get racial and ethnic demographics for all counties in a state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **U.S. Census Full — Complete Demographic & Economic Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a complete socioeconomic profile for Los Angeles County (037) in California (06)"

**🤖 AI Agent:**
> 📊 **U.S. Census Bureau: County Profile: 06-037**

**Los Angeles County, California:**
- Population: 9,936,690
- Median Household Income: $78,671
- Median Home Value: $692,800
- Median Gross Rent: $1,754
- Poverty Rate: 13.9%
- Hispanic/Latino: 4,834,166 (48.6%)
- Foreign Born: 3,365,064 (33.8%)

---

**👤 You:**
> "Which state has the lowest median age?"

**🤖 AI Agent:**
> 📊 **Population by State**

The state with the lowest median age is:
**Utah (49)**
- Median Age: 31.4 years
- Total Population: 3,337,975

---

**👤 You:**
> "Correlate rent prices with Bachelor Degree holders nationwide"

**🤖 AI Agent:**
> 📊 **Analysis: Rent Prices vs. Education Levels**

- Massachusetts: Median Rent $1,469 | Bachelor's or Higher 44.5%
- Colorado: Median Rent $1,594 | Bachelor's or Higher 42.8%
- Mississippi: Median Rent $860 | Bachelor's or Higher 23.2%
There is a strong positive correlation between the percentage of the population holding a Bachelor's degree and the state's median rent.


## Installation & Usage

To install and use the **U.S. Census Full — Complete Demographic & Economic Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-census-full-complete-demographic-economic-intelligence](https://vinkius.com/mcp/us-census-full-complete-demographic-economic-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
