# Feng Shui Bagua Mapper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/feng-shui-bagua-mapper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

Aligns a Bagua map to your floor plan based on entrance orientation.

## Description
The Feng Shui Bagua Mapper connects your physical space to the ancient Bagua energy map. By providing the orientation of your main entrance, you can use `orientationTool` to calculate the rotation, then apply `mapAreaTool` or `analyzeLayoutTool` to identify which life areas--such as Wealth, Love, or Career--correspond to each room in your home. This tool bridges the gap between architectural layouts and spatial energy analysis.


## Available Tools (3)
- **get_orientation_offset**: Converts various entrance descriptions into a standardized numerical rotation value
- **analyze_room_layout**: Takes a collection of rooms and produces a complete mapping of room names to their corresponding Life Areas
- **map_coordinate_to_area**: Determines which single Life Area covers a specific point in space given a rotation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Feng Shui Bagua Mapper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the rotation offset for a North entrance?"

**🤖 AI Agent:**
> A North entrance corresponds to a 0 degree rotation offset.

---

**👤 You:**
> "Analyze this room: Name: Kitchen, X: 5, Y: -2 with a 45 degree offset."

**🤖 AI Agent:**
> The Kitchen is located in the Wealth & Prosperity sector.

---

**👤 You:**
> "Map a layout with two rooms: Living Room (0, 0) and Bedroom (2, 2), rotation offset 90."

**🤖 AI Agent:**
> The Living Room maps to the Career & Life Path area, and the Bedroom maps to the Children & Creativity area.


## ❓ FAQ

**Q: How do I determine my entrance orientation?**
You can use a compass or identify the cardinal direction (e.g., North, NE). Use `orientationTool` to convert this description into a rotation value.

**Q: What information do I need for the room layout analysis?**
You need a list of rooms with their names and center coordinates (x, y), along with the rotation offset calculated from your entrance orientation.

**Q: Can I map multiple rooms at once?**
Yes, use `analyzeLayoutTool` to get a complete mapping for all rooms in your floor plan at once.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/feng-shui-bagua-mapper](https://vinkius.com/mcp/feng-shui-bagua-mapper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Feng Shui Bagua Mapper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `feng-shui-bagua-mapper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Feng Shui Bagua Mapper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "feng-shui-bagua-mapper": {
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
