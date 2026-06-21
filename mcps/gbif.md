# GBIF MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gbif)
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


## ❓ FAQ

**Q: What types of organisms are covered in GBIF?**
GBIF covers all life on Earth across all kingdoms: Animalia (animals), Plantae (plants), Fungi (mushrooms, yeasts), Bacteria, Archaea, Chromista (algae, diatoms), and Protozoa. From microscopic bacteria to blue whales, from orchids to ancient ferns — if a species has been scientifically described, GBIF likely has records for it.

**Q: Is GBIF data free and do I need to register?**
Yes, GBIF data is completely free and open under CC0, CC-BY, or CC-BY-NC licenses. No registration or API key is required for programmatic access. GBIF is funded by governments of 40+ member countries and endorsed by the United Nations Environment Programme.

**Q: Can I filter species observations by country or region?**
Yes! The occurrence search supports country filtering using ISO-2 country codes (US for United States, BR for Brazil, AU for Australia, GB for United Kingdom, JP for Japan, etc.). This allows you to find exactly where a species has been observed in a specific country with GPS coordinates and dates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gbif](https://vinkius.com/mcp/gbif)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GBIF** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gbif` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GBIF** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gbif": {
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
