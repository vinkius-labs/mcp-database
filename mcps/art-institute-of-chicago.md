# Art Institute of Chicago MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/art-institute-of-chicago)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/art-institute-of-chicago-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/art-institute-of-chicago-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search and explore the Art Institute of Chicago's digital collection—artworks, artists, and gallery locations.

## Description
Access one of the world's most impressive art collections directly through your AI agent. The **Art Institute of Chicago** MCP server allows you to query thousands of artworks, research artist biographies, and explore the museum's physical and digital archives.

### What you can do

- **Artwork Discovery** — Search the entire collection by keyword or list artworks with specific metadata fields and pagination.
- **Artist Research** — Retrieve detailed information about 'agents' (artists, designers, and contributors) including their historical context.
- **IIIF Integration** — Fetch IIIF Manifests for artworks to access high-resolution image data and structural metadata.
- **Museum Geography** — Explore physical gallery spaces and the places associated with the origin of various pieces.
- **Deep Metadata** — Access specific fields like exhibition history, provenance, and technical descriptions for any object in the collection.

### How it works

1. Subscribe to this server
2. Provide a User-Agent string (used to identify your requests to the AIC API)
3. Start exploring art history from Claude, Cursor, or any MCP client

### Who is this for?

- **Educators & Students** — Quickly gather facts, artist dates, and artwork descriptions for research or lesson planning.
- **Designers & Creatives** — Find inspiration from centuries of human creativity with direct access to high-quality metadata.
- **Art Historians** — Query specific collection subsets and retrieve technical manifests without manual API calls.


## Available Tools
- **get_agent**: Get details for a specific agent (artist)
- **get_article**: Get details for a specific article
- **get_artwork_manifest**: Get IIIF Manifest for a specific artwork
- **get_artwork**: Get details for a specific artwork
- **get_event**: Get details for a specific event
- **get_exhibition**: Get details for a specific exhibition
- **get_gallery**: Get details for a specific gallery
- **get_place**: Get details for a specific place
- **get_product**: Get details for a specific product
- **get_publication**: Get details for a specific publication
- **get_tour**: Get details for a specific tour
- **list_agents**: List agents (artists) in the collection
- **list_articles**: List articles
- **list_artworks**: List artworks in the Art Institute of Chicago collection
- **list_events**: List events
- **list_exhibitions**: List exhibitions
- **list_galleries**: List physical gallery spaces in the museum
- **list_places**: List places associated with artworks
- **list_products**: List products (Museum shop items)
- **list_publications**: List publications
- **list_tours**: List tours
- **search_agents**: Search agents (artists)
- **search_articles**: Search articles
- **search_artworks**: Search artworks in the Art Institute of Chicago collection
- **search_events**: Search events
- **search_exhibitions**: Search exhibitions
- **search_galleries**: Search galleries
- **search_places**: Search places
- **search_products**: Search products
- **search_publications**: Search publications
- **search_tours**: Search tours


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Art Institute of Chicago** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for artworks by Georges Seurat in the Art Institute of Chicago collection."

**🤖 AI Agent:**
> I found several artworks by Georges Seurat. The most famous is 'A Sunday on La Grande Jatte — 1884' (ID: 27992). Would you like to see the full details or the IIIF manifest for this painting?

---

**👤 You:**
> "Get the details for artwork ID 16568."

**🤖 AI Agent:**
> Artwork 16568 is 'The Old Guitarist' by Pablo Picasso, created in 1903. It is an oil on panel painting from his Blue Period. It is currently located in Gallery 249.

---

**👤 You:**
> "List the first 5 galleries in the museum."

**🤖 AI Agent:**
> Here are the first 5 galleries: Gallery 101 (Ancient Art), Gallery 102, Gallery 103, Gallery 104, and Gallery 105. Would you like to know which artworks are currently displayed in any of these?


## Installation & Usage

To install and use the **Art Institute of Chicago** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/art-institute-of-chicago](https://vinkius.com/mcp/art-institute-of-chicago)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
