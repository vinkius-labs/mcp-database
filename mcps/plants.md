# Plants MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plants)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access a massive botanical database — search for plants, species, and distributions directly from any AI agent.

## Description
Connect to the **Trefle API** to explore global plant data. This server allows your AI to act as a digital botanist, retrieving taxonomic information, distribution maps, and plant characteristics.

### What you can do

- **Plant Discovery** — Search for plants by common or scientific names and list species with advanced filters.
- **Taxonomic Details** — Retrieve complete metadata, including images, growth characteristics, and genus information.
- **Geographical Distribution** — Explore plants based on WGSRPD distribution zones and slugs.
- **Species Variations** — List and search through detailed species, subspecies, and varieties.

### How it works

1. Subscribe to this server
2. Enter your Trefle API Token
3. Start exploring the botanical world from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Botanists** — quickly verify taxonomic data and distribution zones.
- **Gardeners & Enthusiasts** — find plant characteristics and images using natural language.
- **Developers** — integrate plant data into applications without manual API calls.


## Available Tools
- **correct_species**: Submit a data correction for a species
- **get_plant**: Get details for a specific plant
- **get_species**: Get details for a specific species
- **list_distribution_plants**: List plants found in a specific distribution zone
- **list_distributions**: List all distribution zones (WGSRPD standard)
- **list_genus**: List all genera
- **list_plants**: Use query_params for filter[FIELD], range[FIELD], or order[FIELD].

List all main plant species
- **list_species**: Use query_params for advanced filtering.

List all species, subspecies, and varieties
- **report_species_error**: Report an error in a species record
- **search_plants**: Search for plants by name
- **search_species**: Search for species by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plants** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Quercus robur' in the plant database."

**🤖 AI Agent:**
> I found 'Quercus robur' (Common Oak). It is a member of the Fagaceae family. Would you like to see its full growth characteristics or distribution map?

---

**👤 You:**
> "List all plants found in the 'brazil' distribution zone."

**🤖 AI Agent:**
> I've retrieved the list for the Brazil distribution zone. There are thousands of records, including 'Paubrasilia echinata' and various 'Cattleya' species. Do you want to filter this list by a specific genus?

---

**👤 You:**
> "Get the full taxonomic details for species ID 192034."

**🤖 AI Agent:**
> Fetching details for species 192034... This is 'Lavandula angustifolia'. It belongs to the genus Lavandula. I have data on its flower color (purple), foliage texture, and preferred soil pH.


## ❓ FAQ

**Q: How do I search for a specific plant like 'Lavender'?**
You can use the `search_plants` tool. Simply provide the name as the 'q' parameter, and the agent will return a list of matching plants from the database.

**Q: Can I find plants native to a specific region or country?**
Yes! Use the `list_distribution_plants` tool with the specific distribution zone slug (e.g., 'fra' for France or 'bra' for Brazil) to see plants found in that area.

**Q: What is the difference between get_plant and get_species?**
`get_plant` retrieves the main record for a plant, while `get_species` provides more granular taxonomic data, including specific varieties, subspecies, and detailed growth characteristics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plants](https://vinkius.com/mcp/plants)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plants** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `plants` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plants** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plants": {
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
