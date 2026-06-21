# Trefle MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/trefle)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/trefle-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/trefle-mcp)
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


## Installation & Usage

To install and use the **Trefle** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/trefle](https://vinkius.com/mcp/trefle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
