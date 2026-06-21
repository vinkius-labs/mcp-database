# PG&E Public Datasets MCP Server

Access PG&E public energy data: monthly usage, billing, savings, and regional comparisons.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pge-public-datasets)

## Overview
**Category:** data-analytics
**Tools Count:** 8

## Description
Access **PG&E Public Datasets** directly from any AI agent and explore energy consumption, billing trends, efficiency savings, and regional comparisons without any authentication.

### What you can do
- **Monthly Usage** — Get monthly electricity and gas consumption by ZIP code and customer segment
- **Customer Segments** — View energy usage breakdown across Residential, Commercial, Industrial, and Agricultural sectors
- **Yearly Trends** — Analyze year-over-year energy consumption trends
- **Electricity by ZIP** — Access ZIP code-level electricity consumption data
- **Gas by ZIP** — Access ZIP code-level natural gas consumption data
- **Billing Data** — Retrieve average bills and cost metrics by region
- **Savings Data** — Analyze energy efficiency program savings and cost-effectiveness
- **Regional Comparisons** — Compare energy usage across multiple ZIP codes side-by-side

### How it works
1. Subscribe to this server
2. No API key needed — completely free and public
3. Start exploring PG&E energy data from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Energy Researchers** — analyze consumption trends and efficiency program effectiveness
- **Policy Makers** — understand energy affordability and regional consumption disparities
- **Clean Energy Companies** — identify high-consumption areas for solar/EV product targeting
- **Journalists** — access public energy data for reporting and analysis


## Available Tools
- **get_billing_data**: Data is available by ZIP code and customer segment. Use this to analyze energy affordability, compare costs across regions, or identify rate impact on customers. Optional zipCode and year filters.

Get billing data and average costs from PG&E public datasets
- **get_usage_by_customer_type**: Shows total consumption for Residential, Commercial, Industrial, and Agricultural sectors. Use this to understand the energy consumption distribution across different customer categories. Optional dataType ("electric"/"gas") and year filters.

Get energy usage broken down by customer segment (residential, commercial, industrial, agricultural)
- **compare_regions**: Returns side-by-side usage figures (kWh and therms), customer counts, and average bills for each region. Use this to identify regional differences in energy consumption, support geographic targeting for efficiency programs, or compare urban vs. rural usage patterns. ZIP codes are comma-separated (e.g., "94102,94103,94104"). Optional dataType and year filters.

Compare energy usage data between multiple ZIP codes/regions
- **get_electricity_by_zip**: Returns monthly or annual usage figures broken down by geographic area. Use this to compare electricity usage across neighborhoods, identify high-consumption areas, or support energy efficiency targeting. Optional year filter.

Get electricity consumption data for specific ZIP codes in PG&E service area
- **get_gas_by_zip**: Returns monthly or annual gas usage figures by geographic area. Use this to analyze heating demand patterns, compare gas usage across regions, or identify electrification opportunities. Optional year filter.

Get natural gas consumption data for specific ZIP codes in PG&E service area
- **get_monthly_usage**: Data is organized by ZIP code, month, year, and customer segment (Residential, Commercial, Industrial, Agricultural). Returns kWh for electric and therms for gas. Use this to analyze consumption patterns over time. Optional filters: dataType ("electric" or "gas"), customerType, zipCode (5-digit), and year (YYYY).

Get monthly energy consumption data by ZIP code and customer segment from PG&E public datasets
- **get_savings_data**: Includes program participation counts, kWh/therms saved, program costs, and cost-effectiveness metrics by program type. Use this to evaluate program ROI, compare effectiveness across initiatives, or identify high-impact efficiency strategies. Optional programType and year filters.

Get energy efficiency program savings data from PG&E
- **get_yearly_trends**: Shows how electricity and gas usage has changed over multiple years. Use this to identify long-term patterns, growth/decline in energy demand, and seasonal variations. Optional dataType filter ("electric" or "gas").

Get yearly energy consumption trends from PG&E public data


## Installation & Usage

To install and use the **PG&E Public Datasets** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pge-public-datasets](https://vinkius.com/mcp/pge-public-datasets)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
