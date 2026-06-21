# IBGE Agregados (SIDRA) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ibge-agregados-sidra)
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


## ❓ FAQ

**Q: How can I find specific surveys related to a topic like 'Employment'?**
Use the `list_agregados` tool and provide a keyword in the `assunto` parameter. The agent will return a list of all relevant aggregate tables and their IDs.

**Q: Can I see which years or months are available for a specific table ID?**
Yes! By using the `get_periodos` tool with the specific Aggregate ID, you can retrieve all available time intervals for that dataset.

**Q: How do I know if a table has data at the city level (municípios)?**
Run the `get_localidades` tool for the target Aggregate ID. It will list all supported geographic levels, such as 'Brasil', 'Unidade da Federação', or 'Município'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibge-agregados-sidra](https://vinkius.com/mcp/ibge-agregados-sidra)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IBGE Agregados (SIDRA)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ibge-agregados-sidra` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IBGE Agregados (SIDRA)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ibge-agregados-sidra": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
