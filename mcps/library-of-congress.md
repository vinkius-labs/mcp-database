# Library of Congress MCP Server

Search and retrieve millions of historical items, maps, photos, and manuscripts from the world's largest library.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/library-of-congress)

## Overview
**Category:** knowledge-management
**Tools Count:** 8

## Description
Connect your AI agent to the **Library of Congress** (LOC) and explore the vast digital archives of the United States' oldest federal cultural institution. Access millions of records, from historical newspapers to rare maps and sound recordings.

### What you can do

- **Global Search** — Search across the entire LOC catalog including items, legislation, and blogs using the `search` tool.
- **Digital Collections** — Browse and list all available digital collections or drill down into specific ones like the 'Abraham Lincoln Papers' using `list_collections` and `get_collection_items`.
- **Format-Specific Discovery** — Filter your research by specific media types such as maps, audio, or photos with `search_format`.
- **Deep Bibliographic Research** — Retrieve detailed metadata and digital resource links for specific items using `get_item`.
- **OCR & Text Analysis** — Access full-text OCR, word coordinates, and context snippets for digitized documents via `get_text_service`.
- **Technical Image Metadata** — Fetch IIIF technical data for high-resolution images using `get_image_info`.

### How it works

1. Subscribe to this server
2. Enter your Library of Congress API Key (optional but recommended for higher rate limits)
3. Start researching historical data directly from your MCP-compatible client

### Who is this for?

- **Researchers & Historians** — Instantly find primary sources and bibliographic data without manual catalog navigation.
- **Educators & Students** — Access digitized manuscripts and historical records for curriculum development.
- **Data Scientists** — Utilize OCR services and metadata for large-scale historical text analysis.


## Available Tools
- **get_collection_items**: List items within a specific collection
- **list_collections**: List all digital collections
- **search_format**: g., maps, photos, audio).

Search items of a specific format
- **get_image_info**: json for a specific image identifier.

Get technical metadata about an image (IIIF)
- **get_item**: Get detailed bibliographic data for a single item
- **get_resource**: g., a specific page of a newspaper) using resource_id.

Get access to discrete digitized files
- **search**: using a keyword query.

Search the entire Library of Congress website
- **get_text_service**: Access full-text OCR, word coordinates, and context snippets


## Installation & Usage

To install and use the **Library of Congress** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/library-of-congress](https://vinkius.com/mcp/library-of-congress)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
