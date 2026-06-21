# Art Institute of Chicago MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/art-institute-of-chicago)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search and explore the Art Institute of Chicago's digital collection—artworks, artists, and gallery locations.

## Description
Access one of the world's most impressive art collections directly through your AI agent. The **Art Institute of Chicago** MCP server allows you to query thousands of artworks, research artist biographies, and explore the museum's physical and digital archives.

### What you can do

- **Artwork Discovery** — Search the entire collection by keyword or list artworks with specific metadata fields and pagination.
- **Artist Research** — Retrieve detailed information about 'agents' (artists, designers, and contributors) including their historical context.
- **IIIF Integration** — Fetch IIIF Manifests for artworks to access high-resolution image data and structural metadata.
- **Museum Geography** — Explore physical gallery spaces and the places associated with the origin of various pieces.
- **Deep Metadata** — Access specific fields like exhibition history, provenance, and technical descriptions for any object in the collection.

### How it works

1. Subscribe to this server
2. Provide a User-Agent string (used to identify your requests to the AIC API)
3. Start exploring art history from Claude, Cursor, or any MCP client

### Who is this for?

- **Educators & Students** — Quickly gather facts, artist dates, and artwork descriptions for research or lesson planning.
- **Designers & Creatives** — Find inspiration from centuries of human creativity with direct access to high-quality metadata.
- **Art Historians** — Query specific collection subsets and retrieve technical manifests without manual API calls.


## Available Tools (31)
- **get_agent**: Get details for a specific agent (artist)
- **get_article**: Get details for a specific article
- **get_artwork_manifest**: Get IIIF Manifest for a specific artwork
- **get_artwork**: Get details for a specific artwork
- **get_event**: Get details for a specific event
- **get_exhibition**: Get details for a specific exhibition
- **get_gallery**: Get details for a specific gallery
- **get_place**: Get details for a specific place
- **get_product**: Get details for a specific product
- **get_publication**: Get details for a specific publication
- **get_tour**: Get details for a specific tour
- **list_agents**: List agents (artists) in the collection
- **list_articles**: List articles
- **list_artworks**: List artworks in the Art Institute of Chicago collection
- **list_events**: List events
- **list_exhibitions**: List exhibitions
- **list_galleries**: List physical gallery spaces in the museum
- **list_places**: List places associated with artworks
- **list_products**: List products (Museum shop items)
- **list_publications**: List publications
- **list_tours**: List tours
- **search_agents**: Search agents (artists)
- **search_articles**: Search articles
- **search_artworks**: Search artworks in the Art Institute of Chicago collection
- **search_events**: Search events
- **search_exhibitions**: Search exhibitions
- **search_galleries**: Search galleries
- **search_places**: Search places
- **search_products**: Search products
- **search_publications**: Search publications
- **search_tours**: Search tours


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Art Institute of Chicago** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for artworks by Georges Seurat in the Art Institute of Chicago collection."

**🤖 AI Agent:**
> I found several artworks by Georges Seurat. The most famous is 'A Sunday on La Grande Jatte — 1884' (ID: 27992). Would you like to see the full details or the IIIF manifest for this painting?

---

**👤 You:**
> "Get the details for artwork ID 16568."

**🤖 AI Agent:**
> Artwork 16568 is 'The Old Guitarist' by Pablo Picasso, created in 1903. It is an oil on panel painting from his Blue Period. It is currently located in Gallery 249.

---

**👤 You:**
> "List the first 5 galleries in the museum."

**🤖 AI Agent:**
> Here are the first 5 galleries: Gallery 101 (Ancient Art), Gallery 102, Gallery 103, Gallery 104, and Gallery 105. Would you like to know which artworks are currently displayed in any of these?


## ❓ FAQ

**Q: How can I find artworks by a specific artist like Van Gogh?**
You can use the `search_artworks` tool with the query 'Van Gogh'. This will return a list of matching artworks. You can then use `get_artwork` with a specific ID to see full details.

**Q: Can I access high-resolution image data for these artworks?**
Yes. By using the `get_artwork_manifest` tool with an artwork ID, the server retrieves the IIIF Manifest, which contains links to high-resolution image endpoints and structural metadata.

**Q: Is it possible to find where a specific artwork is located in the museum?**
Yes, many artworks include gallery information. You can also use `list_galleries` to see a list of physical spaces and `get_artwork` to check the `gallery_title` or `gallery_id` fields for a specific piece.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/art-institute-of-chicago](https://vinkius.com/mcp/art-institute-of-chicago)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Art Institute of Chicago** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `art-institute-of-chicago` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Art Institute of Chicago** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "art-institute-of-chicago": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
