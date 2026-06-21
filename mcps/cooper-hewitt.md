# Cooper Hewitt MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cooper-hewitt)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cooper-hewitt-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cooper-hewitt-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the Cooper Hewitt Smithsonian Design Museum collection — search objects, explore exhibitions, and retrieve detailed metadata about design history.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cooper Hewitt** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for objects in the collection related to 'Bauhaus' that have images."

**🤖 AI Agent:**
> I've searched the collection for 'Bauhaus' items with images. I found several objects, including a 1923 wallpaper sample (ID: 18491569) and a tea infuser. Would you like to see the detailed metadata or images for any of these?

---

**👤 You:**
> "Give me the color palette for object ID 18639529."

**🤖 AI Agent:**
> Fetching the color profile for object 18639529... The palette includes 'Vivid Tangerine' (#FF9F80), 'Dark Charcoal' (#333333), and 'Light Gray' (#D3D3D3).

---

**👤 You:**
> "Show me a random object from the museum to inspire my next design project."

**🤖 AI Agent:**
> Here is a random selection: 'Bird and Anemone' textile (1882), designed by William Morris. It's a block-printed cotton fabric featuring intricate floral and avian patterns. Would you like to see its exhibition history?


## Installation & Usage

To install and use the **Cooper Hewitt** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cooper-hewitt](https://vinkius.com/mcp/cooper-hewitt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
