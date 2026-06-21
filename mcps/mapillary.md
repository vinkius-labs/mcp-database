# Mapillary MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mapillary)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Access street-level imagery — search images, sequences, traffic signs and map features worldwide.

## Description
Connect to **Mapillary** and access the world's largest street-level imagery platform through natural conversation.

### What you can do

- **Image Search** — Search street-level images by geographic bounding box
- **Image Details** — Get image metadata including GPS coordinates, capture date, compass angle and sequence
- **Sequence Search** — Find image sequences (connected images along routes) by area
- **Map Features** — Search detected traffic signs, objects and road markings by area
- **Object Detections** — Get all detected objects in a specific image

### How it works

1. Subscribe to this server
2. Enter your Mapillary access token
3. Start exploring street-level imagery from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Urban Planners** — analyze street-level imagery for infrastructure and traffic sign inventory
- **Researchers** — access geotagged imagery and map features for GIS and environmental studies
- **Developers** — integrate street-level imagery into mapping and navigation applications


## Available Tools
- **get_detection_value**: Returns the detected value, type, GPS coordinates and image association.

Get details for a specific object detection
- **get_image**: Returns image ID, capture date/time, GPS coordinates, compass angle, sequence ID, organization and thumbnail URL. Use fields parameter to request additional data like "geometry,compass_angle,captured_at,sequence,thumb_256_url,thumb_1024_url,altitude".

Get details for a specific Mapillary image
- **get_image_detections**: Returns detection values, types, geometry and confidence scores.

Get object detections for a specific image
- **get_map_features**: Returns feature type, value, GPS coordinates and detection confidence. Useful for traffic sign inventory and road infrastructure analysis.

Search map features (traffic signs, objects) by area
- **get_sequence**: Returns sequence ID, creation date and related images.

Get details for a specific image sequence
- **search_images**: Returns image IDs, coordinates, capture dates, compass angles and sequence IDs. Bbox format: min_lon,min_lat,max_lon,max_lat (e.g. "-0.15,51.50,-0.10,51.52" for central London).

Search street-level images by geographic area
- **search_sequences**: Returns sequence IDs and metadata for all sequences that pass through the area.

Search image sequences by geographic area


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mapillary** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find street-level images in central London."

**🤖 AI Agent:**
> Found 500+ images in central London bounding box. Images span major streets including Oxford Street, Regent Street and the Thames embankment. Each with GPS coordinates, capture dates and compass angles.

---

**👤 You:**
> "Search for traffic signs in São Paulo."

**🤖 AI Agent:**
> Found 200+ traffic signs including: speed limits (40km/h, 60km/h), stop signs, yield signs and no-parking zones. Each with GPS coordinates and detection confidence.

---

**👤 You:**
> "Get object detections for image abc123."

**🤖 AI Agent:**
> Found 8 detections: regulatory--maximum-speed-limit-50--g1, information--parking--g1, warning--curve-left--g1, object--street-light--g1, and 4 more. Each with value, geometry and confidence score.


## ❓ FAQ

**Q: How do I get a Mapillary access token?**
Sign up at [**mapillary.com/developer**](https://www.mapillary.com/developer) and create an application to get your access token.

**Q: What is a bounding box?**
A bounding box defines a geographic area using min_longitude, min_latitude, max_longitude, max_latitude. Example: "-0.15,51.50,-0.10,51.52" covers central London.

**Q: What map features are available?**
Mapillary detects traffic signs (stop, speed limit, yield, etc.), road objects (fire hydrants, mailboxes, etc.) and road markings. Use get_map_features to search by area.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mapillary](https://vinkius.com/mcp/mapillary)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mapillary** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mapillary` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mapillary** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mapillary": {
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
