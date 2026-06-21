# Trefle MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/trefle)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the world's largest botanical database — search for plants, species, and genera, and explore distribution data directly from your AI agent.

## Description
Connect to the **Trefle API** to empower your AI agent with comprehensive botanical knowledge. Access data on over 1 million plants, including taxonomy, distribution, and scientific metadata.

### What you can do

- **Plant & Species Discovery** — Search and list main plant species or dive deep into sub-taxa, varieties, and hybrids using `search_plants` and `list_species`.
- **Detailed Metadata** — Fetch complete scientific profiles, including family names, year of discovery, and botanical slugs with `get_plant` and `get_species`.
- **Taxonomy Exploration** — Browse through plant genera and understand the hierarchical classification of the plant kingdom via `list_genera`.
- **Geographic Distribution** — List WGSRPD distribution zones and identify which plants are native or introduced in specific regions using `list_distributions`.

### How it works

1. Subscribe to this server
2. Enter your Trefle API Token
3. Start exploring botanical data from Claude, Cursor, or any MCP client

### Who is this for?

- **Researchers & Botanists** — quickly verify taxonomy and distribution data without manual database queries.
- **Developers** — integrate plant data into apps or gardening tools via natural language.
- **Nature Enthusiasts** — learn about plant families and species characteristics through conversation.


## Available Tools
- **get_distribution_plants**: Use query_params to filter by establishment (e.g. {"filter[establishment]": "native"}).

List plants found in a specific distribution zone
- **get_genus**: Get details for a specific genus
- **get_plant**: Get details for a specific plant
- **get_species**: Get details for a specific species
- **list_distributions**: List all distribution zones
- **list_genera**: List all genera
- **list_plants**: Excludes forms, varieties, and subspecies.

List all main plant species
- **list_species**: List all species and sub-taxa
- **report_species_error**: Report an error in species data
- **search_plants**: Search through main plants
- **search_species**: Search through all species
- **submit_species_correction**: Submit a data correction for a species


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Trefle** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Lavandula' and show me the results."

**🤖 AI Agent:**
> I found several results for 'Lavandula'. The most prominent is Lavandula angustifolia (English lavender). Would you like to see the full details for this species?

---

**👤 You:**
> "List the first page of plant genera."

**🤖 AI Agent:**
> I've retrieved the first page of genera. It includes entries like 'Abies', 'Acacia', and 'Acer'. Which one would you like to explore further?

---

**👤 You:**
> "Get the details for the plant with slug 'rosa-canina'."

**🤖 AI Agent:**
> Fetching data for Rosa canina (Dog rose)... It belongs to the Rosaceae family and was first described in 1753. It is widely distributed across Europe and North Africa.


## ❓ FAQ

**Q: Can I search for plants using a simple text query?**
Yes, use the `search_plants` tool. It allows you to find main plant species by providing a query string like 'rose' or 'oak'.

**Q: How can I filter plants by a specific family, like Orchidaceae?**
You can use the `list_plants` tool and provide a JSON string in the `query_params` field, such as `{"filter[family_name]": "Orchidaceae"}`.

**Q: Is it possible to get info on sub-species and varieties?**
Absolutely. While `list_plants` focuses on main species, the `list_species` and `search_species` tools include all sub-taxa, varieties, and hybrids.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/trefle](https://vinkius.com/mcp/trefle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Trefle** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `trefle` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Trefle** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trefle": {
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
