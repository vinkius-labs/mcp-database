# UK ONS Economy — GDP, Inflation & Consumer Spending MCP Server

Official UK economic data: quarterly and annual GDP by region, CPIH inflation (the UK's headline measure), retail sales index, real-time card spending indicators, and household income statistics from the Office for National Statistics.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/uk-ons-economy-gdp-inflation-consumer-spending)

## Overview
**Category:** data-analytics
**Tools Count:** 6

## Description
Official UK economic statistics from the ONS.

### What you can do
- **GDP** — Quarterly and annual, by region
- **CPIH** — The UK's headline inflation measure (including housing)
- **Retail Sales** — Monthly consumer spending volumes
- **Card Spending** — Experimental real-time debit/credit indicator
- **Tax & Benefits** — Household income redistribution

### No API Key Required
Completely open and unrestricted.


## Available Tools
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


## Installation & Usage

To install and use the **UK ONS Economy — GDP, Inflation & Consumer Spending** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uk-ons-economy-gdp-inflation-consumer-spending](https://vinkius.com/mcp/uk-ons-economy-gdp-inflation-consumer-spending)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
