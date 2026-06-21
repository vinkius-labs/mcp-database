# IBGE Agregados (SIDRA) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ibge-agregados-sidra)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ibge-agregados-sidra-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ibge-agregados-sidra-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access official Brazilian statistical data from IBGE SIDRA — query surveys, metadata, variables, and geographic levels directly.

## Description
Connect to the **IBGE SIDRA** (System for Automatic Recovery) database and explore Brazil's official statistical aggregates through natural language. This server provides a direct interface to the most comprehensive source of Brazilian demographic and economic data.

### What you can do

- **Survey Discovery** — List and filter IBGE aggregates (tables) by subject, period, or classification to find exactly the data you need.
- **Metadata Inspection** — Retrieve detailed metadata for specific tables to understand the context and methodology of the data.
- **Variable Analysis** — Identify all available variables within an aggregate to prepare precise data queries.
- **Temporal Coverage** — Check available time periods for any survey to build historical series or snapshots.
- **Geographic Granularity** — Discover which territorial levels (National, State, City, etc.) are available for specific datasets.

### How it works

1. Subscribe to this server
2. No complex API keys are required for this public data service
3. Start querying Brazilian statistics directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists & Analysts** — quickly locate specific tables and variables for economic or social modeling.
- **Researchers & Academics** — access official census and survey metadata without navigating complex web portals.
- **Developers** — integrate official Brazilian statistics into applications with ease.


## Available Tools
- **get_localidades**: Get available geographic levels for an aggregate
- **get_metadados**: Get metadata for a specific aggregate
- **get_periodos**: Get available time periods for an aggregate
- **get_variaveis**: Get variables for a specific aggregate
- **list_agregados**: Allows multidimensional filtering.

List IBGE aggregates (surveys/tables)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBGE Agregados (SIDRA)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all IBGE aggregates related to 'PIB' (GDP)."

**🤖 AI Agent:**
> I've found several aggregates related to GDP. For example, Aggregate 5932 (PIB a preços correntes) and Aggregate 1612 (Contas Regionais). Which one would you like to explore?

---

**👤 You:**
> "What variables are available for aggregate 1737?"

**🤖 AI Agent:**
> For aggregate 1737, the available variables include: 'Número de empresas e outras organizações' (ID: 628), 'Pessoal ocupado total' (ID: 629), and 'Salários e outras remunerações' (ID: 630).

---

**👤 You:**
> "Show me the available geographic levels for aggregate 5932."

**🤖 AI Agent:**
> Aggregate 5932 supports the following geographic levels: 'Brasil' (N1), 'Grande Região' (N2), 'Unidade da Federação' (N3), and 'Município' (N6).


## Installation & Usage

To install and use the **IBGE Agregados (SIDRA)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibge-agregados-sidra](https://vinkius.com/mcp/ibge-agregados-sidra)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
