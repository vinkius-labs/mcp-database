# IBGE Full Access — Dados Brasileiros MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ibge-full-access-dados-brasileiros)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ibge-full-access-dados-brasileiros-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ibge-full-access-dados-brasileiros-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

The ultimate Brazil data Mega-Server: 15 tools spanning census, cities, CNAE economy, name trends, survey indicators, IBGE news, and country comparisons — all of Brazil's official statistics in one zero-auth integration.

## Description
The **definitive Mega-Server** for Brazilian data intelligence. Why install 5 servers when one does it all?

### What you can do
- **🏙️ Localities** — 5,570 municipalities, 27 states, regions, metropolitan areas
- **📊 Census (SIDRA)** — GDP, population, employment, inflation across 10,000+ tables
- **🔬 Surveys** — Health, education, and quality-of-life indicators for every city
- **👤 Names** — Name frequency by decade since the 1930s + popularity rankings
- **💼 Economy (CNAE)** — 1,332 economic activity classifications
- **📰 News** — Latest releases from Agência IBGE Notícias
- **🌍 Countries** — Socioeconomic indicators for any country in the world

### Who is this for?
Power users, data scientists, and AI agents that need comprehensive Brazilian intelligence without managing multiple integrations.


## Available Tools
- **list_estados**: List all 27 Brazilian states
- **get_nome_frequencia**: Get birth frequency by decade for a name
- **get_ranking_nomes**: Filter by decade or sex.

Get ranking of most popular Brazilian names
- **list_secoes_cnae**: List all 21 CNAE economic sections
- **get_subclasse_cnae**: Get CNAE subclass details
- **get_noticias_ibge**: Get latest news from IBGE news agency
- **get_pais_indicadores**: Use the M49 country code.

Get socioeconomic indicators for any country
- **get_municipios_por_uf**: List municipalities in a state
- **get_municipio**: Get municipality details by IBGE code
- **list_regioes**: List the 5 macro-regions of Brazil
- **list_agregados**: List SIDRA aggregate tables
- **get_agregado_data**: Levels: N1=Brasil, N3=UF, N6=Município.

Get data from a SIDRA aggregate table
- **get_agregado_metadados**: Get metadata for a SIDRA aggregate
- **list_pesquisas**: List all IBGE surveys
- **get_resultados_pesquisa**: Get survey results for a municipality


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBGE Full Access — Dados Brasileiros** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Complete profile of the city of Florianópolis — geography, economy, and demographics"

**🤖 AI Agent:**
> 🏝️ **Florianópolis — Full Profile**

📍 IBGE: 4205407 | UF: SC | Region: Sul
👥 Population: 537,213 (2022)
💰 GDP: R$ 24.8B | Per capita: R$ 46,200
📚 Literacy: 98.4% | Schooling: 11.2 yrs
🏥 Life expectancy: 78.4 years
🏘️ Metropolitan region: 22 municipalities

Florianópolis is consistently ranked among Brazil's top 5 cities in quality of life.

---

**👤 You:**
> "What is the most popular baby name in Brazil right now and what is its CNAE equivalent for a naming consultancy?"

**🤖 AI Agent:**
> 👶 **Most Popular Name (2010s)**

Miguel (M) and Helena (F) lead the 2010s decade.

💼 **Naming Consultancy CNAE**
- 7020-4/00 — Management consulting
- 9329-8/99 — Other recreational activities

Cross-domain query executed: Names API + CNAE API in one shot!

---

**👤 You:**
> "Latest IBGE news and how Brazil compares to Argentina in population"

**🤖 AI Agent:**
> 📰 **Latest IBGE News**

1. 'Censo 2022 revela envelhecimento acelerado da população'
2. 'PIB cresce 2.9% em 2024, supera expectativas'
3. 'IPCA de março: 0.43%, acumulado 4.62%'

🌍 **Brazil vs Argentina — Population**
- Brazil: 214.3M | Argentina: 46.2M
- Brazil is 4.6× larger in population
- Brazil density: 25/km² | Argentina: 17/km²


## Installation & Usage

To install and use the **IBGE Full Access — Dados Brasileiros** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibge-full-access-dados-brasileiros](https://vinkius.com/mcp/ibge-full-access-dados-brasileiros)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
