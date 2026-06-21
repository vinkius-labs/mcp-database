# Cooper Hewitt MCP Server

Access the Cooper Hewitt Smithsonian Design Museum collection — search objects, explore exhibitions, and retrieve detailed metadata about design history.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cooper-hewitt)

## Overview
**Category:** knowledge-management
**Tools Count:** 22

## Description
Connect to the **Cooper Hewitt Smithsonian Design Museum** API and explore one of the world's most comprehensive design collections directly through your AI agent.

### What you can do

- **Search the Collection** — Find objects, people, and media using keywords, colors, or specific time periods via `search_collection` and `search_objects`.
- **Object Details** — Retrieve rich metadata, including descriptions, participants, exhibition history, and color palettes using `get_object_info` and `get_object_colors`.
- **Visual Exploration** — Access high-quality images and visual assets for design research with `get_object_images`.
- **On Display** — See what is currently featured in the museum's physical galleries using `get_objects_on_display`.
- **Random Discovery** — Get inspired by pulling random objects from the vast archive with `get_random_object`.

### How it works

1. Subscribe to this server
2. Enter your Cooper Hewitt API Access Token
3. Start exploring design history from Claude, Cursor, or any MCP-compatible client

No more manual searching through web archives. Your AI acts as a specialized design historian and researcher.

### Who is this for?

- **Designers & Creatives** — find inspiration and historical context for projects directly in your workflow
- **Researchers & Students** — extract precise metadata and exhibition histories for academic or professional study
- **Developers** — integrate rich cultural heritage data into applications without complex API wrappers


## Available Tools
- **get_exhibition_info**: Return detailed information for an exhibition
- **get_exhibition_objects**: Return objects displayed in an exhibition
- **get_object_colors**: Return the color palette for an object
- **get_object_exhibitions**: Return exhibitions featuring an object
- **get_object_images**: Return images for an object
- **get_object_info**: Return detailed information for a specific object
- **get_object_participants**: Return people involved with an object
- **get_objects_on_display**: Return a list of objects currently on display
- **get_person_images**: Return images of a person
- **get_person_info**: Return detailed information for a person
- **get_person_objects**: Return objects associated with a person
- **get_random_object**: Return a random object from the collection
- **list_exhibitions**: Return a list of exhibitions
- **list_rooms**: List all rooms across locations
- **list_sites**: List all location sites
- **search_collection**: Search for things in the collection
- **search_objects_faceted**: Search for objects and return faceted results
- **search_objects**: Search specifically for objects
- **spec_formats**: Return the list of valid API response formats
- **spec_methods**: Return the list of available API response methods
- **test_echo**: A testing method which echoes all parameters back in the response
- **test_error**: Return a test error from the API


## Installation & Usage

To install and use the **Cooper Hewitt** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cooper-hewitt](https://vinkius.com/mcp/cooper-hewitt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
