# OpenEI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openei)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/openei-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/openei-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

US electricity rate intelligence — query utility rates by location, sector, and tariff via AI for solar and energy analysis.

## Description
Access the **National Utility Rate Database** through **OpenEI** — the most comprehensive source for US electricity rate data maintained by the Department of Energy. Connect OpenEI to your AI agent to instantly query utility rates by address or coordinates, analyze rate structures across residential, commercial, and industrial sectors, retrieve complete tariff details including time-of-use periods and demand charges — all through natural conversation.

### What you can do

- **Location-Based Rate Lookup** — Find all applicable utility rates by providing a street address or GPS coordinates.
- **Sector-Specific Rates** — Query residential, commercial, or industrial electricity rates separately.
- **Complete Tariff Analysis** — Retrieve full rate structures including time-of-use periods, seasonal variations, demand charges, and energy charges.
- **Utility Company Research** — Search and browse US electric utilities, get company details and service territories.
- **Solar Feasibility Studies** — Instant rate quotes for solar ROI calculations and net metering analysis.
- **Energy Cost Modeling** — Access detailed rate structures for accurate energy cost projections.
- **Demand Charge Analysis** — Understand demand charges for commercial and industrial facilities.
- **Rate Comparison** — Compare rate options across different utilities and locations.

### How it works

1. Subscribe to this server
2. Enter your OpenEI API Key
3. Start querying electricity rates through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Solar Installers** — instant rate quotes for customer proposals and ROI calculations.
- **Energy Consultants** — detailed rate structures for energy cost modeling and feasibility studies.
- **Facility Managers** — compare rates across locations for site selection and budget planning.
- **Researchers** — access comprehensive US electricity rate data for academic and policy analysis.


## Available Tools
- **get_commercial_rates**: Use lat/lon or address to identify the location. Returns all available commercial tariffs including general service, large power, and time-of-use rates. Essential for commercial solar installations, demand response analysis, and business energy cost modeling.

Get commercial electricity rates for a location
- **get_industrial_rates**: Industrial rates typically include the lowest per-kWh costs but may have complex demand charges and power factor adjustments. Use for heavy manufacturing energy cost analysis, load forecasting, and industrial facility site selection.

Get industrial electricity rates for a location
- **get_rate_detail**: Returns the full rate structure including energy charges, demand charges, fixed charges, minimum charges, time-of-use periods, seasonal variations, and applicable taxes. Use this after identifying a rate ID from get_utility_rates to get exhaustive details for cost modeling or bill analysis.

Get detailed information about a specific utility rate/tariff
- **get_utility_rates**: Provide either latitude/longitude coordinates or a physical address to find applicable utility rates. Filter by sector (residential, commercial, industrial) to get specific rate types. Use detail=full to retrieve complete rate structures including time-of-use periods, seasonal variations, demand charges, and energy charges. This is essential for solar analysis, energy cost modeling, and economic feasibility studies. Sector values: 1=Residential, 2=Commercial, 3=Industrial.

Get utility rate information for a specific location
- **get_rates_by_address**: Simply provide a street address and the API will geocode it and identify the serving utility and applicable rates. Perfect for solar installers providing instant rate quotes to customers, or homeowners checking their electricity rates. Returns all available rate options at that address.

Get utility rates for a specific street address
- **get_rates_by_coordinates**: Automatically identifies the serving utility for that location and returns applicable rates. Essential for solar installers, energy consultants, and site selection analysis. Returns residential, commercial, and industrial rates if available. Set detail=full for complete rate structures.

Get utility rates for a location using GPS coordinates
- **get_residential_rates**: Perfect for homeowners comparing electricity costs, evaluating solar ROI, or understanding time-of-use rate options. Returns all residential tariffs including tiered rates, time-of-use plans, and electric vehicle charging rates.

Get residential electricity rates for a location
- **get_utility_detail**: Returns the utility name, address, contact information, service territory, owned generation resources, and associated rates. Use this to research utility companies, understand their generation mix, or identify all rates offered by a specific utility.

Get detailed information about a specific utility company
- **list_utilities**: Filter by state, country, or utility name to find specific companies. Returns utility names, addresses, company IDs, and service territories. Use this to identify utility companies for research or to get company IDs for further queries. Use limit and offset for pagination through large result sets.

List electric utility companies in the OpenEI database
- **search_utilities_by_name**: Useful for finding the correct utility when you know part of the company name but not the ID. Returns matching utilities with their IDs, addresses, and service areas. Use the returned IDs for detailed queries.

Search for utility companies by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenEI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the residential electricity rates at 1617 Cole Blvd, Golden, CO?"

**🤖 AI Agent:**
> I found 5 residential rate options at that address served by Xcel Energy. The standard residential rate is $0.142/kWh with a tiered structure. There's also a time-of-use plan with peak hours at $0.198/kWh and off-peak at $0.089/kWh. Here are the complete rate details.

---

**👤 You:**
> "Show me all utilities in California and their average commercial rates."

**🤖 AI Agent:**
> I found 127 utilities in California. The largest include PG&E (avg $0.231/kWh), SCE (avg $0.218/kWh), and SDG&E (avg $0.267/kWh). California has some of the highest electricity rates in the US. Here's the complete list with rate averages.

---

**👤 You:**
> "Get the complete rate structure for commercial time-of-use rates from PG&E."

**🤖 AI Agent:**
> I retrieved the complete PG&E E-19 commercial time-of-use rate structure. It has 4 seasonal periods (Summer Peak, Summer Off-Peak, Winter Peak, Winter Off-Peak) with energy charges ranging from $0.147 to $0.326/kWh. Demand charges are $18.76/kW in summer and $12.54/kW in winter. Here's the full breakdown.


## Installation & Usage

To install and use the **OpenEI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openei](https://vinkius.com/mcp/openei)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
