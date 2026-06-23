# ANP (Revendedores de Combustíveis) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/anp-revendedores-de-combustiveis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access official Brazilian fuel and LPG reseller data from ANP — query gas stations and cooking gas providers by location or CNPJ.

## Description
Connect to the **ANP (Agência Nacional do Petróleo, Gás Natural e Biocombustíveis)** database to retrieve real-time information about authorized resellers across Brazil through natural conversation.

### What you can do

- **Automotive Fuel Resellers** — Search for gas stations using filters like state (UF), municipality, or specific CNPJ via the `list_combustivel_resellers` tool.
- **LPG (Cooking Gas) Resellers** — Locate authorized GLP distributors and resellers nationwide using the `list_glp_resellers` tool.
- **Public Data Verification** — Verify the registration and status of fuel providers directly from the official regulatory source.
- **Geographic Analysis** — List all resellers within a specific city or state to understand regional coverage and availability.

### How it works

1. Subscribe to this server
2. Enter your ANP API Access Key (if required)
3. Start querying Brazilian energy and fuel data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Market Analysts** — track the distribution of fuel resellers in different regions for competitive analysis
- **Logistics & Fleet Managers** — identify authorized refueling points and verify reseller credentials
- **Compliance Officers** — verify the legal status of resellers against official government records


## Available Tools (2)
- **list_combustivel_resellers**: Can be filtered by CNPJ, state (UF), and municipality.

List automotive fuel resellers
- **list_glp_resellers**: Can be filtered by CNPJ, state (UF), and municipality.

List LPG (cooking gas) resellers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ANP (Revendedores de Combustíveis)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all automotive fuel resellers in the city of 'São Paulo', SP."

**🤖 AI Agent:**
> I've retrieved the list of authorized fuel resellers in São Paulo (SP). There are multiple entries; would you like to see the first page of results or filter by a specific CNPJ?

---

**👤 You:**
> "Find LPG (cooking gas) resellers in the state of Rio de Janeiro (RJ)."

**🤖 AI Agent:**
> Searching for GLP resellers in RJ... I found several authorized distributors. You can further narrow this down by municipality if needed.

---

**👤 You:**
> "Check the status of the reseller with CNPJ 00000000000191."

**🤖 AI Agent:**
> Querying ANP for CNPJ 00000000000191... I have found the registration details. The reseller is currently listed as authorized for automotive fuel sales.


## ❓ FAQ

**Q: Can I search for a specific gas station using its CNPJ?**
Yes! Use the `list_combustivel_resellers` tool and provide the `cnpj` parameter. The agent will return the registration details and authorization status for that specific tax ID.

**Q: How do I list all cooking gas resellers in a specific city?**
Use the `list_glp_resellers` tool and specify the `municipio` and `uf` (state abbreviation). This will return a list of all authorized LPG providers in that location.

**Q: Does the tool support pagination for large result sets?**
Yes. Both `list_combustivel_resellers` and `list_glp_resellers` include a `numeropagina` parameter, allowing you to navigate through multiple pages of data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anp-revendedores-de-combustiveis](https://vinkius.com/mcp/anp-revendedores-de-combustiveis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ANP (Revendedores de Combustíveis)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `anp-revendedores-de-combustiveis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ANP (Revendedores de Combustíveis)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "anp-revendedores-de-combustiveis": {
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
