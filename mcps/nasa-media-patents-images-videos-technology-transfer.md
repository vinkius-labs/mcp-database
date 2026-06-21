# NASA Media & Patents — Images, Videos & Technology Transfer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nasa-media-patents-images-videos-technology-transfer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Search NASA's library of 140,000+ images and videos from every mission: Apollo, ISS, Hubble, Webb, Mars rovers, and more — plus browse NASA's technology transfer portfolio of patents and commercial spinoffs available for licensing.

## Description
Two powerful resources in one server.

### NASA Image & Video Library
- 140,000+ images, videos, and audio
- Every mission from Mercury to Webb
- Full metadata and download URLs

### Technology Transfer
- NASA patents available for licensing
- Commercial spinoffs from space technology
- From memory foam to water purification


## Available Tools
- **search_media**: Covers every mission: Apollo, Space Shuttle, ISS, Hubble, Webb, Mars rovers, and more. Filter by media type and year range.

Search NASA's image and video library — 140,000+ assets
- **get_media_asset**: Use NASA IDs from search results.

Get download URLs for a NASA media asset by its NASA ID
- **get_media_metadata**: Get full metadata for a NASA media asset
- **search_patents**: NASA technologies have been adapted into thousands of commercial products — from memory foam to water purification systems.

Search NASA patents and technology spinoffs available for licensing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NASA Media & Patents — Images, Videos & Technology Transfer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for images of the James Webb Space Telescope"

**🤖 AI Agent:**
> 📸 **NASA Media: James Webb**

1,247 results found

1. 🌌 Webb's First Deep Field (2022) — 4,600 galaxies
2. 🪐 Jupiter in Infrared (2022)
3. ⭐ Carina Nebula 'Cosmic Cliffs' (2022)
4. 🔴 MIRI Instrument Testing (2020)

Each with full-resolution download URLs.

---

**👤 You:**
> "Find the original audio of Neil Armstrong's moon landing quote."

**🤖 AI Agent:**
> I found the audio file titled 'Apollo 11: One Small Step'. It's a historical recording from July 20, 1969, featuring Neil Armstrong's famous quote: 'That's one small step for [a] man, one giant leap for mankind.'

---

**👤 You:**
> "Show me some NASA patents related to robotics."

**🤖 AI Agent:**
> NASA holds numerous robotics patents available for licensing. Notable ones include a 'Robotic Gripper with Tactile Feedback' developed for the ISS, and a 'Tendon-Driven Anthropomorphic Robotic Hand' from JPL.


## ❓ FAQ

**Q: Can I use NASA images commercially?**
Most NASA images are in the public domain and free for commercial use. Some images from partner agencies (ESA, JAXA) may have restrictions — check the copyright field in the metadata.

**Q: Are audio files also included in the media library?**
Yes, the NASA Image and Video Library includes historical audio clips, such as the Apollo 11 moon landing broadcasts, space shuttle mission communications, and sonifications of cosmic data.

**Q: What kind of technologies are listed under Technology Transfer?**
The Technology Transfer portfolio includes software, patents, and spinoff technologies originally developed for space exploration, ranging from advanced materials to health and medicine innovations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasa-media-patents-images-videos-technology-transfer](https://vinkius.com/mcp/nasa-media-patents-images-videos-technology-transfer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NASA Media & Patents — Images, Videos & Technology Transfer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nasa-media-patents-images-videos-technology-transfer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NASA Media & Patents — Images, Videos & Technology Transfer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nasa-media-patents-images-videos-technology-transfer": {
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
