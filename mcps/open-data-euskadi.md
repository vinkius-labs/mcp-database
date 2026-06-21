# Open Data Euskadi MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-data-euskadi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access the official open data portal of the Basque Government — search grants, contracts, news, and execute complex SPARQL queries on Linked Open Data.

## Description
Connect to the **Open Data Euskadi** ecosystem and interact with the Basque Government's official public data through natural conversation. This server provides direct access to a vast catalog of administrative and semantic information.

### What you can do

- **Content Search** — Query the Euskadi.eus catalog for grants, public contracts, news, and administrative procedures using advanced filters.
- **Linked Open Data (LOD)** — Execute raw SPARQL queries against the GraphDB endpoint to retrieve structured RDF data for deep analysis.
- **Administrative Transparency** — Access real-time information on public announcements, board notices, and governmental publications.
- **Meteorological Data** — Retrieve specialized datasets, including weather information from Euskalmet when authorized.
- **Metadata Filtering** — Narrow down results by language, date ranges, and specific portal contexts to find exactly what you need.

### How it works

1. Subscribe to this server
2. Enter your Euskalmet JWT (optional for public data)
3. Start querying Basque public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts & Researchers** — perform complex semantic queries across public datasets without manual exports
- **Legal & Administrative Professionals** — track public grants, subsidies, and government contracts in real-time
- **Developers** — integrate official Basque government data and news feeds directly into your AI-driven workflows


## Available Tools
- **execute_sparql_query**: Execute a SPARQL query against Open Data Euskadi
- **search_euskadi_content**: Search the Euskadi.eus content catalog


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open Data Euskadi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for active grants (ayuda_subvencion) in the Euskadi content catalog."

**🤖 AI Agent:**
> I've searched the catalog. I found several active grants, including 'Digital Transformation Subsidies 2024' and 'SME Innovation Fund'. Would you like the specific metadata for any of these?

---

**👤 You:**
> "Execute a SPARQL query to list the first 10 datasets in the Linked Open Data graph."

**🤖 AI Agent:**
> Querying the LOD endpoint... I've retrieved the first 10 datasets. They include public transport schedules, environmental sensors, and administrative directories. Which one should we analyze?

---

**👤 You:**
> "Find news related to 'sustainability' in the Euskadi portal context."

**🤖 AI Agent:**
> I found 3 recent news articles regarding sustainability. The most recent is 'New Green Energy Initiative for 2025'. Would you like me to fetch the full content details?


## ❓ FAQ

**Q: How can I filter content by a specific language or date range?**
You can use the `metadata_filters` parameter in the `search_euskadi_content` tool. For example, use `documentLanguage.EQ.es` for Spanish or `procedureStartDate.BETWEEN.01/01/2023,31/12/2023` for dates.

**Q: Can I perform advanced semantic analysis on the data?**
Yes! Use the `execute_sparql_query` tool to run raw SPARQL queries against the Linked Open Data (LOD) endpoint. This allows you to traverse relationships in the RDF graph directly.

**Q: What types of administrative content can I search for?**
The `search_euskadi_content` tool allows you to filter by `content_type`. Common types include `ayuda_subvencion` (grants), `contratacion` (contracts), `noticia` (news), and `anuncio_tablon` (board notices).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-data-euskadi](https://vinkius.com/mcp/open-data-euskadi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Open Data Euskadi** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `open-data-euskadi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open Data Euskadi** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open-data-euskadi": {
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
