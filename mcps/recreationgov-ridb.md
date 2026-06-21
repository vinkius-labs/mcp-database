# Recreation.gov (RIDB) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/recreationgov-ridb)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/recreationgov-ridb-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/recreationgov-ridb-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access federal recreation data—find campgrounds, trails, and facilities across the US directly from your AI agent.

## Description
Connect to the **Recreation Information Database (RIDB)** and explore thousands of federal recreation sites, campgrounds, and historic landmarks across the United States through natural conversation.

### What you can do

- **Facility Discovery** — Search for campgrounds, visitor centers, and parks using keywords, states, or specific activities.
- **Geospatial Search** — Find recreation spots near specific coordinates using radial search parameters.
- **Detailed Metadata** — Fetch complete descriptions, operating hours, and management information for any facility or recreation area.
- **Activity Mapping** — List and filter by supported activities like hiking, fishing, or camping to find the perfect spot.
- **Visual Exploration** — Retrieve associated images and media for facilities and recreation areas to preview your destination.
- **Agency Insights** — Identify the federal organizations and agencies managing specific public lands.

### How it works

1. Subscribe to this server
2. Enter your RIDB API Key
3. Start exploring the great outdoors from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travelers & Campers** — quickly find available facilities and check activity support without manual searching
- **Developers & Researchers** — access structured federal data for geographic or environmental analysis
- **Outdoor Enthusiasts** — discover new recreation areas and view site media directly within your workflow


## Available Tools
- **get_activity**: Get details for a specific recreation activity
- **get_facility**: Get details for a specific recreation facility
- **get_organization**: Get details for a specific organization
- **get_recarea**: Get details for a specific recreation area
- **list_activities**: g., Hiking, Camping).

List supported recreation activities
- **list_facilities**: ) with optional filtering.

Retrieve information about recreation facilities
- **list_facility_media**: Retrieve media for a facility
- **list_organizations**: List federal agencies managing resources
- **list_recarea_media**: Retrieve media for a recreation area
- **list_recareas**: List recreation areas


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recreation.gov (RIDB)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all recreation facilities in Florida that support 'Hiking'."

**🤖 AI Agent:**
> I've searched the RIDB for facilities in Florida with hiking activities. I found several locations including the 'Ocala National Forest' and 'Everglades National Park' facilities. Would you like the specific details for one of these?

---

**👤 You:**
> "Show me the media and images for facility ID 233330."

**🤖 AI Agent:**
> Fetching media for facility 233330... I found 3 images showing the campground layout and the surrounding lake views. [Links to images provided].

---

**👤 You:**
> "What are the supported recreation activities I can search for?"

**🤖 AI Agent:**
> I can retrieve the full list of supported activities. Common ones include Camping, Hiking, Fishing, Boating, and Biking. Would you like me to list all available activity types from the database?


## Installation & Usage

To install and use the **Recreation.gov (RIDB)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/recreationgov-ridb](https://vinkius.com/mcp/recreationgov-ridb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
