# OpenFarm Agriculture MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openfarm-agriculture)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/openfarm-agriculture-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/openfarm-agriculture-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access crowdsourced agricultural data — search for crops, growing guides, and planting instructions.

## Description
Connect your AI agent to **OpenFarm**, the world's most comprehensive open-source database for farming and gardening. Access a wealth of knowledge on thousands of plant species and crowdsourced growing techniques.

### What you can do

- **Crop Discovery** — Search for edible and ornamental plants to get their scientific names and descriptions
- **Growing Guides** — Access detailed instructions on how to grow specific crops in different conditions
- **Technical Specs** — Get data on sun requirements, sowing methods, and optimal spacing
- **Gardening Intelligence** — Use AI to plan your garden based on crowdsourced best practices

### How it works

1. Subscribe to this server
2. No API Key required for public data access
3. Start asking about plants and how to grow them directly via chat

### Who is this for?

- **Home Gardeners** — find quick tips on how to care for your plants
- **Urban Farmers** — access technical data for intensive crop production
- **Agricultural Researchers** — explore a vast database of crowdsourced plant data


## Available Tools
- **get_species_details**: Critical for precision agriculture and biodiversity assessments.

Get detailed taxonomic and growing data for a specific species
- **list_species**: Each species includes taxonomic classification, growth form, and habitat data. Use without a query to browse, or with a query to search.

Search for plant species, optionally filtered by name
- **search_crops**: io botanical database for crops matching the query. Returns plant names, scientific names, family, genus, and basic growing attributes. Use this to identify crops before requesting detailed species data.

Search for crops and plants by name
- **get_crop_details**: Essential for crop planning and agronomic decision-making.

Get comprehensive information for a specific plant using its ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenFarm Agriculture** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How do I grow tomatoes according to OpenFarm?"

**🤖 AI Agent:**
> Searching OpenFarm for 'Tomato'... I found several guides. Common requirements include full sun, well-drained soil, and a sowing depth of about 0.5 inches. Would you like a detailed guide?


## Installation & Usage

To install and use the **OpenFarm Agriculture** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openfarm-agriculture](https://vinkius.com/mcp/openfarm-agriculture)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
