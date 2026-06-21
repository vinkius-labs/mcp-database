# IBGE Localidades — Cidades do Brasil MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ibge-localidades-cidades-do-brasil)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Give your AI agent a precise map of Brazil: all 5,570 municipalities, 27 states, 5 macro-regions, metropolitan areas, and the complete administrative hierarchy — zero authentication required.

## Description
Connect your AI agent to the **official IBGE geographic database** — the authoritative source used by every government, fintech, and logistics company operating in Brazil.

### What you can do
- **5,570 Municipalities** — Search any city by IBGE code with mesoregion, microregion, and state hierarchy
- **27 States (UFs)** — Complete Brazilian federation with codes, abbreviations, and macro-region associations
- **5 Macro-Regions** — Norte, Nordeste, Centro-Oeste, Sudeste, Sul with all nested structure
- **Metropolitan Regions** — São Paulo, Rio de Janeiro, Belo Horizonte and all other metropolitan areas by state

### How it works
1. Subscribe — it's free and instant.
2. No API keys needed — IBGE data is open government.
3. Ask your AI about any city, state, or region in Brazil.

### Who is this for?
Fintechs, logistics companies, CRM systems, address validation services, market researchers, and anyone building AI agents that need precise Brazilian geographic intelligence.


## Available Tools
- **list_estados**: List all Brazilian states (UFs)
- **get_municipios_por_uf**: Use the 2-letter UF abbreviation (e.g., SP, RJ, MG, BA).

List all municipalities in a Brazilian state
- **get_municipio**: Use the 7-digit IBGE code.

Get municipality details by IBGE code
- **list_regioes**: List the 5 macro-regions of Brazil
- **list_regioes_metropolitanas**: List metropolitan regions by state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBGE Localidades — Cidades do Brasil** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all municipalities in the state of São Paulo"

**🤖 AI Agent:**
> 🇧🇷 **São Paulo — 645 Municipalities**

1. Adamantina (3500105)
2. Adolfo (3500204)
3. Aguaí (3500303)
...
645. Votorantim (3557006)

São Paulo is Brazil's largest state by municipality count, representing 11.6% of all Brazilian cities.

---

**👤 You:**
> "What is the IBGE code for the city of Rio de Janeiro?"

**🤖 AI Agent:**
> 📍 **Rio de Janeiro**

- IBGE Code: 3304557
- Microregion: Rio de Janeiro
- Mesoregion: Metropolitana do Rio de Janeiro
- State: RJ (33)
- Macro-region: Sudeste

---

**👤 You:**
> "What are the metropolitan regions in the state of Minas Gerais?"

**🤖 AI Agent:**
> 🏙️ **Minas Gerais — Metropolitan Regions**

1. RM de Belo Horizonte (34 municipalities, pop ~5.8M)
2. RM do Vale do Aço (28 municipalities)
3. Colar Metropolitano (16 municipalities)

The Belo Horizonte metro area is Brazil's third largest, after São Paulo and Rio de Janeiro.


## ❓ FAQ

**Q: Do I need an API key?**
No! IBGE data is 100% open government data. This server works instantly with zero configuration — just subscribe and start querying Brazilian geography.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibge-localidades-cidades-do-brasil](https://vinkius.com/mcp/ibge-localidades-cidades-do-brasil)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IBGE Localidades — Cidades do Brasil** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ibge-localidades-cidades-do-brasil` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IBGE Localidades — Cidades do Brasil** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ibge-localidades-cidades-do-brasil": {
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
