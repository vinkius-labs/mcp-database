# Photo Exhibit Wall Layout MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/photo-exhibit-wall-layout)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-tools](../categories/design-tools.md)

Calculates optimal positioning for framed prints on a wall.

## Description
This MCP server provides spatial planning tools for arranging photo exhibits. Use `calculate_layout` to find valid coordinates for frames, `validate_placement` to check for collisions or margin violations, `get_wall_utilization` to measure coverage density, and `find_optimal_spacing` to determine the maximum possible gap between items. It ensures all arrangements respect wall boundaries, safety margins, and inter-frame spacing requirements.


## Available Tools (4)
- **calculate_layout**: Determines a valid set of coordinates for a collection of frames within the specified wall constraints
- **find_optimal_spacing**: Suggests the maximum possible uniform inter-frame spacing that can be maintained for a given set of frames and a specific layout pattern
- **get_wall_utilization**: Calculates the density of the arrangement to help determine if the wall is overcrowded or underused
- **validate_placement**: Verifies if a specific set of coordinates for a set of frames is physically possible and adheres to all spacing rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Photo Exhibit Wall Layout** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a wall that is 200cm wide and 150cm high. I want to place three frames, each 40x40cm, with a 10cm safety margin and 15cm spacing between them. Where should I put them?"

**🤖 AI Agent:**
> The frames can be placed at the following coordinates: Frame 0 at (10, 10), Frame 1 at (65, 10), and Frame 2 at (120, 10).

---

**👤 You:**
> "What is the maximum spacing I can have between 4 frames (50x50cm) on a 300x200cm wall with a 20cm safety margin?"

**🤖 AI Agent:**
> The maximum possible uniform inter-frame spacing for this configuration is 45.5cm.

---

**👤 You:**
> "Is this layout valid? Wall: 100x100, Margin: 5, Spacing: 5. Frame 1: (10,10) size 20x20. Frame 2: (15,15) size 20x20."

**🤖 AI Agent:**
> No, the layout is invalid because Frame 1 overlaps Frame 2.


## ❓ FAQ

**Q: How do I find where to place my frames?**
You can use the `calculate_layout` tool to automatically determine a valid set of coordinates for your frames based on your wall dimensions and spacing constraints.

**Q: Can I check if my manual layout is safe?**
Yes, the `validate_placement` tool checks if your proposed coordinates respect safety margins and prevent frames from overlapping.

**Q: How much of my wall will be covered?**
The `get_wall_utilization` tool calculates the occupancy percentage and the remaining empty area of your wall.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/photo-exhibit-wall-layout](https://vinkius.com/en/ai-agent-connect/photo-exhibit-wall-layout)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Photo Exhibit Wall Layout** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `photo-exhibit-wall-layout` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Photo Exhibit Wall Layout** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "photo-exhibit-wall-layout": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
