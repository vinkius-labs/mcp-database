# Pexels MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pexels-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Search and retrieve high-quality royalty-free photos and videos from Pexels directly within your AI agent.

## Description
Connect to the **Pexels** library to discover millions of high-quality photos and videos. This server allows your AI agent to search, filter, and retrieve media assets for creative projects, content creation, and visual research.

### What you can do

- **Photo Search** — Find images by keyword with filters for orientation (landscape, portrait, square), size, and specific hex colors.
- **Video Discovery** — Search for videos or browse popular clips with duration and resolution filters to enhance your multimedia projects.
- **Curated Content** — Access hand-picked curated photos and popular videos directly from the Pexels community.
- **Collection Management** — Browse featured collections or access your own private collections and their media using specific IDs.
- **Detailed Metadata** — Fetch specific details, photographer information, and source URLs for any photo or video using its unique ID.

### How it works

1. Subscribe to this server
2. Enter your Pexels API Key
3. Start searching for visual assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — quickly find the perfect stock footage or background image for blog posts and social media.
- **Designers** — pull high-resolution assets directly into your workflow without leaving your AI-powered tools.
- **Marketing Teams** — automate the discovery of visual content that matches specific brand colors and orientations.


## Available Tools
- **get_collection_media**: Get all media within a specific collection
- **get_curated_photos**: Get a list of curated photos
- **get_featured_collections**: Get a list of featured collections
- **get_photo**: Get a single photo by its ID
- **get_video**: Get a single video by its ID
- **get_my_collections**: Get a list of your own collections
- **get_popular_videos**: Get a list of popular videos
- **search_photos**: Search for photos using a text query
- **search_videos**: Search for videos using a text query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pexels** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for landscape photos of 'minimalist architecture' with a white color theme."

**🤖 AI Agent:**
> I've found several landscape photos of minimalist architecture with white tones. Here are the top results from Pexels, including a stunning shot by photographer 'X' (ID: 12345).

---

**👤 You:**
> "Show me the most popular videos on Pexels right now."

**🤖 AI Agent:**
> Fetching current popular videos... I've found a selection of trending clips, including nature timelapses and urban drone shots. Which one would you like to see details for?

---

**👤 You:**
> "Get all media from my collection with ID 'abc123xyz'."

**🤖 AI Agent:**
> Accessing your collection... I've retrieved 12 items (8 photos and 4 videos) from your 'Project Assets' collection. Would you like the download links for any of them?


## ❓ FAQ

**Q: Can I search for photos that match a specific brand color?**
Yes! Use the `search_photos` tool and provide a hex code or color name in the `color` parameter to filter results by that specific palette.

**Q: How do I get the highest resolution link for a specific video?**
Use the `get_video` tool with the target Video ID. The agent will return all available file qualities and their direct download URLs.

**Q: Can I see the media inside my own Pexels collections?**
First, use `get_my_collections` to find your collection ID, then use `get_collection_media` with that ID to list all photos and videos stored inside.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pexels-alternative](https://vinkius.com/mcp/pexels-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pexels** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pexels-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pexels** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pexels-alternative": {
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
