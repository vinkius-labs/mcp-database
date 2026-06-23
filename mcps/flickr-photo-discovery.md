# Flickr Photo Discovery MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flickr-photo-discovery)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Universal photography intelligence — search millions of public photos via AI.

## Description
Equip your AI agent with the world's most iconic photography database through the **Flickr** MCP server. This integration provides real-time access to the Flickr ecosystem, allowing your agent to search for public photos by keyword, retrieve detailed metadata (including EXIF-like data and descriptions), and explore the latest uploads from the global community. Whether you are looking for creative inspiration, sourcing reference images, or researching photographic trends, your agent acts as a dedicated photo curator through natural conversation.

### What you can do

- **Photo Search** — Find public images on Flickr by text, tags, or keywords.
- **Metadata Retrieval** — Access titles, descriptions, owner info, and dates for specific photos.
- **Trend Monitoring** — Retrieve the most recently uploaded public photos to stay updated with global creative output.
- **Curated Exploration** — Explore vast collections of thematic photography through automated queries.

### How it works

1. Subscribe to this server
2. Enter your Flickr API Key (get it at flickr.com/services/developer)
3. Start searching for photos from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators & Bloggers** — find high-quality reference images and creative inspiration.
- **Graphic Designers** — source visual ideas and thematic photography for mood boards.
- **Visual Researchers** — analyze photographic styles and social media trends.
- **Travel Enthusiasts** — explore specific locations through the eyes of the global photography community.


## Available Tools (3)
- **get_flickr_photo_info**: Get detailed information for a specific photo
- **get_recent_flickr_photos**: Get most recent public photos
- **search_flickr_photos**: Search for public photos on Flickr


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flickr Photo Discovery** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for Flickr photos of 'Tokyo at night'."

**🤖 AI Agent:**
> Searching Flickr... I've found several stunning night shots of Tokyo, including neon-lit streets in Shinjuku and the Tokyo Tower. Would you like to see the photo titles or links?

---

**👤 You:**
> "Show me the most recent photos uploaded to Flickr."

**🤖 AI Agent:**
> Retrieving the latest public uploads... Here are the most recent photos from the global community, featuring a mix of landscapes, street photography, and portraits. Would you like to inspect any of them in detail?

---

**👤 You:**
> "Get details for Flickr photo ID '5123456789'."

**🤖 AI Agent:**
> Inspecting photo... This image is titled 'Golden Gate Fog' by user 'PhotoEnthusiast'. It was taken on May 12, 2021, and has a detailed description about the camera settings used.


## ❓ FAQ

**Q: Can I search for photos taken in a specific city?**
Yes! Use the `search_flickr_photos` tool and include the city name in your text query. For more precision, you can also ask for specific tags related to that city.

**Q: Does this integration provide the direct image URL?**
Yes. The search results include a direct link (`url_m`) to the medium-sized version of the photo, which can be viewed in any web browser or reference in documents.

**Q: Can I see the technical metadata like camera settings?**
The `get_flickr_photo_info` tool retrieves titles, descriptions, and owner metadata. For exhaustive technical EXIF data, Flickr requires specific additional permissions not included in the standard discovery toolset.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flickr-photo-discovery](https://vinkius.com/mcp/flickr-photo-discovery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flickr Photo Discovery** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flickr-photo-discovery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flickr Photo Discovery** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flickr-photo-discovery": {
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
