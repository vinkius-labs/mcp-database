# IBGE Censo & SIDRA — Dados Censitários MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ibge-censo-sidra-dados-censitarios)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ibge-censo-sidra-dados-censitarios-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ibge-censo-sidra-dados-censitarios-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access Brazil's official census and statistical data: GDP, population, employment, inflation (IPCA), agricultural production, and thousands of SIDRA aggregate tables — the backbone of Brazilian economic intelligence.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBGE Censo & SIDRA — Dados Censitários** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the latest IPCA inflation rate in Brazil?"

**🤖 AI Agent:**
> 📊 **Brazil — IPCA (Consumer Price Index)**

Latest month: +0.43%
12-month accumulated: 4.62%
Top contributors: Food (+0.18%), Transportation (+0.12%)
Target range: 3.0% ± 1.5pp

Inflation remains within the Central Bank's target range.

---

**👤 You:**
> "What is the GDP of the state of São Paulo?"

**🤖 AI Agent:**
> 💰 **São Paulo — GDP**

GDP: R$ 2.7 trillion (2022)
Share of national GDP: 30.5%
Per capita GDP: R$ 58,200

São Paulo alone has a GDP larger than most Latin American countries — equivalent to Argentina's entire economy.

---

**👤 You:**
> "What is the population of Brazil by macro-region?"

**🤖 AI Agent:**
> 👥 **Brazil — Population by Macro-Region**

- Sudeste: 89.6M (41.8%)
- Nordeste: 57.7M (26.9%)
- Sul: 30.4M (14.2%)
- Norte: 19.2M (9.0%)
- Centro-Oeste: 17.4M (8.1%)

**Total: 214.3 million** (2022 Census)


## Installation & Usage

To install and use the **IBGE Censo & SIDRA — Dados Censitários** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibge-censo-sidra-dados-censitarios](https://vinkius.com/mcp/ibge-censo-sidra-dados-censitarios)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
