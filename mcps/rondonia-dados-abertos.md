# Rondônia Dados Abertos MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rondonia-dados-abertos)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rondonia-dados-abertos-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rondonia-dados-abertos-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access official open data from the State of Rondônia — query datasets, transparency records, payroll, and public spending.

## Description
Connect to the **Rondônia Dados Abertos** portal and the Transparency API to explore public information from the State of Rondônia directly through your AI agent.

### What you can do

- **Dataset Catalog** — List and inspect all available datasets, organizations, and thematic groups in the CKAN catalog.
- **Transparency & Spending** — Query detailed records of payments made to suppliers, including dates, values, and managing units.
- **Public Payroll** — Access remuneration data for state employees, searchable by name, year, month, and job title.
- **Financial Oversight** — Monitor state revenues and expenses (committed, liquidated, and paid) with granular filtering.
- **Contracts & Agreements** — List active contracts and cooperation agreements (convênios) managed by the state executive branch.

### How it works

1. Subscribe to this server
2. Enter your API Key (if required for higher rate limits) or use the public access
3. Start querying public administration data from Claude, Cursor, or any MCP client

### Who is this for?

- **Journalists & Researchers** — quickly extract public spending data and payroll information for investigative reports.
- **Citizens & Activists** — monitor government transparency and resource allocation in real-time.
- **Data Analysts** — fetch structured metadata from the CKAN catalog to integrate into larger data pipelines.


## Available Tools
- **get_dataset**: Get details for a specific dataset
- **list_contratos**: Consult state contracts
- **list_convenios**: Consult state covenants (convênios)
- **list_datasets**: List all datasets in the Rondônia Dados Abertos catalog
- **list_despesas**: Consult state expenses (committed, liquidated, and paid)
- **list_fornecedores_impedidos**: Consult currently active barred suppliers
- **list_groups**: List all groups in the catalog
- **list_historico_fornecedores_impedidos**: Consult the complete history of suppliers barred from bidding
- **list_organizations**: List all organizations in the catalog
- **list_pagamentos_fornecedores**: Consult payments made to suppliers by the Executive Branch
- **list_receitas**: Consult state revenues collected
- **list_remuneracao_servidores**: Consult state employee payroll and remuneration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rondônia Dados Abertos** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all datasets available in the Rondônia open data catalog."

**🤖 AI Agent:**
> I've retrieved the catalog. There are several datasets available, including 'Frequência de Servidores', 'Gastos com Diárias', and 'Obras Públicas'. Would you like details on a specific one?

---

**👤 You:**
> "Show me the payroll for state employees in January 2024."

**🤖 AI Agent:**
> Fetching payroll data for 2024-01... I found the records. You can see details for various departments. Do you want to search for a specific name or job title within this month?

---

**👤 You:**
> "Search for payments made to 'CONSTRUTORA' between 2023-01-01 and 2023-03-01."

**🤖 AI Agent:**
> I found several payment records for suppliers matching 'CONSTRUTORA' in that period. The largest payment was for R$ 150,000.00 from the 'Secretaria de Obras'. Would you like the full list of transactions?


## Installation & Usage

To install and use the **Rondônia Dados Abertos** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rondonia-dados-abertos](https://vinkius.com/mcp/rondonia-dados-abertos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
