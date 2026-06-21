# UK ONS Full — Complete Statistical Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uk-ons-full-complete-statistical-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/uk-ons-full-complete-statistical-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/uk-ons-full-complete-statistical-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

The definitive UK ONS Mega-Server: 20 tools spanning GDP, inflation, retail sales, card spending, household income, weekly deaths, well-being, population projections, trade, business counts, and a universal query engine for any of the 337+ available datasets.

## Description
The **ultimate UK ONS Mega-Server** — 20 tools across 4 domains.

### 20 Tools
- 💰 Economy (6) — GDP, CPIH, retail sales, card spending, tax
- 👥 Population (5) — Deaths, well-being, suicides, projections
- 🚢 Trade (3) — Goods trade, business counts, traffic
- 🔍 Discovery (6) — Search, browse, metadata, query

### No API Key Required


## Available Tools
- **search_datasets**: Returns matching dataset IDs, titles, and descriptions. Use this to find the right dataset before querying data.

Search ONS datasets by keyword — explore 337+ available datasets
- **list_datasets**: The catalog contains 337+ datasets covering economy, population, health, trade, business, and more.

Browse the complete ONS dataset catalog with pagination
- **get_dataset_info**: Get metadata for an ONS dataset: dimensions, editions, versions
- **get_dimensions**: Each dimension has options you can use to filter observations. Essential for understanding what query parameters to use.

Get available dimensions and filter options for an ONS dataset
- **get_dimension_options**: g., all geography codes, all time periods, all aggregate categories). Use this to find the correct filter values for observations.

Get all option values for a specific dimension in an ONS dataset
- **get_observations**: Provide dataset ID and dimension filters. Use search_datasets to find IDs and get_dimensions to discover available filters. Set time=* for full time series.

Query any ONS dataset by ID with flexible dimension filters
- **get_gdp**: Main datasets: regional-gdp-by-quarter (quarterly), regional-gdp-by-year (annual). Covers England, Wales, and 9 English regions. Use time=* for the full time series.

Get UK GDP data — quarterly and annual, by region and sector
- **get_cpih**: Dataset: cpih01. The headline UK inflation measure used by the ONS. Filter by aggregate (cpih1dim1A0 = all items) and geography (K02000001 = UK).

Get UK inflation (CPIH) — the official consumer prices index including housing costs
- **get_retail_sales**: Dataset: retail-sales-index. Monthly data showing value and volume of retail sales in Great Britain. Base year 2019=100. Seasonally and non-seasonally adjusted.

Get UK retail sales index — value and volume of consumer spending
- **get_spending_cards**: Dataset: uk-spending-on-cards. Weekly data providing near real-time insight into consumer spending patterns.

Get UK debit and credit card spending — experimental real-time indicator
- **get_tax_benefits**: Dataset: tax-benefits-statistics. Shows redistribution effects of direct and indirect taxation and benefits in cash or kind.

Get the effects of taxes and benefits on UK household income
- **get_economy_dataset**: Common IDs: regional-gdp-by-quarter, cpih01, retail-sales-index, uk-spending-on-cards. Use get_dimensions to discover available filters.

Query any ONS economy dataset by ID with flexible filters
- **get_weekly_deaths**: Datasets: weekly-deaths-age-sex (by age and sex), weekly-deaths-region (by region). National statistics updated weekly.

Get weekly death registrations in England and Wales — by age, sex, and region
- **get_wellbeing**: Dataset: wellbeing-quarterly. Higher scores (0-10) indicate better well-being (except anxiety, where lower is better).

Get UK personal well-being estimates — life satisfaction, happiness, anxiety
- **get_wellbeing_local**: Dataset: wellbeing-local-authority. Covers life satisfaction, worthwhileness, happiness, and anxiety by region.

Get well-being estimates by UK local authority
- **get_suicides**: Dataset: suicides-in-the-uk. National statistics. If you are struggling, call Samaritans free: 116 123.

Get suicide registrations by local authority in England and Wales
- **get_population_projections**: Dataset: projections-older-people-sex-ratios.

Get UK population projections for older people, sex ratios by local authority
- **get_trade**: Dataset: trade. Monthly data on UK trade in goods: imports, exports, trade balance by partner country and commodity. Non-seasonally adjusted. Values in £ million.

Get UK trade in goods data — country by commodity, imports and exports
- **get_business_counts**: Dataset: uk-business-by-enterprises-and-local-units. Source: Inter-Departmental Business Register (IDBR).

Get UK business counts by enterprises and local units, by industry and geography
- **get_traffic_activity**: Dataset: traffic-camera-activity. Used as a real-time indicator to understand economic activity and social change.

Get UK traffic camera activity — experimental economic indicator


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UK ONS Full — Complete Statistical Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Full UK economic briefing: GDP, inflation, retail, and trade"

**🤖 AI Agent:**
> 🇬🇧 **UK Economic Briefing**

💰 GDP: +0.3% Q3 2025 (quarterly)
📈 CPIH: 3.2% (February 2026)
🛒 Retail: +1.2% monthly (volume)
🚢 Trade: -£8.6B deficit with EU
💳 Card Spending: +2.1% vs pre-pandemic

5 ONS datasets queried simultaneously.

---

**👤 You:**
> "Can you compare UK GDP growth with the inflation rate (CPIH) over the last year?"

**🤖 AI Agent:**
> Based on recent ONS data: In the 12 months to February 2026, the CPIH annual inflation rate was 3.2%. Concurrently, UK GDP saw an estimated growth of 0.3% in the latest quarter, indicating low growth against persistent inflation.

---

**👤 You:**
> "Give me a summary of UK population projections and life expectancy."

**🤖 AI Agent:**
> According to the latest ONS projections, the UK population is projected to grow to over 70 million by 2036. Period life expectancy at birth in the UK is currently estimated at 79.0 years for males and 82.9 years for females.


## Installation & Usage

To install and use the **UK ONS Full — Complete Statistical Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uk-ons-full-complete-statistical-intelligence](https://vinkius.com/mcp/uk-ons-full-complete-statistical-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
