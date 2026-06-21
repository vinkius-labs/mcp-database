# The Met Museum MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/the-met-museum)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/the-met-museum-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/the-met-museum-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Explore 470,000+ artworks from The Metropolitan Museum of Art — search by artist, title, culture, date and department.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **The Met Museum** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for paintings by Monet."

**🤖 AI Agent:**
> Found 84 Monet paintings in the Met collection including: Water Lilies (1906), The Japanese Footbridge (1920), Rouen Cathedral series, and many Impressionist masterpieces with high-resolution images.

---

**👤 You:**
> "Show me the highlights from Egyptian Art."

**🤖 AI Agent:**
> Found 200+ Egyptian Art highlights including: Temple of Dendur (reconstructed in the museum), statues of pharaohs, sarcophagi, jewelry and papyrus scrolls spanning 3,000 years of Egyptian civilization.

---

**👤 You:**
> "Find sculptures from the 1800s."

**🤖 AI Agent:**
> Found 300+ sculptures from 1800-1899 including works by Rodin, Carpeaux and other 19th century masters. Each with dimensions, materials, credit lines and images.


## Installation & Usage

To install and use the **The Met Museum** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/the-met-museum](https://vinkius.com/mcp/the-met-museum)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
