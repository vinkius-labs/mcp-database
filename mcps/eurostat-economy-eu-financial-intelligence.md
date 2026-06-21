# Eurostat Economy — EU Financial Intelligence MCP Server

Official EU economic data: quarterly GDP for all 27 member states, government debt and deficit (Maastricht criteria), HICP inflation (the ECB's target measure), interest rates, and EUR exchange rates.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/eurostat-economy-eu-financial-intelligence)

## Overview
**Category:** data-analytics
**Tools Count:** 6

## Description
Connect your AI agent to the official economic statistics of the European Union.

### What you can do
- **GDP** — Quarterly and annual GDP for all 27 EU countries + euro area. Components: consumption, investment, government spending, trade
- **Government Debt** — Public debt (% of GDP) and deficit/surplus. Maastricht criteria monitoring: 60% debt ceiling, 3% deficit limit
- **Inflation (HICP)** — The Harmonised Index of Consumer Prices — the official inflation measure used by the ECB. Monthly rates, annual averages, by COICOP category
- **Interest Rates** — Short-term and long-term government bond yields across the EU
- **Exchange Rates** — EUR vs USD, GBP, JPY, CHF and 30+ currencies
- **Generic Query** — Access any of 7,000+ Eurostat datasets by code

### No API Key Required
Eurostat provides completely open, free access. No registration needed.

### Who is this for?
ECB watchers, sovereign debt analysts, EU policy researchers, macro strategists, and anyone tracking European economic performance.


## Available Tools
- **get_gdp**: Dataset: namq_10_gdp (quarterly) or nama_10_gdp (annual). Filter by country, unit (CLV10_MEUR, CP_MEUR, PC_GDP), and GDP component (B1GQ=GDP, P3=consumption, P5G=investment).

Get EU GDP data by country — quarterly or annual
- **get_government_debt**: Dataset: gov_10dd_edpt1 (annual EDP). Critical for Maastricht criteria monitoring (60% debt, 3% deficit).

Get EU government debt and deficit by country
- **get_inflation**: Datasets: prc_hicp_manr (annual rate, monthly), prc_hicp_mmor (monthly rate), prc_hicp_aind (annual average). The ECB targets 2% HICP inflation. Filter by country and COICOP category.

Get EU inflation (HICP) — the official measure used by the ECB
- **get_interest_rates**: Datasets: irt_st_m (short-term, monthly), irt_lt_mcby_m (long-term government bond yields). Key for ECB policy analysis.

Get EU short-term and long-term interest rates
- **get_exchange_rates**: Dataset: ert_bil_eur_m (monthly) or ert_bil_eur_d (daily).

Get EUR bilateral exchange rates against major currencies
- **get_economic_dataset**: Use the Eurostat Data Browser to find codes. Common: nama_10_gdp, gov_10q_ggnfa, tec00115, teina225.

Query any Eurostat economy/finance dataset by code


## Installation & Usage

To install and use the **Eurostat Economy — EU Financial Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eurostat-economy-eu-financial-intelligence](https://vinkius.com/mcp/eurostat-economy-eu-financial-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
