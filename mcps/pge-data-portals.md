# PG&E Data Portals MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pge-data-portals)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pge-data-portals-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pge-data-portals-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Search and query PG&E energy datasets: usage, EV adoption, solar, grid data.

## Description
Connect **PG&E Data Portals** to any AI agent and programmatically search, discover, and query PG&E's public energy datasets through natural conversation.

### What you can do
- **Dataset Search** — Search the complete PG&E Data Portals catalog for energy-related datasets
- **Energy Usage** — Query electricity and gas consumption data by ZIP code and date range
- **EV Adoption** — Access electric vehicle registration and adoption trends by geographic area
- **Solar Generation** — Retrieve solar energy production and net energy metering (NEM) statistics
- **Energy Efficiency** — Analyze program participation, energy savings achieved, and cost-effectiveness
- **Grid Infrastructure** — Access distribution circuit, substation, and grid capacity data
- **Date Range Queries** — Filter any dataset by specific time periods for trend analysis
- **Dataset Metadata** — Get schema information and field descriptions for all datasets

### How it works
1. Subscribe to this server
2. (Optional) Enter your PG&E Data Portals API Key for higher rate limits
3. Start exploring PG&E energy data from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Energy Analysts** — analyze consumption trends, EV adoption patterns, and solar generation data
- **Urban Planners** — access grid infrastructure and regional energy consumption data
- **Researchers** — query time-series energy data for academic and policy studies
- **Clean Tech Companies** — identify high-potential markets for EV charging, solar, and efficiency products


## Available Tools
- **query_by_date_range**: Specify the dataset ID and start/end dates to retrieve records within that time period. Use this for time-series analysis across any dataset type. Dataset ID from search_datasets. Dates in YYYY-MM-DD format. This is useful for year-over-year comparisons and trend analysis.

Query any PG&E dataset filtered by a specific date range
- **query_ev_adoption**: Use this to analyze EV adoption trends, identify high-adoption areas, and correlate with charging infrastructure. ZIP code is 5-digit format. Year is YYYY format (e.g., "2024").

Query electric vehicle adoption data by ZIP code and year
- **query_energy_efficiency**: ), and investment amounts. Use this to analyze program effectiveness and ROI of energy efficiency initiatives. Optional programType filters by program category. Year is YYYY format.

Query PG&E energy efficiency program data
- **query_energy_usage**: Returns electricity usage aggregated by customer segment (residential, commercial, industrial, agricultural). Use this to analyze energy consumption patterns in specific geographic areas over time. ZIP code format: 5-digit (e.g., "94102"). Dates in YYYY-MM-DD format.

Query PG&E energy consumption data by ZIP code and date range
- **get_dataset_schema**: Use this to understand what columns and data types are available before querying. The datasetId is obtained from search_datasets or list_all_datasets.

Get the schema/metadata for a specific PG&E dataset
- **query_grid_infrastructure**: Use this to understand grid capacity, identify areas needing upgrades, or analyze reliability metrics. Region filters by geographic area. dataType can filter by specific infrastructure type.

Query PG&E grid infrastructure and distribution data
- **list_all_datasets**: Each dataset includes name, description, ID, and metadata. Use this as a starting point to explore what data is available from PG&E — includes energy usage, EV adoption, solar generation, energy efficiency programs, and grid infrastructure datasets.

List all available datasets in the PG&E Data Portals catalog
- **query_dataset**: Optional filters can be passed as key-value pairs to narrow results (e.g., zip_code, year, region). Use this to retrieve actual data records from any dataset in the PG&E Data Portals. Dataset IDs are obtained from search_datasets or list_all_datasets.

Query a specific PG&E dataset with optional filters
- **search_datasets**: Use this to discover available datasets before querying specific data. Returns dataset names, descriptions, IDs, and metadata. Optional query parameter filters results by keyword.

Search the PG&E Data Portals catalog for energy datasets
- **query_solar_generation**: Use this to analyze solar adoption and production trends. Region can be a county name or service area identifier. Year is YYYY format.

Query solar energy generation data by region and year


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PG&E Data Portals** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available PG&E datasets."

**🤖 AI Agent:**
> Found datasets including: Energy Usage by ZIP Code (monthly electricity and gas consumption by customer segment), EV Adoption (electric vehicle registrations by ZIP code), Solar Generation (installed capacity and production), Energy Efficiency Programs (participation and savings), and Grid Infrastructure (distribution circuits and substations). Which dataset would you like to explore?

---

**👤 You:**
> "Show me electricity usage for ZIP code 94102."

**🤖 AI Agent:**
> Electricity usage for 94102 (San Francisco - Mission District): Jan 2024: 2,450,000 kWh (Residential), 3,120,000 kWh (Commercial). Feb 2024: 2,280,000 kWh (Residential), 2,980,000 kWh (Commercial). Average residential bill: $142/month. Peak usage in January during winter heating season.

---

**👤 You:**
> "Show EV adoption trends by ZIP code for 2024."

**🤖 AI Agent:**
> EV adoption data for 2024: 94301 (Palo Alto): 12,450 EVs registered (38% of households). 94102 (SF Mission): 3,280 EVs (15%). 94040 (Mountain View): 9,870 EVs (32%). 95054 (Santa Clara): 7,650 EVs (28%). Highest adoption in Peninsula/Silicon Valley ZIP codes with proximity to tech employers and charging infrastructure.


## Installation & Usage

To install and use the **PG&E Data Portals** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pge-data-portals](https://vinkius.com/mcp/pge-data-portals)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
