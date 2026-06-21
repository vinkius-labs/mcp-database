# Macaulay Library MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/macaulay-library)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/macaulay-library-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/macaulay-library-mcp)
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


## Installation & Usage

To install and use the **Macaulay Library** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/macaulay-library](https://vinkius.com/mcp/macaulay-library)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
