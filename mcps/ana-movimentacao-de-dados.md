# ANA (Movimentação de Dados) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ana-movimentacao-de-dados)
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


## ❓ FAQ

**Q: How can I search for flow data for a specific station?**
Use the `get_serie_vazao` tool by providing the `codigo_estacao`. You can also filter by `data_busca` to get data for a specific date.

**Q: Is it possible to update existing rainfall records?**
Yes, if you have the necessary permissions, you can use the `update_serie_chuva` tool with the updated JSON data body.

**Q: What information is included in the cross-section profile search?**
The `get_serie_perfil_transversal` tool retrieves morphological data of the riverbed at the station location, including depth and width measurements recorded in the series.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ana-movimentacao-de-dados](https://vinkius.com/mcp/ana-movimentacao-de-dados)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ANA (Movimentação de Dados)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ana-movimentacao-de-dados` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ANA (Movimentação de Dados)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ana-movimentacao-de-dados": {
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
