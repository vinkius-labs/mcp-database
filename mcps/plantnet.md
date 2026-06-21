# PlantNET MCP Server

Identify plant species, diseases, and cultivated varieties using the Pl@ntNet AI engine — analyze images and access global taxonomic data.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/plantnet)

## Overview
**Category:** image-video
**Tools Count:** 17

## Description
Connect the **Pl@ntNet** API to your AI agent to transform it into a powerful botanical assistant. This server allows you to identify thousands of plant species, detect diseases, and explore taxonomic referentials directly through natural conversation.

### What you can do

- **Species Identification** — Submit image URLs of leaves, flowers, fruits, or bark to identify species across global or regional projects.
- **Disease & Pest Detection** — Analyze plant health by identifying common diseases and pests from visual symptoms.
- **Cultivated Varieties** — Specifically identify crops and cultivated plant varieties (varieties/crops) from images.
- **Taxonomic Exploration** — List available projects, browse species lists, and align scientific names with official taxonomies.
- **Advanced Surveys** — Perform multi-species identification on high-resolution imagery (Beta) and estimate processing costs.

### How it works

1. Subscribe to this server
2. Enter your PlantNET API Key
3. Start identifying plants from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Botanists & Researchers** — Quickly verify species names and access regional taxonomic databases.
- **Farmers & Gardeners** — Identify pests and diseases affecting crops to take timely action.
- **Nature Enthusiasts** — Learn about the flora around you by simply providing a photo URL.


## Available Tools
- **list_diseases**: List identifiable plant diseases
- **get_quota**: Check current API quota
- **align_species_name**: Align a species name within a project
- **estimate_survey_cost**: Estimate cost for a multi-species survey
- **get_daily_quota**: Check daily API usage
- **list_languages**: Get the list of supported language codes
- **list_projects**: List Pl@ntNet projects (taxonomic referentials)
- **get_quota_history**: Check API quota history (Contractualized only)
- **get_status**: Check Pl@ntNet API service health status
- **identify_disease**: Identify plant diseases and pests from images
- **identify_species**: Project can be "all" or a specific project ID.

Identify a plant species from images
- **identify_variety**: Identify cultivated plant varieties from images
- **list_species**: Can be scoped to a specific project or global.

List species, optionally filtered by project
- **list_varieties**: List identifiable cultivated plant varieties
- **search_observations**: Search DarwinCore plant observations
- **search_plots**: Search DarwinCore plots
- **survey_tiles**: g., quadrat or drone imagery) to identify multiple species.

Identify multiple species in a single high-resolution image (Beta)


## Installation & Usage

To install and use the **PlantNET** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plantnet](https://vinkius.com/mcp/plantnet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
