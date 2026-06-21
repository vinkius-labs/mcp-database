# Flickr MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flickr-alternative)
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


## ❓ FAQ

**Q: Can I search for photos within a specific geographic area?**
Yes. Use the `search_photos` tool with the `lat` and `lon` parameters for radial queries, or the `bbox` parameter to define a specific rectangular bounding box.

**Q: How do I get the username and location of a Flickr member?**
You can use the `get_person_info` tool by providing the user's NSID (user_id). It will return their profile details, including username, real name, and location if public.

**Q: Is there a way to verify my API key is working correctly?**
Yes, you can use the `test_echo` tool. It simply echoes back any parameters you send, allowing you to confirm that the connection to the Flickr API is active.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flickr-alternative](https://vinkius.com/mcp/flickr-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flickr** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `flickr-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flickr** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flickr-alternative": {
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
