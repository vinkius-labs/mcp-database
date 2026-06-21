# IBGE Pesquisas — Brasil Cidades MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ibge-pesquisas-brasil-cidades)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Query the engine behind Brasil Cidades: health, education, economy, and quality-of-life indicators for every Brazilian municipality — rank cities, compare regions, and build data-driven policy analysis.

## Description
Access the same data engine powering the official **Brasil Cidades** portal — the IBGE's most comprehensive municipal indicator database.

### What you can do
- **List All Surveys** — Browse the complete IBGE research catalog (Census, PNAD, POF, Agricultural Census, etc.)
- **Municipal Indicators** — Health, education, income, sanitation, and infrastructure data per city
- **Cross-Survey Results** — Query any indicator across any survey and time period
- **City Rankings** — Rank municipalities by any indicator (best HDI, highest GDP per capita, etc.)

### Who is this for?
Urban planners, public policy researchers, ESG analysts, journalists, and data scientists building Brazilian city intelligence systems.


## Available Tools
- **list_pesquisas**: List all IBGE surveys and research programs
- **get_indicadores**: Use survey ID (e.g., 33 for Censo Demográfico, 38 for Produção Agrícola Municipal).

Get indicators from a specific IBGE survey
- **get_resultados**: Localities can be: BR (Brazil), UF code (e.g., 33 for RJ), or municipality IBGE code.

Get survey results for specific municipalities
- **get_ranking_indicador**: Rank municipalities by a specific indicator


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBGE Pesquisas — Brasil Cidades** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the education indicators for the city of Curitiba?"

**🤖 AI Agent:**
> 📚 **Curitiba — Education Indicators**

- Literacy rate: 97.8%
- Average schooling: 10.9 years
- IDEB (primary): 6.8
- School enrollment (6-14): 98.2%
- Higher education rate: 32.1%

Curitiba ranks in the top 5% of Brazilian municipalities for education.

---

**👤 You:**
> "Which Brazilian cities have the highest GDP per capita?"

**🤖 AI Agent:**
> 🏆 **Top 5 — GDP Per Capita**

1. São Desidério (BA) — R$ 309K
2. Paulínia (SP) — R$ 258K
3. Louveira (SP) — R$ 241K
4. Triunfo (RS) — R$ 234K
5. São Francisco do Conde (BA) — R$ 221K

Small industrial and agribusiness cities dominate the top.

---

**👤 You:**
> "Compare health indicators between São Paulo and Salvador"

**🤖 AI Agent:**
> 🏥 **Health Comparison**

| Indicator | São Paulo | Salvador |
|-----------|-----------|----------|
| Life expect. | 77.3 yrs | 73.8 yrs |
| Infant mort. | 10.2‰ | 15.4‰ |
| Physicians | 4.2/1000 | 2.8/1000 |
| Hospital beds | 3.1/1000 | 2.4/1000 |


## ❓ FAQ

**Q: Is this the same data as the Brasil Cidades portal?**
Yes! This server accesses the **exact same API** that powers the official [Brasil Cidades](https://cidades.ibge.gov.br) portal — the IBGE's premier municipal indicator platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibge-pesquisas-brasil-cidades](https://vinkius.com/mcp/ibge-pesquisas-brasil-cidades)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IBGE Pesquisas — Brasil Cidades** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ibge-pesquisas-brasil-cidades` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IBGE Pesquisas — Brasil Cidades** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ibge-pesquisas-brasil-cidades": {
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
