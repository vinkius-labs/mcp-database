# ANA (Movimentação de Dados) MCP Server

Access and manage hydrometeorological data from the Brazilian National Water Agency (ANA) — query flow, rainfall, water quality, and cross-section series.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ana-movimentacao-de-dados)

## Overview
**Category:** data-management
**Tools Count:** 18

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


## Installation & Usage

To install and use the **ANA (Movimentação de Dados)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ana-movimentacao-de-dados](https://vinkius.com/mcp/ana-movimentacao-de-dados)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
