# Paleobiology Database MCP Server

Access the world's largest fossil database — query occurrences, analyze taxonomic diversity, and explore geological intervals directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/paleobiology-database)

## Overview
**Category:** databases
**Tools Count:** 27

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


## Installation & Usage

To install and use the **Paleobiology Database** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paleobiology-database](https://vinkius.com/mcp/paleobiology-database)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
