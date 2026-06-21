# Species MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/species)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/species-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/species-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the GBIF Backbone Taxonomy to search, match, and explore species data, hierarchies, and biological media directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Species** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the scientific name and details of the 'Red Panda'."

**🤖 AI Agent:**
> I found a match: *Ailurus fulgens* (ID: 2433668). It belongs to the family Ailuridae. Would you like to see its full taxonomic hierarchy or available media?

---

**👤 You:**
> "List all child taxa for the genus 'Panthera'."

**🤖 AI Agent:**
> Retrieving children for *Panthera* (ID: 2435194)... I've found several species including *Panthera leo* (Lion), *Panthera tigris* (Tiger), and *Panthera onca* (Jaguar).

---

**👤 You:**
> "Get descriptions and synonyms for the taxon with ID 5231190."

**🤖 AI Agent:**
> For Taxon ID 5231190 (*Monachus monachus*), I have retrieved 3 synonyms and detailed descriptions regarding its habitat and conservation status. Would you like me to summarize the text?


## Installation & Usage

To install and use the **Species** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/species](https://vinkius.com/mcp/species)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
