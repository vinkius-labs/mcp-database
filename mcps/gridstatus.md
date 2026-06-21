# GridStatus MCP Server

Access real-time and historical US electricity grid data — load, fuel mix, LMP pricing, and generation across all major ISOs (ERCOT, CAISO, PJM, MISO, NYISO, ISO-NE, SPP).

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gridstatus)

## Overview
**Category:** the-unthinkable
**Tools Count:** 12

## Description
Connect to **GridStatus.io API** and bring comprehensive US electricity market intelligence to any AI agent. Monitor all major Independent System Operators (ISOs), track renewable energy transition, analyze wholesale prices, and understand grid dynamics across America.

### What you can do

- **Electricity Load/Demand** — Retrieve real-time and historical electricity consumption data (MW) for any US ISO region
- **Fuel Mix & Generation** — Get breakdown of power generation by source (coal, natural gas, nuclear, solar, wind, hydro) to understand the energy mix
- **Day-Ahead LMP Pricing** — Access hourly Locational Marginal Pricing forecasts for specific nodes and trading hubs across ISOs
- **Real-Time 5-Minute LMP** — Track live wholesale electricity prices at 5-minute intervals to identify price spikes and volatility
- **ERCOT SPP Data** — Query Settlement Point Prices for Texas grid including day-ahead hourly and real-time 15-minute intervals at trading hubs
- **Standardized Zonal Data** — Fetch consistently formatted hourly data with regional/zonal breakdowns for modeling and analysis
- **Capacity Markets** — Monitor capacity commitments and resource adequacy data for long-term planning
- **Dataset Exploration** — List all available datasets, check metadata including coverage dates and available columns
- **API Usage Tracking** — Monitor your API quota usage, row counts, and rate limits
- **Custom Dataset Queries** — Query any dataset with advanced filtering, resampling, and aggregation controls
- **Multi-ISO Coverage** — Access data from ERCOT (Texas), CAISO (California), PJM (Mid-Atlantic), MISO (Midwest), NYISO (New York), ISO-NE (New England), and SPP (Southwest)

### How it works

1. Subscribe to this server
2. Enter your GridStatus API key (free tier available with 500K rows/month)
3. Start querying US electricity data from Claude, Cursor, or any MCP-compatible client

Your AI becomes a US energy analyst, helping you understand grid operations, track renewable adoption, and make data-driven energy decisions.

### Who is this for?

- **Energy Traders** — monitor real-time LMP/SPP prices, identify arbitrage opportunities across nodes and time periods
- **Renewable Developers** — track solar and wind generation growth, understand fuel mix evolution across regions
- **Researchers & Academics** — access granular 5-minute and hourly data for energy studies, modeling, and publications
- **Corporate Sustainability Teams** — monitor regional renewable availability to optimize facility siting and procurement
- **Policy Makers & Advocates** — track state-by-state energy transition progress, fossil fuel dependency, and grid reliability
- **Homeowners & Consumers** — understand when electricity is cheapest or cleanest in your ISO region


## Available Tools
- **get_api_usage**: Shows how many rows you've queried and your remaining allowance.

USE WHEN:
- User asks about their API usage or quota
- User wants to check how many rows they have remaining
- User needs to verify their rate limits
- User asks about their GridStatus account status

EXAMPLES:
- "How much API quota do I have left?" → call with no params
- "Check my API usage this month" → call with no params
- "Show my rate limits" → call with no params

Get API usage statistics and rate limits for your GridStatus account
- **get_capacity_data**: This data is used to track long-term resource adequacy and capacity commitments.

USE WHEN:
- User asks about generation capacity or capacity markets
- User needs capacity commitment data for an ISO
- User wants to track resource adequacy metrics
- User asks about capacity prices or availability

SUPPORTED ISOs:
- pjm (primary capacity market), others may be available

PARAMETERS:
- iso (REQUIRED): ISO identifier
- start (OPTIONAL): Start date
- end (OPTIONAL): End date
- limit (OPTIONAL): Maximum rows

EXAMPLES:
- "PJM capacity data for next month" → call with iso="pjm", start="2026-05-01"
- "Show capacity commitments" → call with iso="pjm"

Get capacity market data for a US ISO
- **get_dataset_metadata**: USE WHEN:
- User wants to know the date range covered by a dataset
- User needs to see what columns are available in a dataset
- User asks about data frequency or schema for a specific dataset
- User is validating if a dataset exists before querying

PARAMETERS:
- dataset_id (REQUIRED): Dataset identifier (e.g. "pjm_load", "ercot_fuel_mix", "caiso_lmp_day_ahead_hourly")

EXAMPLES:
- "Show metadata for PJM load dataset" → call with dataset_id="pjm_load"
- "What columns are in ERCOT fuel mix?" → call with dataset_id="ercot_fuel_mix"
- "Date range for CAISO LMP" → call with dataset_id="caiso_lmp_day_ahead_hourly"

Get metadata for a specific GridStatus dataset
- **get_fuel_mix**: ) for any supported US ISO. Essential for understanding where electricity comes from and tracking the renewable energy transition.

USE WHEN:
- User asks about the energy mix or generation breakdown
- User wants to know how much power comes from solar, wind, coal, etc.
- User asks about renewable energy percentage
- User needs to compare fossil vs clean energy generation

SUPPORTED ISOs WITH FUEL MIX:
- ercot (Texas), caiso (California), isone (New England)

PARAMETERS:
- iso (REQUIRED): ISO identifier: ercot, caiso, or isone
- start (OPTIONAL): Start date
- end (OPTIONAL): End date
- limit (OPTIONAL): Maximum rows
- timezone (OPTIONAL): Timezone for results

EXAMPLES:
- "What is Texas energy mix right now?" → call with iso="ercot", start="latest"
- "Show Californiaia renewable generation today" → call with iso="caiso", start="2026-04-07"
- "New England fuel mix this week" → call with iso="isone", start="2026-04-01", limit=168

Get electricity generation by fuel source (energy mix) for a US ISO
- **get_lmp_data**: LMP is measured in dollars per megawatt-hour ($/MWh).

USE WHEN:
- User asks about wholesale electricity prices at specific locations
- User needs day-ahead price forecasts for an ISO
- User wants to compare prices across different nodes
- User asks about LMP or nodal pricing data

SUPPORTED ISOs WITH LMP:
- pjm (Mid-Atlantic), caiso (California), miso (Midwest), nyiso (New York), isone (New England), spp (Southwest)

PARAMETERS:
- iso (REQUIRED): ISO identifier: pjm, caiso, miso, nyiso, isone, or spp
- start (OPTIONAL): Start date
- end (OPTIONAL): End date
- limit (OPTIONAL): Maximum rows
- timezone (OPTIONAL): Timezone for results
- filter_column (OPTIONAL): Column to filter on (e.g. "location")
- filter_value (OPTIONAL): Value to filter by

EXAMPLES:
- "Show PJM day-ahead LMP for tomorrow" → call with iso="pjm", start="2026-04-08"
- "CAISO LMP at SP15 node today" → call with iso="caiso", start="2026-04-07", filter_column="location", filter_value="SP15"
- "MISO hourly prices this week" → call with iso="miso", start="2026-04-01", limit=168

Get day-ahead Locational Marginal Pricing (LMP) data for a US ISO
- **list_datasets**: Shows dataset identifiers, coverage dates, and available columns.

USE WHEN:
- User wants to explore what data is available in GridStatus
- User needs to find dataset identifiers for querying
- User is exploring the API capabilities for the first time
- User asks what ISOs and data types are supported

SUPPORTED ISOS:
- ERCOT (Texas), CAISO (California), PJM (Mid-Atlantic/Midwest)
- MISO (Midwest), NYISO (New York), ISO-NE (New England), SPP (Southwest)

DATASET TYPES:
- load (electricity demand), fuel_mix (generation by source)
- lmp (locational marginal pricing), spp (settlement point prices)
- capacity, standardized data

EXAMPLES:
- "What datasets are available?" → call with no params
- "Show me all dataset identifiers" → call with no params
- "List all supported ISOs" → call with no params

List all available datasets in the GridStatus API
- **get_load_data**: Shows how much electricity is being consumed across the grid region.

USE WHEN:
- User asks about electricity demand or consumption for an ISO
- User needs load data for a specific time period
- User wants to compare load across different regions
- User asks how much electricity is being used in Texas, California, etc.

SUPPORTED ISOs:
- ercot (Texas), caiso (California), pjm (Mid-Atlantic), miso (Midwest)
- nyiso (New York), isone (New England), spp (Southwest)

PARAMETERS:
- iso (REQUIRED): ISO identifier (lowercase): ercot, caiso, pjm, miso, nyiso, isone, spp
- start (OPTIONAL): Start date in YYYY-MM-DD or ISO 8601 format
- end (OPTIONAL): End date in YYYY-MM-DD or ISO 8601 format
- limit (OPTIONAL): Maximum number of rows to return (default varies by plan)
- timezone (OPTIONAL): Timezone for results ("market" for ISO local time, or standard like "US/Eastern")

EXAMPLES:
- "What is current electricity demand in Texas?" → call with iso="ercot", start="latest"
- "Show PJM load for yesterday" → call with iso="pjm", start="2026-04-06", end="2026-04-07"
- "California load data this week" → call with iso="caiso", start="2026-04-01", limit=168

Get electricity load/demand data for a specific US ISO
- **query_dataset**: Use this when specific data needs are not covered by the specialized tools.

USE WHEN:
- User needs data from a specific dataset not covered by other tools
- User wants custom filtering or resampling
- User has a specific dataset identifier and needs flexible querying
- User needs advanced filter operators

PARAMETERS:
- dataset_id (REQUIRED): Full dataset identifier (e.g. "pjm_load", "ercot_fuel_mix")
- start (OPTIONAL): Start date
- end (OPTIONAL): End date
- limit (OPTIONAL): Maximum rows
- timezone (OPTIONAL): Timezone for results
- filter_column (OPTIONAL): Column name to filter on
- filter_value (OPTIONAL): Value to filter by
- filter_operator (OPTIONAL): Filter operator (=, !=, >, <, >=, <=, in)
- resample (OPTIONAL): Resampling interval (e.g. "1 hour", "1 day")
- resample_function (OPTIONAL): Aggregation function (mean, sum, min, max)

EXAMPLES:
- "Query pjm_load for last week" → call with dataset_id="pjm_load", start="2026-03-31", limit=168
- "ERCOT fuel mix resampled daily" → call with dataset_id="ercot_fuel_mix", start="2026-04-01", resample="1 day", resample_function="mean"
- "CAISO load filtered for SDGE zone" → call with dataset_id="caiso_load", start="2026-04-07", filter_column="location", filter_value="SDGE"

Query any GridStatus dataset with custom filters and parameters
- **get_realtime_lmp**: This is the most granular and up-to-date pricing data available.

USE WHEN:
- User asks about current/real-time electricity prices
- User needs 5-minute interval price data
- User wants to track price spikes or volatility in real-time
- User asks about live nodal pricing

SUPPORTED ISOs:
- pjm, caiso, miso, nyiso, isone, spp

PARAMETERS:
- iso (REQUIRED): ISO identifier
- start (OPTIONAL): Start date/time (use "latest" for most recent)
- end (OPTIONAL): End date/time
- limit (OPTIONAL): Maximum rows (recommended to limit real-time data)
- timezone (OPTIONAL): Timezone

EXAMPLES:
- "Current real-time LMP in PJM" → call with iso="pjm", start="latest", limit=12
- "CAISO 5-min prices right now" → call with iso="caiso", start="latest", limit=12
- "Last hour of real-time MISO prices" → call with iso="miso", start="latest", limit=12

Get real-time 5-minute LMP data for a US ISO
- **get_realtime_spp**: Shows the most current wholesale electricity prices at trading hubs and zones in the Texas grid.

USE WHEN:
- User asks about current/real-time Texas electricity prices
- User needs 15-minute interval SPP data for ERCOT
- User wants to track price spikes or negative pricing in Texas
- User asks about live ERCOT hub prices

PARAMETERS:
- start (OPTIONAL): Start date/time (use "latest" for most recent)
- end (OPTIONAL): End date/time
- limit (OPTIONAL): Maximum rows (recommended for real-time data)
- timezone (OPTIONAL): Timezone

EXAMPLES:
- "Current ERCOT SPP at Houston hub" → call with start="latest", limit=4, filter_column="Settlement Point", filter_value="HB_HOUSTON"
- "Last hour of Texas real-time prices" → call with start="latest", limit=4
- "ERCOT West hub prices today" → call with start="2026-04-07", filter_column="Settlement Point", filter_value="HB_WEST"

Get ERCOT real-time 15-minute Settlement Point Price (SPP) data
- **get_spp_data**: SPP is similar to LMP but specific to ERCOT's market design, showing prices at trading hubs, load zones, and resource zones.

USE WHEN:
- User asks about ERCOT electricity prices or SPP
- User needs day-ahead price forecasts for Texas
- User wants prices at specific ERCOT trading hubs (e.g. HB_HOUSTON, HB_NORTH, HB_WEST)
- User asks about Texas wholesale electricity market prices

PARAMETERS:
- start (OPTIONAL): Start date
- end (OPTIONAL): End date
- limit (OPTIONAL): Maximum rows
- timezone (OPTIONAL): Timezone (ERCOT uses US/Central)
- filter_column (OPTIONAL): Column to filter (e.g. "Settlement Point")
- filter_value (OPTIONAL): Hub/zone name to filter by

EXAMPLES:
- "ERCOT SPP for Houston hub tomorrow" → call with start="2026-04-08", filter_column="Settlement Point", filter_value="HB_HOUSTON"
- "Texas day-ahead prices today" → call with start="2026-04-07"
- "ERCOT SPP this week at North hub" → call with start="2026-04-01", filter_column="Settlement Point", filter_value="HB_NORTH"

Get ERCOT Settlement Point Price (SPP) day-ahead hourly data
- **get_standardized_data**: Useful for zonal/regional breakdowns of load, generation, or pricing with uniform schema across time periods.

USE WHEN:
- User needs consistently formatted hourly data for analysis
- User asks for zonal or regional breakdowns
- User wants standardized data for cross-ISO comparisons
- User needs clean data for modeling or visualization

SUPPORTED ISOs:
- pjm (extensive zonal data), caiso, miso, others

PARAMETERS:
- iso (REQUIRED): ISO identifier
- start (OPTIONAL): Start date
- end (OPTIONAL): End date
- limit (OPTIONAL): Maximum rows
- timezone (OPTIONAL): Timezone

EXAMPLES:
- "PJM zonal load for today" → call with iso="pjm", start="2026-04-07"
- "Standardized CAISO data this week" → call with iso="caiso", start="2026-04-01", limit=168
- "PJM hourly load yesterday" → call with iso="pjm", start="2026-04-06", end="2026-04-07"

Get standardized hourly data for a US ISO with consistent column naming


## Installation & Usage

To install and use the **GridStatus** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gridstatus](https://vinkius.com/mcp/gridstatus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
