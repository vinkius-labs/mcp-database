# Felt (Collaborative Maps) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/felt-collaborative-maps)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Create and manage collaborative maps — upload geographic data, style layers, and manipulate map elements directly from any AI agent.

## Description
Connect **Felt** to your AI agent to take full control of your collaborative mapping workflows through natural conversation. This server allows you to manage maps, layers, and geographic elements without leaving your workspace.

### What you can do

- **Map Management** — List all accessible maps, create new ones with specific viewports, and retrieve detailed metadata or delete maps.
- **Data Uploads & Layers** — Create layers by uploading geographic data (GeoJSON, CSV, KML) via public URLs and monitor their processing status.
- **Dynamic Styling** — Update layer names and apply complex visual styles using the Felt Style Object (FSO) programmatically.
- **Element Manipulation** — Add, update, or delete specific geographic features like points, lines, and polygons within your map layers.
- **Spatial Analysis Context** — Fetch map and layer details to provide your AI with the necessary context for spatial reasoning.

### How it works

1. Subscribe to this server
2. Enter your Felt API Token
3. Start building and editing maps from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **GIS Analysts & Data Scientists** — quickly prototype maps and upload datasets for visualization using simple commands.
- **Urban Planners & Researchers** — manage collaborative project maps and update elements as field data comes in.
- **Logistics & Ops Teams** — visualize routes and service areas by programmatically adding elements to shared maps.


## Available Tools (11)
- **create_layer**: Supports GeoJSON, CSV, KML, Shapefiles, etc.

Create a layer (Upload Data) to a Felt map
- **create_map**: Create a new Felt map
- **delete_element**: Delete a Felt element
- **delete_layer**: Delete a Felt layer
- **delete_map**: Delete a Felt map
- **get_layer**: Get details for a specific Felt layer
- **get_map**: Get details for a specific Felt map
- **list_maps**: List Felt maps
- **update_element**: Update a Felt element
- **update_layer**: Update a Felt layer
- **add_elements**: Add elements to a Felt layer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Felt (Collaborative Maps)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current Felt maps."

**🤖 AI Agent:**
> I've retrieved your maps. You have 3 active maps: 'Urban Planning 2024', 'Logistics Hubs', and 'Environmental Study'. Which one would you like to inspect?

---

**👤 You:**
> "Create a new map titled 'Project Alpha' centered on San Francisco."

**🤖 AI Agent:**
> Map 'Project Alpha' has been created successfully with ID `map_12345`. It is centered at latitude 37.7749 and longitude -122.4194.

---

**👤 You:**
> "Add a point element to layer `layer_abc` at [ -122.4, 37.8 ]."

**🤖 AI Agent:**
> I've added the point to the layer. The new element ID is `elem_9876`. You can now see it on your map.


## ❓ FAQ

**Q: Can I upload my own geographic data files to a map?**
Yes! Use the `create_layer` tool by providing a public URL to your GeoJSON, CSV, or KML file. The server will initiate the upload and processing into your specified Felt map.

**Q: How do I add a specific point or shape to an existing layer?**
You can use the `add_elements` tool. Simply provide the `layer_id` and a JSON array of GeoJSON features (points, lines, or polygons) you want to add to that layer.

**Q: Is it possible to change the visual style of a map layer?**
Yes. Use the `update_layer` tool and provide a 'Felt Style Object' (FSO) in the `style` parameter to programmatically change colors, icons, or visibility rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/felt-collaborative-maps](https://vinkius.com/mcp/felt-collaborative-maps)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Felt (Collaborative Maps)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `felt-collaborative-maps` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Felt (Collaborative Maps)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "felt-collaborative-maps": {
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
