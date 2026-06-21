# Sergipe Dados Abertos MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sergipe-dados-abertos)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sergipe-dados-abertos-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sergipe-dados-abertos-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access public data from the State of Sergipe, Brazil—including expenditures, revenues, personnel, and budget execution—directly from any AI agent.

## Description
Connect to the **Sergipe Transparency Portal** and query official government data through natural conversation. This server provides direct access to the open data infrastructure of the State of Sergipe, Brazil.

### What you can do

- **Expenditures (Despesas)** — Query detailed state spending, including payments to suppliers, sub-elements, and inter-governmental transfers by fiscal year.
- **Revenues (Receitas)** — Monitor state collection, including tax revenue (ICMS, IPVA) and federal transfers with specific date ranges.
- **Personnel (Servidores)** — Access information about the state workforce, including active and retired employees, positions, and salary data.
- **Budget (Orçamento)** — Inspect the Annual Budget Law (LOA) and track real-time budget execution for any given fiscal year.

### How it works

1. Subscribe to this server
2. The server connects to the official Sergipe Open Data API
3. Start auditing public accounts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Journalists & Researchers** — quickly extract spending data and personnel counts for investigative reporting
- **Citizens & Activists** — monitor how public resources are being allocated in the state of Sergipe
- **Data Analysts** — fetch clean JSON data for fiscal analysis without manual CSV downloads


## Available Tools
- **get_despesas**: Get state expenditures (Despesas)
- **get_orcamento**: Get budget data (Orçamento)
- **get_receitas**: Get state revenues (Receitas)
- **get_servidores**: Get personnel information (Servidores)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sergipe Dados Abertos** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the state expenditures for Sergipe in 2023."

**🤖 AI Agent:**
> I've retrieved the expenditure data for 2023. The state processed various payments including supplier contracts and transfers. Would you like to see the breakdown by month or a specific government body?

---

**👤 You:**
> "What were the total revenues collected between January and March 2024?"

**🤖 AI Agent:**
> Querying revenue data... For the first quarter of 2024, the state collected revenues from taxes like ICMS and federal transfers. I can provide the exact totals for each category if you'd like.

---

**👤 You:**
> "List the active personnel in the state government for the last available month."

**🤖 AI Agent:**
> I've accessed the personnel records. There are thousands of active employees across various departments. Would you like to see a summary of positions or filter by a specific employment bond type?


## Installation & Usage

To install and use the **Sergipe Dados Abertos** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sergipe-dados-abertos](https://vinkius.com/mcp/sergipe-dados-abertos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
