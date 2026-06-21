# Artsy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/artsy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/artsy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/artsy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Global art database — search artists, artworks, and shows via AI.

## Description
Equip your AI agent with the most comprehensive art intelligence available via **Artsy**. This unified server provides your agent with instant access to millions of artworks, artist technical details, and global art fair schedules. Your agent can instantly search for specific artists, audit artwork descriptions, and explore art movements (genes) without you ever needing to browse an online gallery. Whether you are identifying a masterpiece or auditing the history of a specific genre, your agent acts as a dedicated art historian and gallery curator through natural conversation.

### What you can do

- **Art Discovery** — Search for thousands of artworks and artists by name, style, or movement.
- **Artist Intelligence** — Fetch complete metadata for artists, including biographies, birth dates, and locations.
- **Movement Auditing** — Retrieve detailed information about art 'genes' or categories like Impressionism or Pop Art.
- **Show & Fair Tracking** — Access global schedules and details for art shows and major fairs.
- **Technical Details** — Retrieve exact dimensions, mediums, and descriptions for individual artworks.

### How it works

1. Subscribe to this server
2. Enter your Artsy Client ID and Client Secret
3. Start managing your art intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Art Collectors & Enthusiasts** — instantly find the history and technical details of their favorite artworks.
- **Researchers & Students** — explore the nuances of art movements and artist profiles through an AI-guided interface.
- **Content Creators** — retrieve high-quality art descriptions and metadata for articles, videos, and media production.
- **Gallery & Museum Professionals** — stay updated on global shows and fairs for organizational planning.
- **Interior Designers** — search for artworks by style and movement to complement their projects.


## Available Tools
- **get_artist_details**: Get artist details
- **get_artwork_details**: Get artwork details
- **get_gene_details**: Get gene details
- **list_artworks**: List artworks
- **list_fairs**: List art fairs
- **list_genes**: g., Abstract, Cubism).

List art genes
- **list_shows**: List art shows
- **search_artsy**: Search Artsy for anything


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Artsy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for information about Andy Warhol."

**🤖 AI Agent:**
> Searching Artsy for 'Andy Warhol'... I've found his profile (ID: andy-warhol). He was a leading figure in the Pop Art movement. I can pull his full biography or a list of his famous artworks for you.

---

**👤 You:**
> "What is 'Impressionism' in art?"

**🤖 AI Agent:**
> Retrieving data for the 'Impressionism' movement... It originated in 19th-century France and is characterized by small, thin, yet visible brush strokes. I have a detailed description and a list of key artists like Monet and Renoir.

---

**👤 You:**
> "Show me artworks by Vincent van Gogh."

**🤖 AI Agent:**
> Fetching artworks by Vincent van Gogh... I've identified several masterpieces including 'The Starry Night' and 'Sunflowers'. I can provide technical details like medium and dimensions for any of these.


## Installation & Usage

To install and use the **Artsy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/artsy](https://vinkius.com/mcp/artsy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
