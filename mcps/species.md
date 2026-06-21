# Species MCP Server

Access the GBIF Backbone Taxonomy to search, match, and explore species data, hierarchies, and biological media directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/species)

## Overview
**Category:** knowledge-management
**Tools Count:** 10

## Description
Connect to the **GBIF Backbone Taxonomy**, the most comprehensive database of biological names and classifications. This server enables your AI to act as a digital biologist, navigating millions of species records with precision.

### What you can do

- **Taxonomic Search & Matching** — Use `search_species` or `match_species` to find correct scientific names and resolve fuzzy queries against the global backbone.
- **Biological Hierarchy** — Explore the tree of life using `get_species_children` and `get_species_parents` to navigate from kingdoms down to subspecies.
- **Rich Metadata** — Retrieve detailed descriptions, literature references, and synonyms to understand the full context of a taxon via `get_species_descriptions` and `get_species_synonyms`.
- **Visual & Media Data** — Access images and multimedia records associated with specific species using the `get_species_media` tool.

### How it works

1. Subscribe to this server
2. Configure your access (Public or API Key)
3. Start exploring biodiversity data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Scientists** — Quickly verify taxonomic statuses and hierarchies without manual database lookups.
- **Educators & Students** — Explore biological relationships and find media for educational content.
- **Developers** — Integrate reliable species data into environmental or biological applications.


## Available Tools
- **get_species_children**: List child taxa for a specific taxon
- **get_species_descriptions**: Retrieve text descriptions for a specific taxon
- **get_species**: Retrieve detailed information for a specific taxon
- **match_species**: Match a scientific name against the GBIF Backbone Taxonomy
- **get_species_media**: Retrieve images and other media for a specific taxon
- **get_species_parents**: List parent taxa for a specific taxon
- **get_species_references**: Retrieve literature references for a specific taxon
- **search_species**: Search for species and higher taxa
- **suggest_species**: Quickly find scientific names for autocomplete or search suggestions
- **get_species_synonyms**: List taxonomic synonyms for a specific taxon


## Installation & Usage

To install and use the **Species** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/species](https://vinkius.com/mcp/species)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
