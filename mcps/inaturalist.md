# iNaturalist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/inaturalist)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Explore biodiversity data — search wildlife observations, identify species, find taxa and discover nature projects.

## Description
Connect to **iNaturalist** and explore the world's largest biodiversity database through natural conversation — no API key needed for public data.

### What you can do

- **Observations** — Search millions of wildlife observations with species IDs, photos and locations
- **Taxa Search** — Find species by name with scientific names, common names and conservation status
- **Species Counts** — Get species observation counts by area, user or taxon
- **Identifications** — Browse community identifications and expert species IDs
- **Projects** — Discover community-curated biodiversity projects
- **User Activity** — View any user's observation history

### How it works

1. Subscribe to this server
2. No API key needed for public endpoints
3. Start exploring nature data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Naturalists** — discover species in your area, track biodiversity trends and find local observation projects
- **Researchers** — access species observation data, taxonomic information and geographic distributions
- **Educators** — explore biodiversity with students, find local species examples and teach taxonomy


## Available Tools (10)
- **autocomplete_taxa**: Returns the top 10 matching taxa with names and ranks. Useful for building search UIs or quickly finding taxon IDs.

Autocomplete taxon names
- **get_controlled_terms**: These include standardized values for life stage, plant phenology, sex, evidence of presence and more. Useful for understanding annotation options.

Get controlled terms (standardized vocabularies)
- **get_identifications**: Filter by taxon or user. Each identification includes the proposed species, the observation it was made on, and the user who made it.

Get identifications made by users
- **get_observation**: Get a specific iNaturalist observation by ID
- **get_observations_by_user**: Filter by quality grade and set result limit. Returns observations with species, photos and dates.

Get observations by a specific user
- **get_projects**: Projects are community-curated collections of observations. Filter by place and set result limit.

Search for iNaturalist projects
- **get_species_counts**: Useful for biodiversity surveys and understanding which species are most commonly observed in an area or by a user. Filter by taxon, place or user.

Get species observation counts grouped by taxon
- **get_taxon**: Returns scientific name, common names, rank, ancestry, conservation status, establishment means and Wikipedia URL.

Get details for a specific taxon
- **search_observations**: Supports powerful filters: free-text query, taxon ID, user, place/location, quality grade (research/needs_id/casual), date range, and whether photos are required. Returns observations with species names, photos, locations, dates and observer info. Pagination: max 200 per page.

Search iNaturalist observations
- **search_taxa**: Returns taxa with scientific names, common names, ranks (species, genus, family, etc.), conservation status and observation counts. Supports filtering by rank.

Search for taxa (species, genera, families, etc.)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **iNaturalist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for monarch butterfly observations in California."

**🤖 AI Agent:**
> Found 12,500+ monarch butterfly (Danaus plexippus) observations in California. Recent observations from San Francisco, Monterey and Los Angeles areas. Most are research-grade with photos.

---

**👤 You:**
> "What are the most commonly observed species this month?"

**🤖 AI Agent:**
> Top observed species: 1. Rock Pigeon (45K observations), 2. European Honey Bee (38K), 3. Mourning Cloak butterfly (32K), 4. White-tailed Deer (28K), 5. Mallard Duck (25K).

---

**👤 You:**
> "Tell me about the Red Fox (Vulpes vulpes)."

**🤖 AI Agent:**
> Red Fox (Vulpes vulpes) — Species, Kingdom: Animalia, Phylum: Chordata, Class: Mammalia, Order: Carnivora, Family: Canidae. 200K+ observations worldwide. Introduced and native populations across North America, Europe, Asia and Australia.


## ❓ FAQ

**Q: Do I need an iNaturalist account?**
No! All public endpoints work without authentication. Just start searching. For write operations (creating observations, identifications), you'd need OAuth2 authentication.

**Q: What kind of species data is available?**
iNaturalist has 150M+ observations of plants, animals, fungi, insects and more. Each observation includes species ID, photos, location, date, observer info and community identifications.

**Q: Can I search for species in my area?**
Yes! Use search_observations with place_id, or lat/lng/radius parameters to filter by location. You can also use get_species_counts with place_id to see which species are most commonly observed in an area.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inaturalist](https://vinkius.com/mcp/inaturalist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **iNaturalist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `inaturalist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **iNaturalist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "inaturalist": {
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
