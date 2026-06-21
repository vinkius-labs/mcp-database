# GBIF MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gbif)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gbif-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gbif-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Search 2.4 billion biodiversity records — find any species on Earth with full taxonomy, observation locations, and geographic distribution from the Global Biodiversity Information Facility.

## Description
Connect your AI agent to the **Global Biodiversity Information Facility (GBIF)** — the largest open biodiversity database on Earth, aggregating data from 2,000+ institutions across 100+ countries.

### What you can do

- **Species Search** — Find any species by scientific name (Panthera leo) or common name (lion, blue whale, orchid) across 400K+ species with complete Linnaean taxonomy (Kingdom→Phylum→Class→Order→Family→Genus→Species)
- **Species Details** — Get comprehensive data for any species including vernacular names in multiple languages, taxonomic status, and direct GBIF links
- **Occurrence Records** — Find where a species has been observed worldwide with GPS coordinates, country, observation date, and specimen type. Filter by country using ISO-2 codes

### How it works

1. Subscribe to this server
2. Start exploring biodiversity immediately — no API key required

### Who is this for?

- **Conservation Biologists** — map species distributions and identify critical habitats for endangered species management
- **Ecologists & Naturalists** — verify species identifications and explore taxonomy for field research
- **Environmental Consultants** — assess biodiversity in specific regions for impact studies and regulatory compliance


## Available Tools
- **get_gbif_occurrences**: Optional country filter (ISO 2-letter code: US, BR, AU, GB).

Find where a species has been observed worldwide
- **get_gbif_species**: Get full species details with common names by GBIF key
- **search_gbif_species**: Returns full taxonomy (Kingdom→Phylum→Class→Order→Family→Genus), taxonomic status, and occurrence counts. Try: Panthera leo, orchid, blue whale, oak.

Search 2.4 billion biodiversity records for any species on Earth


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GBIF** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Tell me about the taxonomy and classification of the blue whale."

**🤖 AI Agent:**
> Balaenoptera musculus (Blue Whale): Kingdom Animalia → Phylum Chordata → Class Mammalia → Order Artiodactyla → Family Balaenopteridae → Genus Balaenoptera → Species B. musculus. Taxonomic status: Accepted. Common names: Blue Whale (en), Baleia-azul (pt), Ballena azul (es), Baleine bleue (fr). GBIF species key: 2440 — the largest animal ever known to have existed.

---

**👤 You:**
> "Where has the jaguar (Panthera onca) been observed in Brazil?"

**🤖 AI Agent:**
> Found 10 occurrence records for Panthera onca in Brazil (ISO: BR). Observations span from the Amazon basin (Manaus region, -3.1°, -60.0°) to the Pantanal wetlands (Mato Grosso do Sul, -19.5°, -57.0°) and Atlantic Forest fragments (São Paulo state). Most recent record: 2023-08-15. Basis of record: Human Observation, Machine Observation (camera trap).

---

**👤 You:**
> "Search for all orchid species in the GBIF database."

**🤖 AI Agent:**
> Found 10 results for 'orchid'. The Orchidaceae family is one of the largest flowering plant families with 28,000+ species. Top results include: Phalaenopsis (moth orchids — most popular houseplant orchid), Dendrobium (1,800+ species across Asia), Vanilla planifolia (the source of vanilla flavoring), and Cattleya (classic corsage orchid). Each with full Linnaean taxonomy and GBIF links.


## Installation & Usage

To install and use the **GBIF** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gbif](https://vinkius.com/mcp/gbif)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
