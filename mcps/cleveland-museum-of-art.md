# Cleveland Museum of Art MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cleveland-museum-of-art)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Explore the Cleveland Museum of Art's collection — search artworks, creators, and exhibitions via Open Access API.

## Description
Access over 60,000 artworks from the **Cleveland Museum of Art** directly through your AI agent. This server connects to the CMA Open Access API, allowing for deep exploration of one of the world's most distinguished comprehensive art museums.

### What you can do

- **Artwork Search** — Filter the collection by keyword, department, technique, or even specific artist demographics like African American or LGBTQ artists.
- **Visual Discovery** — Use image similarity search to find visually related pieces within the collection.
- **Creator Insights** — Retrieve detailed biographies and associated works for thousands of artists and creators.
- **Exhibition History** — Search and inspect past and current exhibitions held at the museum.
- **Metadata Access** — Get precise accession numbers, dimensions, and copyright statuses for any piece.

### How it works

1. Subscribe to this server
2. No API key is required for public access
3. Start exploring art history from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Art Historians & Researchers** — quickly cross-reference metadata and exhibition histories
- **Educators** — find high-quality CC0 images and artist biographies for lesson plans
- **Designers & Creatives** — use similarity search to find visual inspiration from historical masterpieces


## Available Tools (9)
- **get_exhibition**: Retrieve a specific exhibition by ID
- **get_may_show_creator**: Retrieve a specific May Show creator by ID
- **search_artworks**: Search for artworks and associated metadata
- **search_creators**: Search for creators in the collection
- **search_exhibitions**: Search for exhibitions
- **search_may_show_creators**: Search for artists who participated in the Cleveland Museum of Art "May Shows"
- **search_similar_artworks**: Uses POST but acts as a read-only query.

Image Similarity Search. Find visually similar artworks
- **get_artwork**: Retrieve a specific artwork by its Athena ID or accession number
- **get_creator**: Retrieve a specific creator record by ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cleveland Museum of Art** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for Impressionist paintings in the Cleveland Museum collection."

**🤖 AI Agent:**
> I've searched the collection using `search_artworks`. I found several notable Impressionist works, including pieces by Claude Monet and Berthe Morisot. Would you like the details for 'Water Lilies' (1915.634)?

---

**👤 You:**
> "Get full metadata for artwork with accession number 1953.424."

**🤖 AI Agent:**
> Using `get_artwork`, I've retrieved the record for 'The Crucifixion'. It is a 14th-century tempera on wood by an unknown Florentine artist, currently located in Gallery 204a.

---

**👤 You:**
> "Find information about the creator 'Vincent van Gogh'."

**🤖 AI Agent:**
> I've used `search_creators` to find Vincent van Gogh (ID: 1048). He was a Dutch Post-Impressionist painter (1853–1890). The museum holds several of his works, including 'The Large Plane Trees'.


## ❓ FAQ

**Q: How can I find artworks that are currently on view in the museum galleries?**
You can use the `search_artworks` tool and set the `currently_on_view` parameter to true. This will filter the results to show only pieces you can see in person at the museum.

**Q: Can I find visually similar artworks using an image file?**
Yes! The `search_similar_artworks` tool allows you to provide a local file path to an image. The server will then return artworks from the collection that share visual characteristics.

**Q: How do I get the full biography and details of a specific artist?**
Use the `get_creator` tool with the specific creator's ID. It will return their full biographical record, nationality, birth/death dates, and associated artworks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cleveland-museum-of-art](https://vinkius.com/mcp/cleveland-museum-of-art)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cleveland Museum of Art** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cleveland-museum-of-art` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cleveland Museum of Art** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cleveland-museum-of-art": {
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
