# The Met Museum MCP Server

Explore 470,000+ artworks from The Metropolitan Museum of Art — search by artist, title, culture, date and department.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/the-met-museum)

## Overview
**Category:** knowledge-management
**Tools Count:** 8

## Description
Connect to **The Met Museum** and explore one of the world's largest art collections through natural conversation — no API key needed.

### What you can do

- **Artwork Search** — Search 470,000+ artworks by artist name, title, culture, medium or any term
- **Artwork Details** — Get full metadata including title, artist, date, medium, dimensions, credit line and images
- **Department Browse** — Explore artworks by department (European Paintings, Egyptian Art, Asian Art, etc.)
- **Highlights** — Discover curator-selected highlights from the collection
- **On-View Objects** — Find artworks currently displayed in the museum galleries
- **Date Range Search** — Filter artworks by century or specific date ranges
- **Image Discovery** — Find artworks with Open Access CC0 images

### How it works

1. Subscribe to this server
2. No API key needed — all data is open access
3. Start exploring art from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Art Enthusiasts** — discover artworks, explore artists and learn about art history
- **Educators** — use artwork metadata and images for teaching and presentations
- **Researchers** — analyze art collections, provenance and cultural heritage data


## Available Tools
- **get_departments**: Useful for filtering searches by department (e.g. European Paintings, Egyptian Art, Asian Art, Arms and Armor).

Get all museum departments
- **get_object**: Returns title, artist, culture, date, medium, dimensions, credit line, repository URL, image URLs and more. All Open Access images are CC0 public domain.

Get detailed info for a specific artwork by object ID
- **get_objects_by_department**: Use get_departments first to find the department ID. Returns list of object IDs which can be used with get_object for full details.

Get all object IDs for a specific department
- **search_by_century**: Returns object IDs which can be used with get_object for full artwork details including images.

Search for objects created in a specific century
- **search_highlights**: These represent some of the most significant and popular works in the collection.

Search for highlighted (curator-selected) objects
- **search_objects**: Supports filtering by department, date range, medium, images, highlights and on-view status. Returns object IDs which can be used with get_object for full details.

Search The Met collection for artworks
- **search_on_view**: Useful for planning museum visits.

Search for objects currently on view in the museum
- **search_with_images**: Useful for finding visual artworks. Supports all standard search filters plus has_images=true.

Search for objects that have images


## Installation & Usage

To install and use the **The Met Museum** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/the-met-museum](https://vinkius.com/mcp/the-met-museum)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
