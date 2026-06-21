# TCE-SP (Audesp) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tce-sp-audesp)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tce-sp-audesp-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tce-sp-audesp-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access public transparency data from the São Paulo State Court of Auditors (TCE-SP) — query municipal expenses and revenues directly.

## Description
Connect to the **TCE-SP Audesp** system to audit and analyze public spending across municipalities in the state of São Paulo. This server provides direct access to the official transparency portal data.

### What you can do

- **Municipality Lookup** — List all cities under TCE-SP jurisdiction and retrieve their unique slugs for precise querying
- **Expense Analysis** — Fetch detailed expense (despesas) records for any municipality, filtered by fiscal year and month
- **Revenue Tracking** — Access revenue (receitas) data to monitor municipal collections and budget performance
- **Fiscal Auditing** — Use AI to compare spending patterns and identify fiscal trends across different periods

### How it works

1. Subscribe to this server
2. Enter your API access credentials or token
3. Start querying public data from any MCP-compatible client like Claude or Cursor

### Who is this for?

- **Journalists & Researchers** — quickly extract fiscal data for investigative reporting without manual portal navigation
- **Public Managers** — monitor municipal performance and compare budget execution against historical data
- **Citizens & Activists** — promote transparency by easily accessing how public resources are being allocated


## Available Tools
- **list_despesas**: List expenses for a specific municipality, year, and month
- **list_municipios**: List all municipalities under TCE-SP jurisdiction
- **list_receitas**: List revenues for a specific municipality, year, and month


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TCE-SP (Audesp)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all municipalities available in the TCE-SP system."

**🤖 AI Agent:**
> I've retrieved the list of municipalities. There are hundreds of cities available, including 'santos', 'campinas', and 'sao-bernardo-do-campo'. Which one would you like to analyze?

---

**👤 You:**
> "Show me the expenses for the municipality of 'santos' in January 2023."

**🤖 AI Agent:**
> Fetching expenses for Santos (01/2023)... I've found the detailed records. The data includes operational costs, personnel expenses, and investments made during that period.

---

**👤 You:**
> "What were the revenues for 'campinas' in the year 2022, month 12?"

**🤖 AI Agent:**
> Querying revenues for Campinas (12/2022)... The report shows the total collection for the month, including tax revenues and state transfers.


## Installation & Usage

To install and use the **TCE-SP (Audesp)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tce-sp-audesp](https://vinkius.com/mcp/tce-sp-audesp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
