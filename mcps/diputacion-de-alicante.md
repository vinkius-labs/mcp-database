# Diputación de Alicante MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/diputacion-de-alicante)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/diputacion-de-alicante-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/diputacion-de-alicante-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access open data from the province of Alicante — query demographics, municipal budgets, public debt, and local festivals directly.

## Description
Connect your AI agent to the **Diputación de Alicante Open Data** portal to retrieve real-time statistics and historical records about the province. This server provides a direct bridge to official datasets covering demographics, economy, and culture.

### What you can do

- **Demographics** — Analyze population registers, nuclei distribution, and foreign population statistics broken down by country of origin.
- **Economy & Finance** — Access municipal budgets, live debt (Deuda Viva), public debt statistics, and provincial budget evolution.
- **Culture & Tourism** — Explore the calendar of official local festivals, Moors and Christians celebrations, cultural centers, and Blue Flag beach data.
- **Custom Dataset Access** — Use the generic dataset tool to fetch any specific data from the portal using its unique slug.

### How it works

1. Subscribe to this server
2. Configure your access to the Open Data portal
3. Start querying provincial data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly retrieve financial and demographic metrics for provincial research
- **Public Administrators** — monitor budget evolutions and debt levels across different municipalities
- **Tourism & Event Planners** — access official festival calendars and beach quality data for regional planning


## Available Tools
- **get_mayors**: Get Mayors (Historical) dataset
- **get_moors_and_christians_festivals**: Get Moors and Christians Festivals dataset
- **get_municipal_budgets**: Get Municipal Budgets dataset
- **get_official_local_festivals**: Get Official Local Festivals dataset
- **get_population_nuclei**: Get Population Nuclei dataset
- **get_population_register**: Get Population Register Evolution dataset
- **get_provincial_budget_evolution**: Get Provincial Budget Evolution dataset
- **get_provincial_corporation_members**: Get Provincial Corporation Members dataset
- **get_public_debt**: Get Public Debt dataset
- **get_staffing_levels**: Get Staffing Levels (Plantilla de Personal) dataset
- **get_blue_flags**: Get Blue Flags (Beaches) dataset
- **get_cemeteries**: Returns GeoJSON format.

Get Cemeteries dataset
- **get_cultural_centers**: Get Cultural Centers dataset
- **get_dataset**: Use this for datasets not covered by specific tools.

Get any dataset from Diputación de Alicante Open Data
- **get_elections_results**: Get Elections Results dataset
- **get_foreign_population_by_country**: Get Foreign Population by Country dataset
- **get_foreign_population_stats**: Get Foreign Population Statistics dataset
- **get_live_debt**: Get Live Debt (Deuda Viva) dataset
- **get_local_directory**: Get Local Directory (Town Halls) dataset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Diputación de Alicante** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the evolution of the population register in Alicante."

**🤖 AI Agent:**
> I'm fetching the population register evolution data... The dataset shows the historical demographic changes across the province's municipalities from the latest available records.

---

**👤 You:**
> "What are the municipal budgets for this year?"

**🤖 AI Agent:**
> Accessing the municipal budgets dataset... I have retrieved the financial allocations and budget data for the municipalities within the province of Alicante.

---

**👤 You:**
> "List the beaches in Alicante that have received the Blue Flag award."

**🤖 AI Agent:**
> Querying the Blue Flags dataset... I found the list of beaches in Alicante recognized for their environmental and quality standards. Notable entries include beaches in Denia, Altea, and Alicante city.


## Installation & Usage

To install and use the **Diputación de Alicante** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/diputacion-de-alicante](https://vinkius.com/mcp/diputacion-de-alicante)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
