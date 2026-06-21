# Ember Climate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ember-climate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access global electricity data — generation, demand, emissions, and capacity from Ember Climate's open energy API.

## Description
Connect your AI agents to **Ember Climate's** open electricity dataset and gain instant access to global energy intelligence covering over 200 countries and regions.

### What you can do

- **Carbon Intensity Analysis** — Track yearly and monthly carbon footprint (gCO2/kWh) of electricity grids worldwide
- **Generation by Source** — Break down electricity production by energy type: coal, gas, nuclear, wind, solar, hydro, and more
- **Demand Trends** — Analyze electricity consumption patterns in TWh with per-capita metrics across nations
- **Power Sector Emissions** — Monitor CO2 emissions from the power sector in megatonnes and percentage shares
- **Renewable Capacity Tracking** — Follow monthly wind and solar capacity installations in GW to measure clean energy deployment
- **Multi-Country Comparison** — Query multiple nations simultaneously using comma-separated country codes for comparative analysis
- **Filter Discovery** — Explore available entities, energy sources, and date ranges dynamically before making targeted queries

### How it works

1. Subscribe to this server
2. Enter your Ember Climate API Key (free, obtained via email signup)
3. Start querying global electricity data from Claude, Cursor, or any MCP-compatible client

No more manual CSV downloads or spreadsheet wrangling. Your AI becomes an instant energy analyst, capable of answering complex questions about the global energy transition in seconds.

### Who is this for?

- **Climate Researchers** — instantly retrieve emissions data and grid carbon intensity trends without writing data pipelines
- **Energy Consultants** — compare generation mixes across countries and track renewable adoption rates programmatically
- **Sustainability Teams** — monitor power sector decarbonization progress and contextualize corporate ESG goals against national benchmarks
- **Policy Makers & Journalists** — fact-check energy claims with authoritative data from over 200 geographies on demand


## Available Tools
- **get_carbon_intensity_monthly**: Use entity or entity_code to filter by country (e.g., "Brazil", "DE", "US"). Use start_date and end_date with format YYYY-MM (e.g., "2023-01", "2024-12"). This helps analyze seasonal patterns in grid carbon footprint and track monthly decarbonization progress.

Get monthly carbon intensity of electricity generation for countries/regions
- **get_carbon_intensity_yearly**: Use entity or entity_code to filter by country (e.g., "Brazil", "DE", "US"). Use start_date and end_date with format YYYY (e.g., "2020", "2023"). Returns emissions intensity data showing how clean or polluting the electricity grid is over time.

Get yearly carbon intensity of electricity generation for countries/regions
- **get_electricity_demand_monthly**: Use entity or entity_code to filter by country (e.g., "Brazil", "DE", "US"). Use start_date and end_date with format YYYY-MM (e.g., "2023-01", "2024-12"). Useful for analyzing seasonal demand patterns, peak consumption periods, and demand forecasting.

Get monthly electricity demand data for countries/regions
- **get_electricity_demand_yearly**: Use entity or entity_code to specify countries (e.g., "Brazil", "DE", "US"). Use start_date and end_date with format YYYY (e.g., "2020", "2023"). Essential for understanding energy consumption trends and comparing per-capita usage across nations.

Get yearly electricity demand data for countries/regions
- **get_electricity_generation_monthly**: ). Returns generation in TWh and percentage share of total generation for each source. Use entity or entity_code to filter by country (e.g., "Brazil", "DE", "US"). Use start_date and end_date with format YYYY-MM (e.g., "2023-01", "2024-12"). Use series to filter by specific energy sources (e.g., "coal", "wind", "solar", "hydro", "nuclear", "gas"). Perfect for analyzing seasonal generation patterns, renewable intermittency, and monthly energy mix changes.

Get monthly electricity generation by source for countries/regions
- **get_electricity_generation_yearly**: ). Returns generation in TWh and percentage share of total generation for each source. Use entity or entity_code to filter by country (e.g., "Brazil", "DE", "US"). Use start_date and end_date with format YYYY (e.g., "2020", "2023"). Use series to filter by specific energy sources (e.g., "coal", "wind", "solar", "hydro", "nuclear", "gas"). Essential for analyzing energy transition, renewable adoption, and fossil fuel phase-out progress.

Get yearly electricity generation by source for countries/regions
- **get_generation_multi_entity**: g., "BRA,DE,US" for Brazil, Germany, and United States). Use start_date and end_date with format YYYY for yearly or YYYY-MM for monthly data. Use series to filter by energy source (e.g., "coal", "wind", "solar", "hydro", "nuclear", "gas"). This is highly efficient for comparative analysis across multiple nations without making separate API calls. Example: entity_code="BRA,DE,US,CHN,IND" to compare BRICS+ nations energy generation.

Get electricity generation data for multiple countries simultaneously
- **get_installed_capacity_monthly**: Use entity or entity_code to filter by country (e.g., "Brazil", "DE", "US"). Use start_date and end_date with format YYYY-MM (e.g., "2023-01", "2024-12"). Use series to filter by capacity type (e.g., "wind", "solar"). Tracks renewable infrastructure deployment and capacity growth over time across different nations.

Get monthly installed power capacity (wind and solar) for countries
- **get_api_options**: Use dataset (e.g., "electricity-generation"), temporal_resolution (e.g., "monthly", "yearly"), and filter_name (e.g., "entity", "series", "entity_code", "date", "year"). This tool is useful for discovering valid country codes, energy source types, and available date ranges before making specific data queries.

Get available filter options for Ember electricity datasets
- **get_power_sector_emissions_monthly**: Use entity or entity_code to filter by country (e.g., "Brazil", "DE", "US"). Use start_date and end_date with format YYYY-MM (e.g., "2023-01", "2024-12"). Use series parameter to filter by emission types (e.g., "co2"). Enables granular tracking of monthly emission trends and seasonal variations in power sector pollution.

Get monthly power sector CO2 emissions for countries/regions
- **get_power_sector_emissions_yearly**: Use entity or entity_code to filter by country (e.g., "Brazil", "DE", "US"). Use start_date and end_date with format YYYY (e.g., "2020", "2023"). Use series parameter to filter by emission types (e.g., "co2"). Critical for tracking national decarbonization progress and climate policy effectiveness.

Get yearly power sector CO2 emissions for countries/regions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ember Climate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the carbon intensity of Brazil's electricity grid in recent years?"

**🤖 AI Agent:**
> Fetching carbon intensity data for Brazil... The Brazilian grid shows an intensity of approximately 85 gCO2/kWh in 2023, which is significantly lower than the global average. This is due to Brazil's heavy reliance on hydropower and growing wind/solar capacity.

---

**👤 You:**
> "Compare wind and solar generation between Germany, China, and the US for the last 3 years."

**🤖 AI Agent:**
> Running multi-entity comparison I've fetched wind and solar generation data for DEU, CHN, and USA from 2021 to 2023. China leads with over 1,000 TWh of combined wind+solar in 2023, followed by the US at ~600 TWh and Germany at ~350 TWh. All three show strong double-digit growth rates year over year.

---

**👤 You:**
> "Show me the monthly electricity demand in France during 2024."

**🤖 AI Agent:**
> Fetching monthly demand data for France in 2024... Peak demand occurred in January and December (winter heating season) at around 55-60 TWh per month, while summer months like July and August dropped to approximately 35-40 TWh, reflecting strong seasonal variation.


## ❓ FAQ

**Q: How do I get an Ember Climate API key and how long does it take?**
Simply visit the [Ember Climate API page](https://ember-energy.org/data/api/), enter your email address, and click to request your key. You'll receive it via email almost instantly. It only takes 30 seconds — no OAuth apps to configure, no developer portals to navigate, no complex setup.

**Q: What countries and regions are covered by the Ember electricity dataset?**
The dataset covers over 200 countries and geographical regions worldwide, including individual nations, continents (like Europe), and regional aggregates (like OECD, EU-27). You can use the `get_api_options` tool to discover all available entity codes and country names before querying specific data.

**Q: Can I compare electricity generation across multiple countries in a single query?**
Yes! Use the `get_generation_multi_entity` tool and provide comma-separated ISO country codes in the `entity_code` parameter (e.g., "BRA,DE,US,CHN" for Brazil, Germany, USA, and China). This is highly efficient for comparative energy analysis without making multiple separate API calls.

**Q: What energy sources can I filter by when querying electricity generation?**
You can filter by all major energy sources including fossil fuels (coal, gas, oil), renewables (wind, solar, hydro, bioenergy, geothermal), nuclear, and storage. Use the `series` parameter with values like "coal", "wind", "solar", "hydro", "nuclear", "gas". Call `get_api_options` with filter_name="series" to see the complete list of available energy types for any dataset.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ember-climate](https://vinkius.com/mcp/ember-climate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ember Climate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ember-climate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ember Climate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ember-climate": {
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
