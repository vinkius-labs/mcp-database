# PropertyData MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/propertydata)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Access comprehensive UK property market data, valuations, and building analytics directly from your AI agent.

## Description
Connect **PropertyData** to your AI agent to unlock professional-grade UK real estate insights. This server allows you to query live market prices, historical growth, and detailed building information using postcodes, UPRNs, or coordinates.

### What you can do

- **Address & Identity** — Match addresses to UPRNs, lookup title numbers, and find all properties within a specific postcode area.
- **Market Analytics** — Retrieve live asking prices, sold prices, and price-per-square-foot data for any UK location.
- **Investment Insights** — Analyze capital growth over 7 years, local sales demand, and national economic indicators.
- **Building Intelligence** — Estimate rebuild costs, check energy efficiency (EPC) ratings, and calculate internal floor areas.
- **Valuations** — Generate instant sale valuations or historical valuations for specific dates in the past.

### How it works

1. Subscribe to this server
2. Enter your PropertyData API Key
3. Start analyzing UK property data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Property Investors** — Quickly evaluate potential deals by checking local growth and demand metrics.
- **Developers** — Analyze building plots and estimate rebuild costs without leaving your workflow.
- **Real Estate Professionals** — Generate instant valuations and floor area reports for client properties.


## Available Tools (68)
- **account_credits**: API account credits used/remaining
- **account_documents**: Summary of previous document purchases
- **address_match_uprn**: Match an address to its closest UPRN
- **agents**: Local estate agent market share
- **analyse_buildings**: Analyse buildings on a title plot
- **aonb**: Check if a location is within an AONB
- **area_type**: Determine area type (e.g., rural or urban)
- **build_cost**: Calculate building costs for construction
- **conservation_area**: Check if a postcode is within a conservation area
- **council_tax**: Average council tax bills in an area
- **crime**: Analytics data on local crime
- **demand**: Determine local property sales demand
- **demand_rent**: Determine local property rental demand
- **demographics**: Local population demographics
- **development_calculator**: Calculate potential profit for a development
- **development_gdv**: Estimate gross development value
- **energy_efficiency**: Find EPC ratings for property within a postcode
- **flood_risk**: Risk of flooding from rivers/sea
- **floor_areas**: Known internal floor areas for a full UK postcode
- **freeholds**: Local freehold titles with headline info
- **george**: AI-powered property research assistant
- **green_belt**: Check if a postcode is within the green belt
- **growth**: Up to 7-year capital growth
- **growth_psf**: Up to 7-year growth per square foot
- **household_income**: Average household income for an area
- **internet_speed**: Internet speeds for a postcode
- **land_registry_documents**: Purchase Land Registry documents
- **lha_rate**: The LHA rate for a given postcode / property size
- **listed_buildings**: Local listed buildings
- **mortgage_calculator**: Calculate monthly mortgage payments
- **mortgage_rates**: Average mortgage interest rates
- **national_data**: National property market data and economic indicators
- **national_hmo_register**: Search the national register of HMOs
- **national_park**: Check if a postcode is within a national park
- **planning_applications**: Local planning applications
- **politics**: Constituency information and recent results
- **population**: Population, household, and density information
- **postcode_key_stats**: Key stats for all postcode districts in a region
- **prices**: Live local asking prices
- **prices_per_sqf**: Live local asking £/sqft
- **property_types**: ONS breakdown of local property stock by type
- **ptal**: PTAL score (Greater London only)
- **rebuild_cost**: Estimate the approximate rebuild cost of a house
- **rents**: Live local long-let asking rents
- **rents_commercial**: Commercial property quoting rents
- **rents_hmo**: Live local HMO asking rents
- **restaurants**: Nearby restaurants
- **schools**: Nearby schools
- **site_plan_documents**: Purchase A4 scale site plans
- **sold_prices**: Local property sold prices
- **sold_prices_per_sqf**: Local property sold £/sqft
- **sourced_properties**: Properties from a sourcing list
- **sourced_property**: Information relating to a specific sourced property
- **stamp_duty_calculator**: SDLT payable on a property transaction
- **tenure_types**: ONS breakdown of local property stock by tenure
- **title**: Address, type, and ownership information by title number
- **title_use_class**: Predicted planning use class
- **titles_by_company**: Search land titles by company ownership
- **uprn**: Property information from UPRN
- **uprn_title**: Lookup a title number from a UPRN
- **uprns**: Find UPRNs in a given postcode area
- **valuation_commercial_rent**: Rental valuation for a commercial property
- **valuation_commercial_sale**: Sale valuation for a commercial property
- **valuation_historical**: Estimate the value of a property on a date in the past
- **valuation_hmo**: Sale and gross rental valuations for an HMO
- **valuation_rent**: Rental valuation for a property
- **valuation_sale**: Sale valuation for a property
- **yields**: Determine local rental yields


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PropertyData** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the average asking prices in the postcode area OX1?"

**🤖 AI Agent:**
> I've analyzed the OX1 area. The current average asking price is £545,000, with detached houses averaging £820,000 and flats around £350,000. Would you like to see the price per square foot for this area as well?

---

**👤 You:**
> "Find the UPRN for '10 Downing Street, London' and tell me its energy efficiency rating."

**🤖 AI Agent:**
> The UPRN for 10 Downing Street is 100023336951. According to the latest EPC data, the property has an energy efficiency rating of D. I can also fetch the floor area or title number if needed.

---

**👤 You:**
> "Analyze the capital growth in Manchester over the last 5 years."

**🤖 AI Agent:**
> In Manchester, capital growth has been strong, showing a cumulative increase of approximately 28.5% over the last 5 years. The highest growth was seen in the M1 and M4 postcodes. Would you like a breakdown of the current sales demand in those specific areas?


## ❓ FAQ

**Q: How can I find the unique identifier (UPRN) for a specific UK address?**
You can use the `pdAddressMatchUprn` tool. Simply provide the full address string, and the agent will return the closest matching UPRN along with property details.

**Q: Can the AI estimate how much it would cost to rebuild a specific house?**
Yes, by using the `pdRebuildCost` tool. You can provide a postcode or coordinates along with optional parameters like internal area, wall type, and roof type to get an approximate rebuild estimate.

**Q: Is it possible to see the historical capital growth of an area?**
Absolutely. Use the `pdGrowth` tool with a postcode or town name to retrieve up to 7 years of capital growth data for that specific UK location.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/propertydata](https://vinkius.com/mcp/propertydata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PropertyData** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `propertydata` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PropertyData** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "propertydata": {
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
