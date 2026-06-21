# Flickr MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flickr-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/flickr-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/flickr-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Search photos, explore albums, and retrieve detailed image metadata from the Flickr community.

## Description
Connect to the **Flickr** API to search one of the world's largest photo libraries and extract rich metadata directly through your AI agent.

### What you can do

- **Advanced Photo Search** — Find images using tags, free text, or specific upload dates via the `search_photos` tool.
- **Geographic Discovery** — Search for photos by latitude, longitude, or bounding boxes to find visual content from specific locations.
- **Detailed Metadata** — Use `get_photo_info` to retrieve descriptions, titles, and technical details for any public photo.
- **User & Profile Insights** — Fetch user statistics, locations, and profile information using `get_person_info`.
- **Album Exploration** — List all public photosets (albums) belonging to any user with `list_photosets` to understand their curated collections.

### How it works

1. Subscribe to this server
2. Enter your Flickr API Key
3. Start exploring the world of photography from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Find inspiration and reference images using specific tags and text searches.
- **Researchers** — Gather geographic visual data and metadata for specific regions or time periods.
- **Developers** — Test API connectivity and parameter passing using the built-in `test_echo` utility.


## Available Tools
- **get_person_info**: Get information about a user
- **get_photo_info**: Get detailed metadata for a photo
- **list_photosets**: Returns the albums (photosets) belonging to a user
- **search_photos**: Search for photos on Flickr
- **test_echo**: A testing method that echoes back all passed parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flickr** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for photos of 'mountains' with the tag 'landscape'."

**🤖 AI Agent:**
> I've searched Flickr for 'mountains' with the tag 'landscape'. I found several high-quality images. Would you like the details for any specific photo ID?

---

**👤 You:**
> "Get the metadata and description for photo ID 534211092."

**🤖 AI Agent:**
> Fetching info for photo 534211092... This photo is titled 'Golden Gate at Sunset' by user 'sf_photog'. It was taken with a Sony A7III and has 1,200 views.

---

**👤 You:**
> "List all albums for the user with ID 12345678@N01."

**🤖 AI Agent:**
> I found 3 public albums for this user: 'Summer Vacation 2023', 'Street Photography', and 'Macro Shots'. Which one would you like to explore?


## Installation & Usage

To install and use the **Flickr** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flickr-alternative](https://vinkius.com/mcp/flickr-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
