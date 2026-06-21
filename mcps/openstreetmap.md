# OpenStreetMap MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openstreetmap)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/openstreetmap-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/openstreetmap-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access and edit OpenStreetMap data — manage changesets, query map elements, and retrieve geospatial data directly from any AI agent.

## Description
Connect your AI agent to the world's largest open geographic database. This server enables full interaction with the **OpenStreetMap API (v0.6)**, allowing you to query, create, and update geospatial data through natural conversation.

### What you can do

- **Map Data Retrieval** — Fetch raw OSM data (nodes, ways, relations) within specific bounding boxes for analysis or visualization.
- **Element Management** — Create, read, update, or delete map elements including points of interest (nodes), roads (ways), and complex boundaries (relations).
- **Changeset Workflows** — Open, update, and close changesets to group your edits and provide meaningful metadata to the OSM community.
- **Historical Analysis** — Retrieve the full version history of any map element to track changes over time.
- **Advanced Querying** — Filter changesets by user, time range, or geographic area to monitor local mapping activity.

### How it works

1. Subscribe to this server
2. Enter your OpenStreetMap OAuth Token
3. Start exploring and editing the map from Claude, Cursor, or any MCP-compatible client

Your AI can now act as a GIS specialist, helping you audit map data or contribute to open-source geography without leaving your workspace.

### Who is this for?

- **GIS Analysts** — quickly extract raw map data for specific regions without manual exports
- **Open Source Contributors** — automate the creation of map elements and manage changesets via chat
- **Developers** — inspect map element metadata and history directly while building location-based services


## Available Tools
- **close_changeset**: Close a changeset
- **close_note**: Close a map note
- **comment_note**: Add a comment to an existing map note
- **create_changeset**: Create a new changeset
- **create_element**: Create a new node, way, or relation
- **create_note**: Create a new map note
- **delete_element**: Delete a node, way, or relation
- **delete_message**: Delete a message
- **download_changeset**: Download a changeset in OsmChange format
- **get_auth_user_details**: Get details for the authenticated user
- **get_changeset**: Read a changeset by ID
- **get_element_history**: Get the history of a node, way, or relation
- **get_element**: Read a node, way, or relation by ID
- **get_elements**: Multi-fetch nodes, ways, or relations
- **get_gpx_data**: Download data for a GPS trace
- **get_gpx_metadata**: Read metadata for a GPS trace
- **get_inbox**: Get the authenticated user's message inbox
- **get_map_data**: Get map data (nodes, ways, relations) within a bounding box
- **get_message**: Read a specific message
- **get_note**: Read a map note by ID
- **get_outbox**: Get the authenticated user's message outbox
- **get_permissions**: Get OAuth permissions for the authenticated user
- **get_user_preferences**: Get preferences for the authenticated user
- **get_user**: Get details for a specific user
- **list_notes**: List map notes within a bounding box
- **list_user_gpx**: List GPS traces for the authenticated user
- **query_changesets**: Query changesets with filters
- **search_notes**: Search for map notes
- **send_message**: Send a private message to another user
- **update_changeset**: Update tags of an open changeset
- **update_element**: Update an existing node, way, or relation
- **update_message_status**: Update the read status of a message
- **upload_gpx**: Upload a GPS trace (GPX)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenStreetMap** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get map data for the bounding box -0.15, 51.50, -0.10, 51.52 (Central London)."

**🤖 AI Agent:**
> I've retrieved the map data for that area. It contains 142 nodes and 24 ways. Would you like me to list the primary road names or points of interest found?

---

**👤 You:**
> "Show me the history of way ID 4225123."

**🤖 AI Agent:**
> Inspecting history for Way 4225123... This element has 4 versions. It was originally created in 2015 and last updated by user 'MapMaster' in 2023 to add a 'bicycle_lane' tag.

---

**👤 You:**
> "Find the 5 most recent closed changesets by user 'JohnDoe'."

**🤖 AI Agent:**
> Searching for changesets... I found 5 recent closed changesets for 'JohnDoe'. The most recent one (ID: 1452390) involved updates to building footprints in Berlin. Would you like to download the details of any specific changeset?


## Installation & Usage

To install and use the **OpenStreetMap** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openstreetmap](https://vinkius.com/mcp/openstreetmap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
