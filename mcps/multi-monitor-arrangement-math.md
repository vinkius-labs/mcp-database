# Multi-Monitor Arrangement Math MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/multi-monitor-arrangement-math)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate total desktop dimensions and coordinate offsets for multi-monitor setups.

## Description
This MCP server provides precise calculations for unified 2D coordinate planes in multi-monitor environments. By anchoring a primary monitor at (0,0), it determines the total bounding box dimensions and exact (X,Y) coordinate space maps for any configuration of connected displays. Use `get_bounding_box` to find the total desktop span, `get_coordinate_map` to retrieve individual monitor origins, and `get_monitor_area_percentage` to analyze screen real estate distribution.


## Available Tools (3)
- **get_bounding_box**: Calculate the bounding box of a multi-monitor setup
- **get_coordinate_map**: Get the top-left coordinates for each monitor
- **get_monitor_area_percentage**: Calculate the percentage of total area occupied by each monitor


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Multi-Monitor Arrangement Math** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the total dimensions of a setup with a 1920x1080 primary monitor and a 1920x1080 secondary monitor placed to the right, aligned to the top?"

**🤖 AI Agent:**
> The total desktop dimensions are 3rad 3840 pixels in width and 1080 pixels in height.

---

**👤 You:**
> "Calculate the coordinate map for a primary monitor (1920x1080) and a monitor placed at the bottom, centered."

**🤖 AI Agent:**
> The Primary Monitor is at (0, 0). The secondary monitor is located at (0, 1080).

---

**👤 You:**
> "What percentage of the total area does each monitor occupy in a setup with two identical 1920x1080 monitors?"

**🤖 AI Agent:**
> Each monitor occupies exactly 50.0% of the total desktop area.


## ❓ FAQ

**Q: How is the coordinate system anchored?**
The system uses a Primary Monitor as the anchor, fixing its top-left corner at the origin point (0, 0).

**Q: Can I calculate the total area of my setup?**
Yes, by using the `get_bounding_box` tool, you can determine the total width and height of your entire multi-monitor desktop area.

**Q: How do I find where a specific monitor is located?**
The `get_coordinate_map` tool provides the exact (X, Y) origin for every monitor in your configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/multi-monitor-arrangement-math](https://vinkius.com/mcp/multi-monitor-arrangement-math)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Multi-Monitor Arrangement Math** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `multi-monitor-arrangement-math` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Multi-Monitor Arrangement Math** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "multi-monitor-arrangement-math": {
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
