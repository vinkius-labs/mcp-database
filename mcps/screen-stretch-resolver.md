# Screen Stretch Resolver MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/screen-stretch-resolver)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming](../categories/gaming.md)

Calculate pixel stretching, FOV shifts, and coordinate mapping for stretched resolutions.

## Description
The Screen Stretch Resolver is a precision utility designed for tactical shooter players who use stretched resolutions (like 4:3) on widescreen monitors (like 16:9). This MCP server provides tools to calculate the exact pixel expansion factors using `calculate_stretch_multipliers`, determine how your field of view changes with `analyze_fov_shift`, and translate crosshair or enemy positions from your stretched view back to native pixels with `map_coordinate_conversion`. It helps players understand the visual distortion and maintain accuracy when switching aspect ratios.


## Available Tools (3)
- **map_coordinate_conversion**: Translates a specific point on the screen from stretched space to native space
- **analyze_fov_shift**: Calculates how much the perceived field of view is altered by the aspect ratio change
- **calculate_stretch_multipliers**: Determines the magnitude of pixel expansion between resolutions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Screen Stretch Resolver** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am playing on 1280x960 (4:3) on a 1920x1080 monitor. What is my horizontal stretch multiplier?"

**🤖 AI Agent:**
> The horizontal scale factor is 1.5, meaning your horizontal pixels are expanded by 50%.

---

**👤 You:**
> "If my original FOV is 90 on a 16:9 monitor, what is the effective horizontal FOV when using 4:3 stretched?"

**🤖 AI Agent:**
> Your effective horizontal field of view is approximately 75.9 degrees.

---

**👤 You:**
> "Convert the point (640, 480) from a 1280x960 stretched resolution to my 1920x1080 native monitor."

**🤖 AI Agent:**
> The mapped coordinates on your native 1920x1080 screen are (960, 540).


## ❓ FAQ

**Q: How does the stretch multiplier calculation work?**
The `calculate_stretch_multipliers` tool compares your monitor's native resolution to your game's active resolution to find the horizontal and vertical expansion factors.

**Q: Can I use this to map crosshair positions?**
Yes, by using `map_coordinate_conversion`, you can take a coordinate from your stretched resolution and find its corresponding pixel position on your native monitor.

**Q: Does this tool account for FOV changes?**
Yes, the `analyze_fov_shift` tool calculates the effective horizontal field of view and the percentage change in visibility when you switch aspect ratios.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/screen-stretch-resolver](https://vinkius.com/mcp/screen-stretch-resolver)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Screen Stretch Resolver** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `screen-stretch-resolver` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Screen Stretch Resolver** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "screen-stretch-resolver": {
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
