# Macaulay Library MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/macaulay-library)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Access the world's largest archive of animal sounds and videos. Search for species media, browse recent uploads, and retrieve detailed metadata for bird and wildlife assets.

## Description
Connect to the **Macaulay Library** at the Cornell Lab of Ornithology. This MCP server allows AI agents to query a massive scientific database of bird and wildlife media, providing direct access to millions of photos, audio recordings, and videos.

### What you can do

- **Search Media** — Find specific media assets by species (taxon code), location, contributor, or media type (photo, audio, video).
- **Recent Uploads** — Track the latest wildlife media submissions globally or filtered by specific country or subnational region codes.
- **Asset Metadata** — Retrieve deep technical and scientific details for any specific cataloged asset using its unique ML Catalog Number.
- **Scientific Research** — Leverage structured data for ornithological studies, biodiversity monitoring, or educational content creation.

### How it works

1. Subscribe to this server
2. Enter your eBird API Token
3. Start exploring wildlife media from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Scientists** — quickly gather media datasets for specific species or regions for biodiversity analysis.
- **Educators & Content Creators** — find high-quality, scientifically-vetted media for lessons or nature-focused projects.
- **Birders & Enthusiasts** — explore recent sightings and study species vocalizations and plumages directly through an AI assistant.


## Available Tools
- **get_asset**: Retrieve detailed metadata for a specific media asset
- **get_recent_media**: Retrieve the most recently uploaded media assets
- **search_media**: Search for media assets in the Macaulay Library


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Macaulay Library** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for photos of the House Sparrow (houhou) in the Macaulay Library."

**🤖 AI Agent:**
> I've found several photos of the House Sparrow (Passer domesticus). Here are the most recent assets, including ML Catalog Numbers 614523011 and 614522981, both captured recently in North America.

---

**👤 You:**
> "Show me the most recent wildlife media uploaded from Brazil (BR)."

**🤖 AI Agent:**
> Fetching recent media from Brazil... I found 20 new assets, including a variety of bird vocalizations and photos of endemic species like the Saffron Toucanet and various Tanagers.

---

**👤 You:**
> "Get the detailed metadata for the asset with ML Catalog Number 456789."

**🤖 AI Agent:**
> Inspecting asset 456789... This is an audio recording of a Wood Thrush (Hylocichla mustelina) recorded by Peter Paul Kellogg. It was captured in New York, USA, and includes high-quality song phrases.


## ❓ FAQ

**Q: Can I filter my media search to only show audio recordings for a specific species?**
Yes! Use the `search_media` tool and set the `mediaType` parameter to 'a' (audio) along with the `taxonCode` for the species you are interested in.

**Q: How do I find the most recent media uploads from a specific country like Canada?**
You can use the `get_recent_media` tool and provide the `regionCode` (e.g., 'CA' for Canada) to fetch the latest submissions from that area.

**Q: What information can I get if I have a specific ML Catalog Number?**
By using the `get_asset` tool with the `mlCatalogNumber`, you will receive detailed metadata including species identification, location, date, contributor details, and technical specifications of the media.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/macaulay-library](https://vinkius.com/mcp/macaulay-library)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Macaulay Library** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `macaulay-library` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Macaulay Library** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "macaulay-library": {
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
