# IBGE Serviços de Dados MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ibge-servicos-de-dados)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ibge-servicos-de-dados-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ibge-servicos-de-dados-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access official Brazilian statistics, geographic data, economic classifications (CNAE), and demographic insights directly from IBGE.

## Description
Connect to the **IBGE (Brazilian Institute of Geography and Statistics)** data services and empower your AI agent with official Brazilian socio-economic and geographic data.

### What you can do

- **Statistical Aggregates** — Query complex data from various IBGE surveys including inflation, employment, and production metrics.
- **Demographics & Names** — Explore the frequency of first names in Brazil based on the 2010 Census, filtered by region or gender.
- **Economic Classifications** — Browse the CNAE (National Classification of Economic Activities) to identify business sectors and classes.
- **Geographic Data** — Retrieve geographic names from the BNGB and fetch state-level geographic meshes for mapping.
- **Official News** — Stay updated with the latest releases, news, and reports from the Agência IBGE Notícias.
- **Release Calendar** — Monitor the schedule of upcoming statistical publications and survey results.

### How it works

1. Subscribe to this server
2. No complex authentication is required for public data access
3. Start querying official Brazilian data from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts** — quickly fetch official time-series and aggregates for Brazilian economic indicators
- **Developers** — integrate official CNAE classifications and geographic identifiers into business applications
- **Researchers** — access demographic trends and census data through natural language queries


## Available Tools
- **get_agregados**: Obtém o conjunto de agregados do IBGE
- **get_nome_geografico**: Obtém um nome geográfico do BNGB
- **get_calendario**: Obtém o calendário de divulgações de uma pesquisa
- **get_cnae_classe**: Obtém classes CNAE
- **get_malha_estado**: Obtém malha geográfica de um estado
- **get_metadados**: Obtém metadados de pesquisas do IBGE
- **get_nomes_frequencia**: Consulta frequência de nomes no Brasil
- **get_noticias**: Consulta notícias e releases do IBGE


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBGE Serviços de Dados** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the frequency of the name 'João' in Brazil according to IBGE?"

**🤖 AI Agent:**
> I've queried the 2010 Census data. The name 'João' has a total frequency of 2,971,335 occurrences. The decade with the highest frequency was the 1950s with 418,174 births.

---

**👤 You:**
> "Show me the latest news from IBGE about the 'Censo'."

**🤖 AI Agent:**
> I found several recent updates regarding the Census. The most recent release is 'IBGE releases new demographic coordinates from the 2022 Census'. Would you like the full summary?

---

**👤 You:**
> "What are the CNAE classes related to code 0111-3?"

**🤖 AI Agent:**
> The CNAE class 0111-3 refers to 'Cultivation of cereals'. It includes activities like growing corn, wheat, rice, and other grains. Is there a specific sub-category you need?


## Installation & Usage

To install and use the **IBGE Serviços de Dados** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibge-servicos-de-dados](https://vinkius.com/mcp/ibge-servicos-de-dados)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
