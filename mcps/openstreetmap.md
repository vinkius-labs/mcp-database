# OpenStreetMap MCP Server

Access and edit OpenStreetMap data — manage changesets, query map elements, and retrieve geospatial data directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/openstreetmap)

## Overview
**Category:** data-management
**Tools Count:** 33

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


## Installation & Usage

To install and use the **OpenStreetMap** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openstreetmap](https://vinkius.com/mcp/openstreetmap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
