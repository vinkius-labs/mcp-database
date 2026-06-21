# ANA (Movimentação de Dados) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ana-movimentacao-de-dados)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ana-movimentacao-de-dados-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ana-movimentacao-de-dados-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access and manage hydrometeorological data from the Brazilian National Water Agency (ANA) — query flow, rainfall, water quality, and cross-section series.

## Description
Connect to the **ANA (Agência Nacional de Águas e Saneamento Básico)** data movement API to retrieve and manage critical hydrometeorological information directly through your AI agent.

### What you can do

- **Flow & Rainfall Series** — Query historical and real-time data for flow (Vazão) and rainfall (Chuva) using station codes or specific series IDs.
- **Water Quality (QA)** — Access detailed water quality parameters and monitoring series to analyze environmental health.
- **Cross-Section Profiles** — Retrieve transverse profile data (Perfil Transversal) for river morphology and engineering studies.
- **Discharge Summaries** — Inspect discharge summaries (Resumo Descarga) and level data (Cota) for comprehensive basin management.
- **Data Management** — Beyond querying, authorized users can create and update data series records directly in the ANA system.

### How it works

1. Subscribe to this server
2. Provide your ANA Identificador and Senha (credentials)
3. Start querying Brazilian water data from Claude, Cursor, or any MCP client

### Who is this for?

- **Hydrologists & Engineers** — Quickly pull station data for modeling and reporting without manual portal navigation.
- **Environmental Researchers** — Analyze water quality and rainfall trends across different Brazilian basins.
- **Data Scientists** — Automate the collection of hydrometeorological time series for climate and impact analysis.


## Available Tools
- **create_serie_chuva**: Inclusion of Rainfall (Chuva) Series data
- **create_serie_cota**: Inclusion of Stage/Level (Cota) Series data
- **create_serie_perfil_transversal**: Inclusion of Cross-Section Profile Series (Série Perfil Transversal) data
- **create_serie_qa**: Inclusion of Water Quality (QA) Series data
- **create_serie_resumo_descarga**: Inclusion of Discharge Summary Series (Série Resumo Descarga) data
- **create_serie_vazao**: Inclusion of Flow Series (Série Vazão) data
- **get_serie_chuva**: Search for Rainfall (Chuva) Series data
- **get_serie_cota**: Search for Stage/Level (Cota) Series data
- **get_serie_perfil_transversal**: Search for Cross-Section Profile Series (Série Perfil Transversal) data
- **get_serie_qa**: Search for Water Quality (QA) Series data
- **get_serie_resumo_descarga**: Search for Discharge Summary Series (Série Resumo Descarga) data
- **get_serie_vazao**: No limitation on the number of searches per request.

Search for Flow Series (Série Vazão) data
- **update_serie_chuva**: Update/Modification of Rainfall (Chuva) Series data
- **update_serie_cota**: Update/Modification of Stage/Level (Cota) Series data
- **update_serie_perfil_transversal**: Update/Modification of Cross-Section Profile Series (Série Perfil Transversal) data
- **update_serie_qa**: Update/Modification of Water Quality (QA) Series data
- **update_serie_resumo_descarga**: Update/Modification of Discharge Summary Series (Série Resumo Descarga) data
- **update_serie_vazao**: Update/Modification of Flow Series (Série Vazão) data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ANA (Movimentação de Dados)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for flow series data (vazão) for station code 66070000."

**🤖 AI Agent:**
> I've retrieved the flow data for station 66070000. The series includes daily measurements showing a mean flow of 150 m³/s for the requested period. Would you like to see the full table?

---

**👤 You:**
> "Get the water quality (QA) series for ID 12345."

**🤖 AI Agent:**
> Accessing Water Quality data... For series ID 12345, I found parameters for Turbidity, Dissolved Oxygen, and pH levels. The last recorded pH was 7.2.

---

**👤 You:**
> "List the rainfall series (chuva) for station 45001000 on 2023-05-20."

**🤖 AI Agent:**
> Querying rainfall data... On 2023-05-20, station 45001000 recorded a total precipitation of 12.5mm. There are 3 active series associated with this station.


## Installation & Usage

To install and use the **ANA (Movimentação de Dados)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ana-movimentacao-de-dados](https://vinkius.com/mcp/ana-movimentacao-de-dados)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
