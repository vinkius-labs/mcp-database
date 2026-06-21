# Paleobiology Database MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/paleobiology-database)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access the world's largest fossil database — query occurrences, analyze taxonomic diversity, and explore geological intervals directly from your AI agent.

## Description
Connect to the **Paleobiology Database (PBDB)** and turn your AI agent into a specialized paleontological researcher. Access millions of records spanning the history of life on Earth.

### What you can do

- **Fossil Occurrences** — Search for specific fossil records using taxonomic names, geographic coordinates, or temporal filters like 'Jurassic' or 'Cretaceous'.
- **Diversity Analysis** — Tabulate and visualize fossil diversity over time to understand extinction events and evolutionary radiations.
- **Taxonomic Hierarchy** — Explore the tree of life, from broad phyla down to specific species and their synonyms.
- **Geographic Clustering** — Summarize fossil finds into geographic clusters to identify high-density fossil beds and ancient migration patterns.
- **Geological Context** — Retrieve detailed information on time scales, strata, and intervals to place every find in its correct temporal context.

### How it works

1. Subscribe to this server
2. (Optional) Enter your PBDB API Key if you have one for higher rate limits
3. Start exploring Earth's biological history through natural language queries

### Who is this for?

- **Researchers & Academics** — quickly pull occurrence data and diversity metrics for papers and analysis.
- **Students & Educators** — explore evolutionary history and fossil distributions through interactive AI-guided discovery.
- **Science Enthusiasts** — satisfy your curiosity about prehistoric life by querying the same data used by professional paleontologists.


## Available Tools
- **autocomplete_combined**: General auto-completion across multiple record types (taxa, strata, intervals, people)
- **autocomplete_strata**: Auto-completion for strata names
- **autocomplete_taxa**: Auto-completion for taxonomic names
- **get_collection**: Get information about a single fossil collection
- **get_collections_summary**: Geographic summary of collections (clustering)
- **get_config**: Returns database configuration info (ranks, continents, countries, lithologies, environments)
- **get_occurrence**: Get information about a single fossil occurrence
- **get_occurrences_diversity**: Tabulate fossil diversity over time (full computation)
- **get_occurrences_geosum**: Summarize occurrences into geographic clusters
- **get_occurrences_prevalence**: Get the most prevalent taxa in a selected set of occurrences
- **get_occurrences_quickdiv**: Quick tabulation of fossil diversity over time
- **get_occurrences_taxa**: Get taxonomic hierarchy of a selected set of occurrences
- **get_opinion**: Get information about a single taxonomic opinion
- **get_reference**: Get information about a single bibliographic reference
- **get_specimen**: Get information about a single specimen
- **get_taxon**: Get information about a single taxonomic name
- **list_collections**: List fossil collections based on filters
- **list_intervals**: List geological time intervals (e.g., Cretaceous)
- **list_occurrences**: List fossil occurrences based on filters
- **list_opinions**: List taxonomic opinions based on filters
- **list_references**: List bibliographic references based on filters
- **list_specimen_measurements**: List measurements associated with specimens
- **list_specimens**: List specimens based on filters
- **list_strata**: List geological strata (formations, groups, members)
- **list_taxa**: List taxa, children, or parents
- **list_timescales**: List available geological time scales
- **match_reference**: Check for a matching reference in the PBDB database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paleobiology Database** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all Tyrannosaurus occurrences recorded in the Cretaceous period."

**🤖 AI Agent:**
> I've searched the database for Tyrannosaurus in the Cretaceous. I found several occurrences, including specimens from the Hell Creek Formation (Montana) and the Lance Formation (Wyoming). Would you like the specific IDs for these records?

---

**👤 You:**
> "Show me the diversity of Trilobites over time."

**🤖 AI Agent:**
> Generating diversity tabulation for Trilobita... The data shows a peak in diversity during the Ordovician period, followed by a gradual decline until their extinction at the end of the Permian. I can provide a breakdown by geological interval if you'd like.

---

**👤 You:**
> "List fossil collections found in the geographic area of Montana, USA."

**🤖 AI Agent:**
> I've filtered collections for the Montana region (approx. lat 44-49, lng -116 to -104). I found numerous collections, primarily from the Cretaceous and Paleogene, including many dinosaur and early mammal sites. Should I list the most recent ones?


## ❓ FAQ

**Q: Can I search for fossils within a specific geological time period like the Cretaceous?**
Yes! Use the `list_occurrences` tool and provide the period name in the `interval` parameter. The agent will return all recorded fossil occurrences from that specific time block.

**Q: How do I analyze the diversity of a specific group of animals over time?**
You can use the `get_occurrences_diversity` or `get_occurrences_quickdiv` tools. By providing a `base_name` (like 'Trilobita'), the agent will generate a tabulation of how many different taxa existed across different geological intervals.

**Q: Can I find fossil collections based on geographic coordinates?**
Absolutely. The `list_collections` and `list_occurrences` tools allow you to specify a bounding box using `lngmin`, `lngmax`, `latmin`, and `latmax` to find all records within a specific map area.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paleobiology-database](https://vinkius.com/mcp/paleobiology-database)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paleobiology Database** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `paleobiology-database` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paleobiology Database** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paleobiology-database": {
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
