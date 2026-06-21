# Eurostat Full Access — EU Statistical Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eurostat-full-access-eu-statistical-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eurostat-full-access-eu-statistical-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eurostat-full-access-eu-statistical-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

The ultimate EU statistics Mega-Server: 26 tools spanning economy (GDP, inflation, debt), demographics (population, unemployment, migration), trade, environment (emissions, energy, renewables), and 7,000+ dataset discovery — all 27 EU member states.

## Description
The **definitive Mega-Server** for EU statistical intelligence.

### 26 tools across 5 domains
- 💰 Economy (6) — GDP, debt, HICP, rates, exchange
- 👥 Population (6) — Demographics, unemployment, migration, wages
- 🚢 Trade (5) — International trade, industrial production, retail
- 🌱 Environment (6) — Emissions, energy, renewables, waste, agriculture
- 🔍 Discovery (3) — Search 7K+ datasets, metadata, generic query

### No API Key Required


## Available Tools
- **search_datasets**: Returns matching dataset codes and names. Use this to find the right dataset code before querying data.

Search Eurostat dataset catalog by keyword
- **get_dataset_metadata**: Shows all available dimensions, code lists, and possible filter values. Use this before querying to understand what filters are available.

Get metadata for a Eurostat dataset: dimensions, codes, frequencies
- **get_dataset**: Provide the dataset code and optional dimension filters. Find codes via search_datasets or the Eurostat Data Browser.

Query any Eurostat dataset by code with flexible filters
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
- **get_emissions**: Units: tonnes of CO2 equivalent. Breakdown by source sector (energy, agriculture, transport, industry, waste). Essential for EU Green Deal and Paris Agreement tracking.

Get EU greenhouse gas emissions by country and sector
- **get_energy_balance**: Production, imports, exports, gross consumption by energy source. The definitive view of a country energy system.

Get EU complete energy balance by country
- **get_energy_prices**: Datasets: nrg_pc_204 (electricity households), nrg_pc_205 (electricity industry), nrg_pc_202 (gas households), nrg_pc_203 (gas industry). Semi-annual data in EUR per kWh / GJ.

Get EU electricity and gas prices for households and industry
- **get_renewable_energy**: The EU target is 42.5% by 2030. Leaders: Sweden (~65%), Finland (~48%). Laggards: Luxembourg, Malta, Belgium.

Get EU renewable energy share by country
- **get_waste_statistics**: Treatment: landfill, incineration, recycling. Key for circular economy policy.

Get EU waste generation and treatment data
- **get_agriculture_data**: Covers cereals, fruits, vegetables, wine grapes, olive oil. Essential for Common Agricultural Policy (CAP) analysis.

Get EU agriculture production data
- **get_population**: Dataset: demo_pjan. Filter by age group and sex. Covers all 27 EU members + EEA + candidate countries.

Get EU population by country, age, and sex
- **get_unemployment**: Dataset: une_rt_m (monthly). The most-watched EU labor market indicator. Youth unemployment (une_rt_m with age=Y_LT25) is a critical policy metric.

Get EU unemployment rates monthly by country, age, and sex
- **get_employment**: Key indicators for labor market tightness and wage pressure analysis.

Get EU employment rates and labor cost index
- **get_migration**: Critical data for understanding EU migration flows, asylum, and demographic change.

Get EU immigration and emigration data by citizenship
- **get_life_expectancy**: A key demographic and health policy indicator. Shows dramatic variation across EU: from ~74 years (Bulgaria) to ~84 years (Spain).

Get life expectancy at birth by EU country and sex
- **get_minimum_wages**: Shows EUR/month values. Not all EU countries have statutory minimums (e.g., Nordics use collective bargaining). Updated semi-annually.

Get minimum wage levels across EU countries
- **get_trade_balance**: Dataset: ext_lt_maineu. Key partners: US, CN, UK, JP, CH.

Get EU international trade balance by partner country
- **get_trade_by_product**: Dataset: ext_st_eu27_2020sitc. Covers food, raw materials, fuels, chemicals, machinery, manufactured goods.

Get EU trade by product classification (SITC)
- **get_industrial_production**: Base year 2015=100. Breakdown by NACE sector. A leading indicator of economic activity.

Get EU industrial production index by country and sector
- **get_retail_trade**: Consumer spending proxy. Covers food, non-food, and online retail.

Get EU retail trade volume index
- **get_trade_dataset**: Common codes: ext_tec01, sts_inpr_m, sts_trtu_m, sbs_na_ind_r2.

Query any Eurostat trade/industry dataset by code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eurostat Full Access — EU Statistical Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Full EU snapshot: GDP, unemployment, inflation, and emissions"

**🤖 AI Agent:**
> 🇪🇺 **EU Dashboard**

| Indicator | EU27 | Trend |
|-----------|------|-------|
| GDP Growth | +0.8% | → |
| Unemployment | 5.9% | ↓ |
| HICP Inflation | 2.4% | ↓ |
| GHG Emissions | -31% vs 1990 | ↓ |
| Renewable Share | 23.0% | ↑ |
| Youth Unemployment | 14.5% | → |

Cross-domain query using economy + population + environment tools.

---

**👤 You:**
> "Compare Portugal across economy, demographics, and energy"

**🤖 AI Agent:**
> 🇵🇹 **Portugal — Multi-Domain Profile**

💰 GDP: €245B (2.3% growth)
📊 Debt/GDP: 99.1%
👥 Population: 10.3M (aging rapidly)
📉 Unemployment: 6.6%
💶 Minimum wage: €820
⚡ Electricity: 0.218 €/kWh
🌱 Renewable share: 34%
🌍 Emissions: -38% vs 1990

7 different datasets queried in one session.

---

**👤 You:**
> "Find and query a dataset about tourism in the EU"

**🤖 AI Agent:**
> 🔍 Found: `tour_occ_ninat` — Nights spent in tourist accommodation

🏨 **EU Tourism (Nights Spent)**

🇪🇸 Spain: 468M nights (#1)
🇮🇹 Italy: 436M
🇫🇷 France: 394M
🇩🇪 Germany: 389M
🇬🇷 Greece: 142M

Discovery + query in a single session.


## Installation & Usage

To install and use the **Eurostat Full Access — EU Statistical Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eurostat-full-access-eu-statistical-intelligence](https://vinkius.com/mcp/eurostat-full-access-eu-statistical-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
