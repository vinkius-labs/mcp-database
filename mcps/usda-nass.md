# USDA NASS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/usda-nass)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access US agricultural statistics via USDA NASS — query crop yields, livestock data, farm economics and demographics from any AI agent.

## Description
Connect to **USDA NASS** (National Agricultural Statistics Service) APIs through any AI agent and explore American agriculture data through natural conversation.

### What you can do

- **Crop Production** — Query yield, production, harvested acres and price data for all major crops (corn, soybeans, wheat, cotton, rice)
- **Livestock Data** — Retrieve cattle inventory, hog production, poultry statistics, milk and egg production data
- **Agricultural Economics** — Access prices received/paid by farmers, farm income, production expenses and land values
- **Farm Demographics** — Explore Census of Agriculture data including operator age, experience, occupation and veteran status
- **Parameter Discovery** — Discover valid values for any filter parameter (commodities, states, years, units)
- **Survey Metadata** — Review information about all NASS surveys including frequencies and methodologies

### How it works

1. Subscribe to this server
2. Enter your USDA NASS API Key (free at nass.usda.gov/developer)
3. Start exploring agricultural data from Claude, Cursor, or any MCP-compatible client

No more navigating complex Quick Stats interfaces to find crop yields or livestock data. Your AI acts as a dedicated agricultural data analyst.

### Who is this for?

- **Agricultural Analysts** — quickly query crop production data, compare yields across states and track price trends
- **Farmers & Ranchers** — check market prices, review production statistics and benchmark against state/national averages
- **Researchers** — access demographics data, survey methodologies and historical agricultural statistics for academic work
- **Commodity Traders** — monitor production volumes, inventory levels and economic indicators for market analysis


## Available Tools
- **get_survey_info**: This is useful for understanding what data is available and how frequently it is collected.

Get information about USDA NASS surveys
- **search_by_commodity**: Optionally filter by state, year and sector. This is a broad search that returns all available data for the commodity, including production, price, inventory and acreage statistics.

Search Quick Stats by commodity name
- **get_crop_summary**: Requires a commodity name (e.g. CORN, SOYBEANS, WHEAT, COTTON). Optionally filter by state and year. Returns detailed statistics with units, geographic scope and time period.

Get crop production summary from USDA NASS
- **get_demographics_data**: Optionally filter by state and year. Sector is automatically set to DEMOGRAPHICS.

Get farm demographics data from USDA NASS
- **get_economics_data**: Optionally filter by commodity, state and year. Sector is automatically set to ECONOMICS.

Get agricultural economics data from USDA NASS
- **get_livestock_summary**: Requires a commodity name (e.g. CATTLE, HOGS, CHICKENS, MILK, EGGS). Optionally filter by state and year.

Get livestock production summary from USDA NASS
- **get_param_values**: Parameters include: sector, group, commodity, commodity_desc, short_desc, source_desc, util_desc, unit_desc, freq_desc, domain_desc, state, county. Use this to discover what values you can filter by before making queries.

Get valid values for a Quick Stats parameter
- **get_quick_stats**: Accepts parameters: sector (CROPS, ANIMALS & PRODUCTS, ECONOMICS, DEMOGRAPHICS), commodity, group, commodity_desc, state, year, freq (ANNUAL, MONTHLY), unit_desc, source_desc. Returns statistical data with value, unit, state, year and commodity information. Use get_param_values to discover valid parameter values before querying.

Query USDA NASS Quick Stats database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **USDA NASS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the corn production summary for Iowa in 2024."

**🤖 AI Agent:**
> Iowa corn production in 2024: 2,480 million bushels produced from 12.8 million harvested acres, with an average yield of 193.8 bushels/acre. The average price received by farmers was $4.45/bushel. Iowa remains the #1 corn-producing state in the US.

---

**👤 You:**
> "What are the current cattle inventory numbers for Texas?"

**🤖 AI Agent:**
> Texas cattle inventory (Jan 2024): Total cattle and calves at 13.5 million head (down 2% from 2023). Beef cows: 4.1 million, Milk cows: 0.58 million, Other cattle: 8.82 million. Texas remains the #2 cattle state after Montana.

---

**👤 You:**
> "Show me what commodity values are available for filtering."

**🤖 AI Agent:**
> Available commodities include: CORN, SOYBEANS, WHEAT, COTTON, RICE, SORGHUM, OATS, BARLEY, HAY, PEANUTS, POTATOES, SUGARCANE, SUNFLOWER, CATTLE, HOGS, CHICKENS, TURKEYS, MILK, EGGS, HONEY, WOOL and 200+ more. Use `get_param_values` with any parameter to see the complete list.


## ❓ FAQ

**Q: How do I get a USDA NASS API key?**
Visit [**nass.usda.gov/developer**](https://www.nass.usda.gov/developer/index.php) and register for a free API key. The key is delivered instantly via the web form. It's completely free with no usage cost.

**Q: What crops and commodities are available?**
The NASS Quick Stats database covers all major US agricultural commodities: CORN, SOYBEANS, WHEAT, COTTON, RICE, SORGHUM, OATS, BARLEY, HAY, PEANUTS, POTATOES for crops; CATTLE, HOGS, CHICKENS, TURKEYS, MILK, EGGS, HONEY for livestock; plus fruit, vegetables, nursery products and many more. Use `get_param_values` with param 'commodity' to see the complete list.

**Q: Can I filter data by state and year?**
Yes! All query tools support optional state and year parameters. State can be the full name (e.g. 'IOWA') or abbreviation (e.g. 'IA'). Year accepts specific years (e.g. '2024') or ranges. The data returned includes the state, year, commodity, value and unit for each record.

**Q: What kind of economic data is available?**
The ECONOMICS sector includes: prices received by farmers for crops and livestock, prices paid by farmers (inputs, feed, fuel), farm production expenses, farm real estate values, cash rent for cropland and pasture, and agricultural income data. Use `get_economics_data` to query by commodity, state and year.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/usda-nass](https://vinkius.com/mcp/usda-nass)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **USDA NASS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `usda-nass` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **USDA NASS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "usda-nass": {
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
