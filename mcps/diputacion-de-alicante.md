# Diputación de Alicante MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/diputacion-de-alicante)
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


## Available Tools (19)
- **get_population_nuclei**: Get Population Nuclei dataset
- **get_population_register**: Get Population Register Evolution dataset
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
- **get_mayors**: Get Mayors (Historical) dataset
- **get_moors_and_christians_festivals**: Get Moors and Christians Festivals dataset
- **get_municipal_budgets**: Get Municipal Budgets dataset
- **get_official_local_festivals**: Get Official Local Festivals dataset
- **get_provincial_budget_evolution**: Get Provincial Budget Evolution dataset
- **get_provincial_corporation_members**: Get Provincial Corporation Members dataset
- **get_public_debt**: Get Public Debt dataset
- **get_staffing_levels**: Get Staffing Levels (Plantilla de Personal) dataset


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


## ❓ FAQ

**Q: How can I check the current debt levels for municipalities in Alicante?**
You can use the `get_live_debt` tool to retrieve the 'Deuda Viva' dataset, which contains financial data regarding the outstanding debt of local municipalities.

**Q: Is it possible to see the distribution of foreign residents by their country of origin?**
Yes. The `get_foreign_population_by_country` tool provides detailed statistics on the foreign population residing in the province, categorized by nationality.

**Q: Can I find information about local festivals like Moors and Christians?**
Absolutely. Use the `get_moors_and_christians_festivals` tool for specific data on those celebrations, or `get_official_local_festivals` for the general provincial festival calendar.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/diputacion-de-alicante](https://vinkius.com/mcp/diputacion-de-alicante)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Diputación de Alicante** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `diputacion-de-alicante` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Diputación de Alicante** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "diputacion-de-alicante": {
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
