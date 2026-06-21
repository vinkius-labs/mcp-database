# IBGE Censo & SIDRA — Dados Censitários MCP Server

Access Brazil's official census and statistical data: GDP, population, employment, inflation (IPCA), agricultural production, and thousands of SIDRA aggregate tables — the backbone of Brazilian economic intelligence.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ibge-censo-sidra-dados-censitarios)

## Overview
**Category:** data-analytics
**Tools Count:** 4

## Description
Connect your AI agent to **SIDRA** — Brazil's most powerful statistical data system, maintained by IBGE since 1940.

### What you can do
- **GDP & Economy** — National, state, and municipal GDP data with time series
- **Population Census** — Demographic data from the latest census with age, sex, race, education breakdowns
- **Employment** — PNAD labor force survey data by region and sector
- **Inflation (IPCA)** — Monthly consumer price index with product-level decomposition
- **Agriculture** — Crop production, livestock, and agricultural census data

### How it works
1. Subscribe — it's free and instant.
2. Query any of SIDRA's 10,000+ aggregate tables.
3. Filter by geography (Brasil, state, municipality), time period, and variable.

### Who is this for?
Economists, journalists, policy researchers, investment analysts, ESG consultants, and data scientists working with Brazilian macroeconomic data.


## Available Tools
- **list_agregados**: List all SIDRA aggregate tables grouped by survey
- **get_agregado_data**: Example: aggregate 4714 (IPCA) variable 63 (monthly variation). Levels: N1=Brasil, N2=Região, N3=UF, N6=Município.

Get census/survey data from a SIDRA aggregate table
- **get_agregado_metadados**: Get metadata for a SIDRA aggregate
- **get_agregado_periodos**: Get available periods for a SIDRA aggregate


## Installation & Usage

To install and use the **IBGE Censo & SIDRA — Dados Censitários** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibge-censo-sidra-dados-censitarios](https://vinkius.com/mcp/ibge-censo-sidra-dados-censitarios)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
