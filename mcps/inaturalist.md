# iNaturalist MCP Server

Explore biodiversity data — search wildlife observations, identify species, find taxa and discover nature projects.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/inaturalist)

## Overview
**Category:** data-management
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **iNaturalist** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inaturalist](https://vinkius.com/mcp/inaturalist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
