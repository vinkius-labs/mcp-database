# Datos.gob.es (Catálogo Nacional) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datosgobes-catalogo-nacional)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access Spain's National Open Data Catalog — search datasets, filter by theme, publisher, or format, and retrieve public sector information directly.

## Description
Connect to the official **Datos.gob.es** API to explore Spain's vast repository of public sector information. This MCP server allows AI agents to query, filter, and analyze thousands of datasets from national, regional, and local administrations.

### What you can do

- **Dataset Discovery** — Search for specific datasets by title or browse the entire catalog with advanced pagination and sorting.
- **Advanced Filtering** — Narrow down results by publisher ID, specific themes (e.g., health, economy), or file formats like CSV, JSON, and RDF.
- **Geographic Analysis** — Filter data by spatial scope, including provinces, regions, or specific administrative levels.
- **Metadata Inspection** — Retrieve detailed metadata for any dataset, including its distributions, update frequency, and issuing body.
- **Public Sector Mapping** — List and inspect public sector organizations, provinces, and regions involved in the open data ecosystem.

### How it works

1. Subscribe to this server
2. The server connects to the public Datos.gob.es API
3. Start querying Spanish public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly find and inspect public datasets for research and reporting without manual browsing.
- **Developers** — identify API endpoints and data formats for integration into applications.
- **Policy Researchers** — track public sector transparency and data availability across different Spanish regions.


## Available Tools (22)
- **get_country_spain**: Get country-level information for Spain
- **get_dataset**: Get a specific dataset by its URI identifier
- **get_province**: g., Madrid).

Get a specific province by ID
- **get_public_sector**: g., comercio).

Get a specific primary sector by ID
- **get_region**: g., Comunidad-Madrid).

Get a specific Autonomous Community (Region) by ID
- **list_datasets_by_date**: Filter datasets by modification date range
- **list_datasets_by_format**: g., csv).

Filter datasets by format
- **list_datasets_by_keyword**: Filter datasets by keyword
- **list_datasets_by_publisher**: g., A16003011).

Filter datasets by publisher ID
- **list_datasets_by_spatial**: g., word1=Autonomia, word2=Pais-Vasco).

Filter datasets by geographic scope
- **list_datasets_by_theme**: g., hacienda).

Filter datasets by theme/category
- **list_datasets**: gob.es catalog.

Get all datasets from the catalog
- **list_distributions_by_dataset**: Get distributions by dataset ID
- **list_distributions_by_format**: g., csv).

Filter distributions by format
- **list_distributions**: Get all data distributions
- **list_provinces**: Get all provinces
- **list_public_sectors**: Get the taxonomy of primary sectors
- **list_publishers**: Get all publishers in the catalog
- **list_regions**: Get all Autonomous Communities (Regions)
- **list_spatial_options**: Get all geographic coverage options
- **list_themes**: Get all categories/themes
- **search_datasets_by_title**: Search datasets by title


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Datos.gob.es (Catálogo Nacional)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets related to 'transporte' in the Spanish open data catalog."

**🤖 AI Agent:**
> I've found several datasets related to 'transporte'. Notable entries include 'Transporte Terrestre de Viajeros' and 'Red de Carreteras'. Would you like the full details for any of these?

---

**👤 You:**
> "List all datasets that are available in CSV format."

**🤖 AI Agent:**
> I am retrieving datasets with CSV distributions... I've found a list of datasets including 'Censo de locales' and 'Presupuestos municipales'. I can provide the download links if you're interested.

---

**👤 You:**
> "Show me the themes or categories available in the Datos.gob.es catalog."

**🤖 AI Agent:**
> The catalog is organized into several themes such as 'Hacienda', 'Cultura y Ocio', 'Medio Ambiente', and 'Salud'. Which category would you like to explore?


## ❓ FAQ

**Q: How can I search for datasets containing a specific word in the title?**
Use the `search_datasets_by_title` tool. Provide the string you are looking for in the `title` parameter, and the agent will return all matching datasets from the national catalog.

**Q: Is it possible to filter datasets by a specific file format like CSV or JSON?**
Yes! Use the `list_datasets_by_format` tool and specify the format (e.g., 'csv', 'json', 'xlsx'). This will retrieve only the datasets that offer distributions in that format.

**Q: Can I find datasets belonging to a specific category like 'Health' or 'Environment'?**
Absolutely. Use the `list_datasets_by_theme` tool with the corresponding theme ID. You can first use `list_themes` to see all available categories in the catalog.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datosgobes-catalogo-nacional](https://vinkius.com/mcp/datosgobes-catalogo-nacional)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Datos.gob.es (Catálogo Nacional)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `datosgobes-catalogo-nacional` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Datos.gob.es (Catálogo Nacional)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "datosgobes-catalogo-nacional": {
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
